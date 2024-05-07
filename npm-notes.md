# Introduction to NPM
• npm is a package manager for JavaScript, useful for managing dependencies and automating tasks
• It helps with installing, publishing, and managing code libraries/packages, enhancing code reusability

* Using npm to Manage npm:
    • Verify npm CLI installation using __'npm -- version'__ or __'npm -v'__
    • Upgrade npm CLI using __'npm install -g npm@latest'__

* Using npm to Manage Project Dependencies:
    • Initialise a project with npm using __'npm init'__
    • Follow prompts to set package details like name, verion, description, etc.
    • Alternatively, use __'npm init --y'__ to accept default values
    • Utilise npm registry to find packages for project needs

* Installing Dependencies:
    • Install a package locally using __'npm install package-name'__
    • Package details are added to 'dependencies' in 'package.json'
    • Node modules are stored in 'node_modules' folder

* Using Dependencies in Code:
    • Import installed packages using __'require()'__ function
    • Example: __'const colors = require('colors');'__

* Dependency Types:
    • Two types: 'dependencies' (for production) and 'devDependencies' (for development)
    • DevDependencies are added using __'--save-dev'__ flag

* Summary:
    • Learn to verify/update npm, initialise projects, find/install packages, use packages in code
    • Understand the difference between regular dependencies and development dependencies


# Part Two

* Installing Existing Project's Dependencies:
    • Use __'npm install'__ in a project with 'package.json' and 'package-lock.json' to install dependencies listed
    • Output summarises installation status and potential funding needs
    • Vulnerabilities are checked during installation

* Uninstalling a Dependancy:
    • Remove unnecessary dependencies with __'npm uninstall package-name'__
    • Removes package and dependencies from 'node_modules' and updates 'package.json'

* Updating a Dependancy:
    • Update packages to fix bugs or add features with __'npm update package-name'__
    • Package version is updated in 'package.json'
    • Use __'npm update'__ to update all project dependencies

* Fixing Package Security Vulnerabilities
    • __'npm audit'__ checks for security vulnerabilities in installed packages
    • use __'npm audit fix'__ to fix vulnerabilities if possible, considering severity levels
    • Major version updates may require manual intervention or __'--force'__ flag

* Writing and Running npm Scripts:
    • Define scripts in 'package.json' under the 'scripts' field
    • Common predefined scripts include 'start' and 'test'
    • Custom scripts can be defined for specific project needs
    • Run scripts using __'npm run script-name'__


# CommonJS Modules:

• Organise code into multiple files for better maintainability and scalability
• Each JavaScript file in Node.js defines a module
• Modules can be local (within your project) or external (like built-in Node.js modules)
• Use __'module.exports'__ to export items from a module
• Use __'require()'__ to import items from a module
• Later, you can also use modules in JavaScript for browser-side scripting

* Exporting from a Module:
    • Option A: Assign an object to __'module.exports'__ with properties representing items to be exported
    • Option B: Set properties on __'module.exports'__ directly
    • Option C: Use the __'exports'__ shortcut, equivalent to __'module.exports'__

* Importing with 'require()':
    • Use __'require()'__ to import items from other modules
    • Provide a relative path to the module you want to import
    • File extensions (like '.js') ar not necessary

* Importing Multiple Items:
    • Imported items are properties of the exported object
    • Extract properties using object destructuring or direct assignment

* Importing Single Items:
    • If a module exports a single item, it's returned directly by __'require'__
    • No need for object destructuring

* Folder Modules:
    • A folder with an __'index.js'__ file can be loaded as a module
    • Use the folder name to import, Node.js looks for __'index.js'__ automatically
    • Useful for organising related files into a module

* Summary:
    • Learned how to structure a Node.js applications with local modules
    • Understand exporting and importing mechanisms
    • Recognise different export styles and when to use them
    • Note the ability to import folders as modules, with __'index.js'__ acting as the entry point
