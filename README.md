# ReactNativeDiary
- https://reactnative.dev/docs/environment-setup
- check compatiblity and stability of versions

# new technology shift
- learn setup
- learn api
- learn network call

# Setup
- Setup for development in mac for 
1. mobile dev
2. web
- Setup for windows

  1. Install choco, node, and JDK
  2. Install Andriod studio
  3. Downloads SDK and emulator
  4. Add environment variables
  5. Create RN App
  6. Run app



1. Install Node.js and npm
React Native requires Node.js to run. It also installs npm (Node Package Manager) which is used to install libraries and dependencies.

Go to Node.js download page.
Download the latest LTS version for Windows.
Run the installer and follow the on-screen instructions to complete the installation.
Verify the installation:

bash
Copy code
node -v
npm -v
2. Install JDK (Java Development Kit)
React Native uses Android Studio, which requires the Java Development Kit (JDK).

Go to AdoptOpenJDK or Oracle JDK and download the recommended version (OpenJDK 11 or JDK 8).
Install the JDK.
After installation, set the JAVA_HOME environment variable:

Right-click on This PC and select Properties.
Click on Advanced system settings and then Environment Variables.
Under System Variables, click New and add JAVA_HOME as the variable name, and the path to your JDK installation folder (e.g., C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot) as the variable value.
Add the JDK bin folder to your system PATH. For example, add C:\Program Files\AdoptOpenJDK\jdk-11.0.10.9-hotspot\bin.
Verify the Java installation:

bash
Copy code
java -version
3. Install Android Studio
Android Studio provides the Android SDK and Emulator to run React Native apps.

Download and install Android Studio.
During installation, ensure that you select the Android Virtual Device and Android SDK components.
After installation, open Android Studio and follow the setup wizard to install the necessary Android SDK components.
Set up Android SDK:

Go to File > Settings (or Configure > SDK Manager on the welcome screen).
Install the required Android SDK versions (e.g., Android 11 or newer).
Install the necessary Android SDK Build Tools, Android Emulator, and Android Support Repository.
Set the ANDROID_HOME environment variable to point to the Android SDK location. This is usually located in C:\Users\<YourUser>\AppData\Local\Android\Sdk.
Add Android SDK paths to your system PATH:

In the Environment Variables window, add the following paths to the Path variable under System variables:
C:\Users\<YourUser>\AppData\Local\Android\Sdk\platform-tools
C:\Users\<YourUser>\AppData\Local\Android\Sdk\tools
C:\Users\<YourUser>\AppData\Local\Android\Sdk\tools\bin
4. Install React Native CLI (Optional)
You can use either Expo CLI or React Native CLI. If you prefer to use the React Native CLI (which gives you more control), you need to install it globally.

bash
Copy code
npm install -g react-native-cli
5. Install React Native via npx (Recommended)
The recommended way to create a React Native app is by using npx to create a project without having to install the React Native CLI globally.

bash
Copy code
npx react-native init MyProject
cd MyProject
6. Start Android Emulator (Optional)
If you want to run your app on an Android emulator:

Open Android Studio.
Click on Configure > AVD Manager (Android Virtual Device Manager).
Create a new virtual device or choose an existing one and start the emulator.
7. Run the React Native Project
To run your project, open the command prompt and navigate to your project directory:

bash
Copy code
cd MyProject
npx react-native run-android
This will build the app and launch it on your Android emulator or connected physical device.

8. Troubleshooting
If you encounter errors:

Ensure all environment variables (e.g., JAVA_HOME, ANDROID_HOME) are set correctly.
Ensure your Android Emulator is running and has sufficient resources.
Check for any missing dependencies using react-native doctor.
     - mobile dev
   **how ??❓🤔**
     - method 1 
       1. vs code
       2. expo
       **Subdivision**
           1. vs code
           2. Enumerator  
      - method 2
       1. android
       2. expo
     
3. web
- set up for linux
1. app
2. web
- 


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
-  (NOBRIDGE) LOG  Bridgeless mode is enabled
 INFO 
 💡 JavaScript logs will be removed from Metro in React Native 0.77! Please use React Native DevTools as your default tool. Tip: Type j in the terminal to open (requires Google Chrome or Microsoft Edge).

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
1. expo
2. @expo/cli---> local/global
3. metro

- 

# Come to know 
- Adjust Babel Configuration (For Non-Expo Projects)

