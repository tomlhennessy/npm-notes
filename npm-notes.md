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
