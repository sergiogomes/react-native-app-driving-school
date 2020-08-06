# React Native App - Driving School

React Native App - Driving School

## Preparing Environment

### Node & Watchman

We recommend installing Node and Watchman using Homebrew. Run the following commands in a Terminal after installing Homebrew:

```sh
brew install node
brew install watchman
```

Watchman is a tool by Facebook for watching changes in the filesystem. It is highly recommended you install it for better performance.

### Xcode & CocoaPods

The easiest way to install Xcode is via the Mac App Store. Installing Xcode will also install the iOS Simulator and all the necessary tools to build your iOS app.

If you have already installed Xcode on your system, make sure it is version 9.4 or newer.

#### Command Line Tools

You will also need to install the Xcode Command Line Tools. Open Xcode, then choose "Preferences..." from the Xcode menu. Go to the Locations panel and install the tools by selecting the most recent version in the Command Line Tools dropdown.

#### Installing an iOS Simulator in Xcode

To install a simulator, open Xcode > Preferences... and select the Components tab. Select a simulator with the corresponding version of iOS you wish to use.

#### CocoaPods

CocoaPods is built with Ruby and it will be installable with the default Ruby available on macOS. You can use a Ruby Version manager, however we recommend that you use the standard Ruby available on macOS unless you know what you're doing.

Using the default Ruby install will require you to use sudo when installing gems. (This is only an issue for the duration of the gem installation, though.)

```sh
sudo gem install cocoapods
```

### React Native Command Line Interface

React Native has a built-in command line interface. Rather than install and manage a specific version of the CLI globally, we recommend you access the current version at runtime using npx, which ships with Node.js. With npx react-native command, the current stable version of the CLI will be downloaded and executed at the time the command is run.

## Creating the Application

You can use React Native's built-in command line interface to generate a new project. Let's create a new React Native project called "driver-id-on-purse":

```sh
npx react-native init DriverIDonPurse
```

Navigate to ios foldes and run

```sh
cd ios
pod install
cd ..
```

Run instructions for iOS:
    • cd "/Users/sergiogomes/Documents/Workfolder/react-native-app-driving-school/DriverIDonPurse" && npx react-native run-ios
    - or -
    • Open DriverIDonPurse/ios/DriverIDonPurse.xcworkspace in Xcode or run "xed -b ios"
    • Hit the Run button

Run instructions for Android:
    • Have an Android emulator running (quickest way to get started), or a device connected.
    • cd "/Users/sergiogomes/Documents/Workfolder/react-native-app-driving-school/DriverIDonPurse" && npx react-native run-android

Run instructions for Windows and macOS:
    • See <https://aka.ms/ReactNative> for the latest up-to-date instructions.

## Running your React Native application

### Step 1: Start Metro

First, you will need to start Metro, the JavaScript bundler that ships with React Native. Metro "takes in an entry file and various options, and returns a single JavaScript file that includes all your code and its dependencies."—Metro Docs

To start Metro, run npx react-native start inside your React Native project folder:

```sh
npx react-native start
```

### Step 2: Start your application

Let Metro Bundler run in its own terminal. Open a new terminal inside your React Native project folder. Run the following:

```sh
npx react-native run-ios
```

You should see your new app running in the iOS Simulator shortly.

npx react-native run-ios is one way to run your app. You can also run it directly from within Xcode.

Within Xcode open the DriverIDonPurse.xcworkspace file.
