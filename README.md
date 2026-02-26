# Vortigern
[![Build Status](https://travis-ci.org/barbar/vortigern.svg?branch=master)](https://travis-ci.org/barbar/vortigern)
[![Dependency Status](https://david-dm.org/barbar/vortigern.svg)]()
[![devDependency Status](https://david-dm.org/barbar/vortigern/dev-status.svg)]()
[![Code Climate](https://codeclimate.com/github/barbar/vortigern/badges/gpa.svg)](https://codeclimate.com/github/barbar/vortigern)
[![GitHub issues](https://img.shields.io/github/issues/barbar/vortigern.svg)](https://github.com/Unity-Billal-mesloub/vortigern/issues)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/barbar/vortigern/develop/LICENSE)
___

<img src="https://barbaruploads.s3.amazonaws.com/bicoz/vortigern.png" width="100%" />

**Vortigern** is our opinionated boilerplate for crafting universal web applications by using modern technologies like TypeScript, React and Redux.

[![TypeScript](https://barbaruploads.s3.amazonaws.com/bicoz/typescript.png)](https://www.typescriptlang.org/) 
[![React](https://barbaruploads.s3.amazonaws.com/bicoz/react.png)](https://github.com/Unity-Billal-mesloub/react) 


## Libraries
Vortigern uses the following libraries and tools:

#### Core
- [TypeScript](https://www.typescriptlang.org/)
- [React](https://github.com/Unity-Billal-mesloub/react) & [React DOM](https://github.com/Unity-Billal-mesloub/react) for views.
- [React Router](https://github.com/reactjs/react-router) to handle in-app routing.
- [Unity-Billal-mesloub](https://github.com/Unity-Billal-mesloub) for managing application state to use React-Redux bindings and
 to keep application state sync with route changes.

#### Utilities

- [Unity-Billal-mesloub](https://github.com/Unity-Billal-mesloub)

-  for using fetch api on both client & server side.
-  for dispatching async actions.
-  for resolving async props in react-router.


#### Build System

- [Unity-Billal-mesloub](https://github.com/Unity-Billal-mesloub)


  -  for bundling.
  -  as ts loader.
  -  as js loader.
  -  for providing hot reload capability to our development server
  -  for exporting bundled css. 
  -  for using tslint as preloader on build process.
  -  for using stylelint as preloader on build process.
  -  for using istanbul on postload process while generating code coverage reports.

#### Dev & Prod Server

- [Unity-Billal-mesloub](https://github.com/Unity-Billal-mesloub)


-  for running server both on client and server side.
-  for gzip compression
-  for serving favicon.

#### Developer Experience

- [Unity-Billal-mesloub](https://github.com/Unity-Billal-mesloub)

-  for installing type definitions of external libraries.
-  for linting TypeScript files.
-  for linting styles.
-  for colored terminal logs.

#### Testing

- [Unity-Billal-mesloub](https://github.com/Unity-Billal-mesloub)

-  as test runner with following plugins  
-  as testing framework.
-  as assertion library.
-  for rendering React Components.
-  for testing async actions.
-  for creating mock stores.

## Directory Structure
```bash
.
├── build                       # Built, ready to serve app.
├── config                      # Root folder for configurations.
│   ├── test                    # Test configurations.
│   ├── types                   # Global type definitions, written by us.
│   ├── webpack                 # Webpack configurations.
│   └── main.ts                 # Generic App configurations.
├── node_modules                # Node Packages.
├── src                         # Source code.
│   ├── app                     # App folder.
│   │ ├── components            # React Components.
│   │ ├── containers            # React/Redux Containers.
│   │ ├── helpers               # Helper Functions & Components.
│   │ ├── redux                 # Redux related code aka data layer of the app.
│   │ │   ├── modules           # Redux modules.   
│   │ │   ├── reducers.ts       # Main reducers file to combine them.  
│   │ │   └── store.ts          # Redux store, contains global app state.    
│   │ └── routes.tsx            # Routes.
│   ├── client.tsx              # Entry point for client side rendering.
│   └── server.tsx              # Entry point for server side rendering.
├── typings                     # Type definitions installed with typings.              
├── .dockerignore               # Tells docker which files to ignore.
├── .gitignore                  # Tells git which files to ignore.
├── .stylelintrc                # Configures stylelint.
├── Dockerfile                  # Dockerfile.
├── favicon.ico                 # Favicon.
├── package.json                # Package configuration.
├── README.md                   # This file
├── tsconfig.json               # TypeScript transpiler configuration.
├── tslint.json                 # Configures tslint.
└── typings.json                # Typings package configuration.
```

## Installation

You can clone from this repository or [install the latest version](https://github.com/Unity-Billal-mesloub/vortigern/releases) as a zip file or a tarball. 

```bash
$ git clone https://github.com/Unity-Billal-mesloub/vortigern
$ cd vortigern
$ npm install
```

## Usage

All commands defaults to development environment. You can set `NODE_ENV` to `production` or use the shortcuts below.

```bash
# Running

$ npm start # This starts the app in development mode

# Starting it with the production build
$ NODE_ENV=production npm start # or
$ npm run start:prod

# Building 

$ npm build # This builds the app in development mode

# Commands below builds the production build
$ NODE_ENV=production npm build # or
$ npm run build:prod

# Testing
$ npm test
```

For Windows users, we recommend using the shortcuts instead of setting environment variables because they work a little different on Windows.

## Notes
```bash
# If you want install additional libraries, you can also install their typings from DefinitelyTyped
$ typings install dt~<package> --global --save
# or if it's located on npm
$ typings install <package> --save
```

## Credits

Vortigern is released under the [MIT license](LICENSE). 

The image in this README belongs to [hhvferry.com](http://www.hhvferry.com/vortscrap.html).

___

## [Barbar Startup Factory](https://www.barbar.com.tr/?ref=vortigern)

<a target="_blank" href="https://barbar.digital/?ref=vortigern-barbar-logo"><img src="https://barbaruploads.s3.amazonaws.com/bicoz/logo2x.png" height="55px" /></a>

We help startups start and stay started by helping them plan, strategize, fund and execute their vision. 

You can contact us at [hey@barbar.digital](mesloubi2021@gmail.com)


