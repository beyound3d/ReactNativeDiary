# ReactNativeDiary
- https://reactnative.dev/docs/environment-setup
- check compatiblity and stability of versions

# Setup
```
npx create-expo-app@latest
```

**run**

```
npx expo start
```
```
npx expo start -c
```

```
 npm run start
```

**reset**
```
npm run reset-project
```

**Q:differnce between npm and npx**


 NPM is a package management that is used to install, uninstall, and update Javascript packages on your workstation, whereas NPX is a package executer that is used to directly execute Javascript packages without installing them.


**Vs code extnesions**
- ES7 React/Redux/GraphQL/React-Native snippets
- React-Native/React/Redux snippets for es6/es7
- React Native Elements Snippets
- ES7+ React/Redux/React-Native snippets


**splash screen**
- libarary
- figma direct page setup se hotta h
- code se bhi hotta h

**fonts**
- by plugins expo
- direct trying-custom font-ho gyi ass tesi
  
```
 npx react-native-asset
```

```
npm i react-native-asset
```

# how to set splash screen app icon and logo in react native
working on it in vs code

**module export**
- common.js
- ES Modules
    |         Common.js                      |             Es Modules                         |
    | ------------------------               | ---------------------------------------------- |
    |  // Exporting in ES Modules            |    // Exporting in CommonJS                    |
    |     export function greet() {          |     module.exports.greet = function() {        |
    |    console.log('Hello, world!');       |        console.log('Hello, world!');           |
    |    }                                   |              };                                |
    |                                        |                                                |
    |   // Importing in ES Modules           |    // Importing in CommonJS                    |
    |  import { greet } from './greet.js';   |      const { greet } = require('./greet');     |
    |     greet();                           |       greet();                                 |
 
# Api


# Css Properties

``` flex: 1,
justifyContent: "center",
```

```
  alignItems: "center",
```

# PowerShell
```
Remove-Item -Recurse -Force node_modules
```
# cmd

# git bash

# javascript terminal

CMD: rmdir /s /q node_modules
PowerShell: Remove-Item -Recurse -Force node_modules
Git Bash/WSL: rm -rf node_modules


CMD: del package-lock.json
PowerShell: Remove-Item package-lock.json
Git Bash/WSL: rm -f package-lock.json

**execution policy**
1. Open PowerShell as Administrator.
Set the execution policy:
```
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```

2. Run your Expo command:

```
expo r -c
```

3. Optionally, revert the execution policy:
```
Set-ExecutionPolicy Restricted -Scope CurrentUser
```

# Miscellaneous words
- including breaking changes
- overriding peer dependency/conflicts
-  high severity vulnerabilities

# points to ponder 
- if we want to clean cache we have to  use --force Recommended protections disabled.
- Use --force only when necessary: It's often better to try resolving dependency issues manually rather than forcing the installation.
  Try --legacy-peer-deps: For peer dependency conflicts, this is usually a safer option.- rmeove packages
-    

# Problems with depreaction
- expo@52.0.6
- install and delete node modules in different terminal
- Check for Updates in expo-router or Expo
newer versions of expo-router have been released that are compatible with Expo 52. Sometimes, dependency conflicts arise from older package versions, and package maintainers often release updates that fix these issues.
```
npm show expo-router
```
- expo cli

# Don't know what it is 
- legacy global expo-cli
- Check package.json for the versions of the following:
expo
@expo/cli
metro
- 

