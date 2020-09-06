<div align="center">
<img alt="Electron Aurelia Crossover Banner" src="https://raw.githubusercontent.com/soulehshaikh99/assets/master/create-electron-framework-app/readme/svg/Electron_Aurelia.svg" width="580" />
</div>
<br />
The boilerplate code to get started creating Cross-platform Desktop Apps with Electron and Aurelia as front-end technology.
<br />
<br />
<div align="center">

[![forthebadge](http://forthebadge.com/images/badges/built-by-developers.svg)](http://forthebadge.com)&nbsp;&nbsp;&nbsp;&nbsp;[![forthebadge](http://forthebadge.com/images/badges/makes-people-smile.svg)](http://forthebadge.com)<br />

[![forthebadge](http://forthebadge.com/images/badges/uses-html.svg)](http://forthebadge.com)&nbsp;&nbsp;&nbsp;[![forthebadge](http://forthebadge.com/images/badges/uses-css.svg)](http://forthebadge.com)&nbsp;&nbsp;&nbsp;[![forthebadge](http://forthebadge.com/images/badges/uses-js.svg)](http://forthebadge.com)

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

</div>

## ✒️ Overview

The aim of this project is to provide Web Developers using `aurelia` the power to create cross-platform desktop apps using `electron`.

#### 🧐 What packages does the project use?

**`electron`** enables you to create desktop applications with pure JavaScript by providing a runtime with rich native (operating system) APIs. You could see it as a variant of the Node.js runtime that is focused on desktop applications instead of web servers.

**`electron-builder`** is used as a complete solution to package and build a ready for distribution (supports Numerous target formats) Electron app with "auto update" support out of the box.

**`electron-serve`** is used for Static file serving for Electron apps.

**`aurelia`** is an amazing framework that embraces simple and clean code without sacrificing power. Aurelia's standards-based, unobtrusive style makes it the only framework that empowers you to build components using vanilla JavaScript or TypeScript. At the core of Aurelia is a high-performance, reactive system, capable of batching DOM updates in a way that leaves other frameworks, and their virtual DOMs, in the dust. Experience consistent, scalable performance, no matter how complex your UI.

**`concurrently`** is used to run multiple commands concurrently.

**`wait-on`** is used as it can wait for sockets, and http(s) resources to become available.
<br />

## 🚀 Getting Started

**Note:** If you wish to use npm over yarn then modify `package.json` by replacing `yarn` with `npm` in `electron-dev` and `preelectron-pack` scripts.
But I strongly recommend using <em>yarn</em> as it is a better choice when compared to <em>npm</em>.

### 🤓 Use this boilerplate

```bash
# Clone the Project

# Use degit scaffolding tool
$ npx degit soulehshaikh99/create-aurelia-electron-app create-aurelia-electron-app
# or GitHub CLI Users
$ gh repo clone https://github.com/soulehshaikh99/create-aurelia-electron-app.git
# or Normal Git Users
$ git clone https://github.com/soulehshaikh99/create-aurelia-electron-app.git

# Switch location to the cloned directory
$ cd create-aurelia-electron-app

# Install dependencies
$ yarn # or npm install

# Run your app
$ yarn electron-dev # or npm run electron-dev

# Package Your App
$ yarn electron-pack # or npm run electron-pack
```

### 💫 Create this boilerplate from scratch (Manual Setup)

#### 1) Start by installing aurelia-cli globally

```bash
$ yarn global add aurelia-cli
# npm i -g aurelia-cli
```

#### 2) Create a aurelia project using aurelia-cli

```bash
$ au new create-aurelia-electron-app
```

#### 3) Switch to project directory

```bash
$ cd create-aurelia-electron-app
```

#### 4) Move all dependencies to devDependencies using IDE / Text Editor

```bash
"dependencies": {},
"devDependencies": {
  "@babel/core": "^7.11.1",
  "@babel/plugin-proposal-class-properties": "^7.10.4",
  "@babel/plugin-proposal-decorators": "^7.10.5",
  "@babel/plugin-syntax-dynamic-import": "^7.8.3",
  "@babel/preset-env": "^7.11.0",
  "@babel/register": "^7.10.5",
  "app-settings-loader": "^1.0.6",
  "aurelia-animator-css": "^1.0.4",
  "aurelia-bootstrapper": "^2.3.3",
  "aurelia-cli": "^2.0.0",
  "aurelia-loader-nodejs": "^1.1.0",
  "aurelia-pal-nodejs": "^2.0.0",
  "aurelia-testing": "^1.0.0",
  "aurelia-webpack-plugin": "^4.0.0",
  "babel-eslint": "^10.1.0",
  "babel-jest": "^26.3.0",
  "babel-loader": "^8.1.0",
  "babel-plugin-istanbul": "^6.0.0",
  "clean-webpack-plugin": "^3.0.0",
  "copy-webpack-plugin": "^6.0.3",
  "css-loader": "^4.2.1",
  "duplicate-package-checker-webpack-plugin": "^3.0.0",
  "eslint": "^7.7.0",
  "expose-loader": "^1.0.0",
  "file-loader": "^6.0.0",
  "gulp": "^4.0.2",
  "gulp-eslint": "^6.0.0",
  "html-loader": "^1.1.0",
  "html-webpack-plugin": "^4.3.0",
  "istanbul-instrumenter-loader": "^3.0.1",
  "jest": "^26.4.0",
  "jest-cli": "^26.4.0",
  "jest-transform-stub": "^2.0.0",
  "json-loader": "^0.5.7",
  "mini-css-extract-plugin": "^0.10.0",
  "minimatch": "^3.0.4",
  "promise-polyfill": "^8.1.3",
  "regenerator-runtime": "^0.13.7",
  "style-loader": "^1.2.1",
  "tree-kill": "^1.2.2",
  "url-loader": "^4.1.0",
  "webpack": "^4.44.1",
  "webpack-bundle-analyzer": "^3.8.0",
  "webpack-cli": "^3.3.12",
  "webpack-dev-server": "^3.11.0"
}
```

#### 5) Install Development Dependencies

```bash
$ yarn add --dev electron electron-builder wait-on concurrently
# npm i -D electron electron-builder wait-on concurrently
```

#### 6) Install Production Dependency

```bash
$ yarn add electron-serve # or npm i electron-serve
```

#### 7) Your dependencies should look something like this

```json
"dependencies": {
  "electron-serve": "^1.0.0"
},
"devDependencies": {
  "@babel/core": "^7.11.1",
  "@babel/plugin-proposal-class-properties": "^7.10.4",
  "@babel/plugin-proposal-decorators": "^7.10.5",
  "@babel/plugin-syntax-dynamic-import": "^7.8.3",
  "@babel/preset-env": "^7.11.0",
  "@babel/register": "^7.10.5",
  "app-settings-loader": "^1.0.6",
  "aurelia-animator-css": "^1.0.4",
  "aurelia-bootstrapper": "^2.3.3",
  "aurelia-cli": "^2.0.0",
  "aurelia-loader-nodejs": "^1.1.0",
  "aurelia-pal-nodejs": "^2.0.0",
  "aurelia-testing": "^1.0.0",
  "aurelia-webpack-plugin": "^4.0.0",
  "babel-eslint": "^10.1.0",
  "babel-jest": "^26.3.0",
  "babel-loader": "^8.1.0",
  "babel-plugin-istanbul": "^6.0.0",
  "clean-webpack-plugin": "^3.0.0",
  "concurrently": "^5.3.0",
  "copy-webpack-plugin": "^6.0.3",
  "css-loader": "^4.2.1",
  "duplicate-package-checker-webpack-plugin": "^3.0.0",
  "electron": "^10.1.1",
  "electron-builder": "^22.8.0",
  "eslint": "^7.7.0",
  "expose-loader": "^1.0.0",
  "file-loader": "^6.0.0",
  "gulp": "^4.0.2",
  "gulp-eslint": "^6.0.0",
  "html-loader": "^1.1.0",
  "html-webpack-plugin": "^4.3.0",
  "istanbul-instrumenter-loader": "^3.0.1",
  "jest": "^26.4.0",
  "jest-cli": "^26.4.0",
  "jest-transform-stub": "^2.0.0",
  "json-loader": "^0.5.7",
  "mini-css-extract-plugin": "^0.10.0",
  "minimatch": "^3.0.4",
  "promise-polyfill": "^8.1.3",
  "regenerator-runtime": "^0.13.7",
  "style-loader": "^1.2.1",
  "tree-kill": "^1.2.2",
  "url-loader": "^4.1.0",
  "wait-on": "^5.2.0",
  "webpack": "^4.44.1",
  "webpack-bundle-analyzer": "^3.8.0",
  "webpack-cli": "^3.3.12",
  "webpack-dev-server": "^3.11.0"
}
```

#### 8) Download the app icon

[favicon.png](https://raw.githubusercontent.com/soulehshaikh99/assets/master/framework-icons/aurelia/favicon.png) and place it in the static directory.

#### 9) Add `output` configuration in `aurelia_project/aurelia.json`

```bash
# aurelia_project/aurelia.json
# This will make sure that the electron-builder and aurelia-cli
# has seperate directories for output.
{
  ...
  ...
  "platform": {
    ...
    ...
    "output": "build"
  }
}
```

#### 10) Create main.js file (serves as entry point for Electron App's Main Process)

```bash
# Windows Users
$ fsutil file createnew main.js 0
# notepad main.js

# Linux and macOS Users
$ touch main.js
```

#### 11) Paste the below code in main.js file

```js
// Modules to control application life and create native browser window
const { app, BrowserWindow } = require("electron");
const path = require("path");
const serve = require("electron-serve");
const loadURL = serve({ directory: "build" });

// Keep a global reference of the window object, if you don't, the window will
// be closed automatically when the JavaScript object is garbage collected.
let mainWindow;

function isDev() {
  return !app.isPackaged;
}

function createWindow() {
  // Create the browser window.
  mainWindow = new BrowserWindow({
    width: 800,
    height: 600,
    webPreferences: {
      nodeIntegration: true,
    },
    // Use this in development mode.
    icon: isDev()
      ? path.join(process.cwd(), "static/favicon.png")
      : path.join(__dirname, "build/favicon.png"),
    // Use this in production mode.
    // icon: path.join(__dirname, 'build/favicon.png'),
    show: false,
  });

  // This block of code is intended for development purpose only.
  // Delete this entire block of code when you are ready to package the application.
  if (isDev()) {
    mainWindow.loadURL("http://localhost:8080/");
  } else {
    loadURL(mainWindow);
  }

  // Uncomment the following line of code when app is ready to be packaged.
  // loadURL(mainWindow);

  // Open the DevTools and also disable Electron Security Warning.
  // process.env['ELECTRON_DISABLE_SECURITY_WARNINGS'] = true;
  // mainWindow.webContents.openDevTools();

  // Emitted when the window is closed.
  mainWindow.on("closed", function () {
    // Dereference the window object, usually you would store windows
    // in an array if your app supports multi windows, this is the time
    // when you should delete the corresponding element.
    mainWindow = null;
  });

  // Emitted when the window is ready to be shown
  // This helps in showing the window gracefully.
  mainWindow.once("ready-to-show", () => {
    mainWindow.show();
  });
}

// This method will be called when Electron has finished
// initialization and is ready to create browser windows.
// Some APIs can only be used after this event occurs.
app.on("ready", createWindow);

// Quit when all windows are closed.
app.on("window-all-closed", function () {
  // On macOS it is common for applications and their menu bar
  // to stay active until the user quits explicitly with Cmd + Q
  if (process.platform !== "darwin") app.quit();
});

app.on("activate", function () {
  // On macOS it's common to re-create a window in the app when the
  // dock icon is clicked and there are no other windows open.
  if (mainWindow === null) createWindow();
});
// In this file you can include the rest of your app's specific main process
// code. You can also put them in separate files and require them here.
```

#### 12) Update the script section of `package.json`

```bash
# Add this scripts
"electron": "wait-on http://localhost:8080 && electron .",
"electron-dev": "concurrently \"yarn run start\" \"yarn run electron\"",
"preelectron-pack": "yarn build",
"electron-pack": "electron-builder"

# You should end up with something similar
"scripts": {
  "build": "webpack --env.production --extractCss",
  "start": "webpack-dev-server --extractCss",
  "build:dev": "webpack --extractCss",
  "analyze": "webpack --env.production --analyze",
  "test": "au test",
  "electron": "wait-on http://localhost:8080 && electron .",
  "electron-dev": "concurrently \"yarn run start\" \"yarn run electron\"",
  "preelectron-pack": "yarn build",
  "electron-pack": "electron-builder"
}
```

#### 13) Add the following configuration in `package.json`

**Note:** build configuration is used by electron-builder, modify it if you wish to add more packaging and native distribution options for different OS Platforms.

```bash
"main": "main.js",  # Application Entry Point, please verify entry point is set to main.js
"build": {
  "icon": "static/favicon.png",
  "productName": "Aurelia and Electron App",
  "files": [
    "build/**/*",
    "main.js"
  ],
  "win": {},  # Windows Specific Configuration
  "linux": {},  # Linux Specific Configuration
  "mac": {}  # MacOs Specific Configuration
}
```

#### 14) Test drive your app

```bash
# Run your app
$ yarn electron-dev # or npm run electron-dev

# Package Your App
$ yarn electron-pack # or npm run electron-pack
```

### 💯 Result

<div align="center">
<img alt="Electron Aurelia Window Screeenshot" src="https://raw.githubusercontent.com/soulehshaikh99/assets/master/create-electron-framework-app/readme/png/create-aurelia-electron-app.png" />
</div>

<h3>😍 Made with ❤️ from Souleh</h3>
 
[![forthebadge](http://forthebadge.com/images/badges/built-with-love.svg)](http://forthebadge.com)
<br/>

<h3>📋 License: </h3>
Licensed under the <a href="https://github.com/soulehshaikh99/create-aurelia-electron-app/blob/master/LICENSE">MIT License</a>.