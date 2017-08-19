# Node.js Commands
<p align="center">
  <br><br>
  <img src="assets/images/nodejs-logo.png">
</p>

## Require

Require is used to include the modules into your project.

First, create an app.js file in the root of the project folder.

An example of using require to use the File System module:

```node
const fs = require ("fs");

fs.appendFile ("greetings.txt", "HelloWorld");

```

The 'fs' after the const acts like a variable name (so you can use anything) and  the "'fs' within the require function is the name of the module as it is in the docuumentation.

You can also require local files (such as function.js) to be used in your application files, and when the app file runs, the function file runs as well:

```node
const fs = require ("fs"),
      os = require ("os"),
      notes = require ("./notes.js");
```

There is an order in which you should require modules.

## NPM

|NPM Command|Description|
|:----------|:----------|
|`$ npm init`|Used to create package.json file|
|`$ npm install [package name] --save `|Installs package and saves it as a dependency in package.json|
|`$ npm install [package name] --save-dev `|Installs package and saves it as a dev dependency in package.json|
|`$ npm install [package name]@[version number] --save-dev `|As above but for a particular version of the package|
|`$ npm install [package name] -g `|Installs package globally - used for packages run in the terminal (does not add to package.json)*|
|`module.exports = { [function name] }`|Exports the function so it can be used elsewhere (ie app.js)|





*Packages that run in the command line do not need to be required. To run a package (such as Nodemon) type 'nodemon app.js' into the command line.

### A quick note about JSON

You can create JSON by creating a JavaScript object:

```javascript
var obj = {name: "Graeme"};
```

But JSON needs everything in double quotes. To do this, you can call the JSON function 'stringify' to turn an object into JSON.

```javascript
var stringifyObj = JSON.stringify(obj);
```

However, as all elements of the JSON data are now wrapped in double quotes ("name": "Graeme") you will need to use a JSON function called 'parse' in order to convert the JSON data back into an object to make it usable.

```javascript
var parsedObj = JSON.parse(stringifyObj)
```



### Usefall NPM packages

[g] Nodemon - Watches app.js file for changes and restarts app.js when changes occur.




























## Node.js Commands
### Setup

|Git Command|Description|
|:----------|:----------|
|`$ git config --global user.name "[name]"`|Set your username for all Git actions|
|`$ git config --global user.email "[email]"`|Set your email for all Git actions|
|`$ git config --list`|Lists all of the config values|

### Getting Started

First go to GitHub and add a new repository.

Inside the terminal, locate to the folder you would like to start tracking

|Git Command|Description|
|:----------|:----------|
|`$ git init`|Start tracking / initialise a repository from existing code|
|`$ rm -rf .git`|Stop tracking a repository|
|`$ touch .gitignore`|Creates a .ignore file of file extensions to ignore*|
|`$ git remote add origin [GitHub repo url]`|Creates remote repository pointing to GitHub**|

*Do this first, go to the editor and edit the .gitignore file, and add in .DS_Store plus anything else
**Only needs to be done once at the start of the process


