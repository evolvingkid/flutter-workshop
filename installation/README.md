# Flutter Setup

To set up the flutter in your system you can go through the [official doc](https://docs.flutter.dev/get-started/install) or steps that we provided down below. 

## Installation
To setup flutter, you need:
* [Android Studio](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/README.md#android-installation)
* [Xcode](https://github.com/evolvingkid/flutter-workshop-1/tree/master/installation#xcode) (In mac devices) 
* [git](https://git-scm.com/)
* [Google chrome](https://www.google.com/intl/en_in/chrome/) (Planing to do flutter web)
* [Flutter SDK](https://github.com/evolvingkid/flutter-workshop-1/tree/master/installation#flutter-installation)

## Android Installation

Download android studio from the [official website](https://developer.android.com/studio). (For linux user you can also install it from store or snapstore).

![Android studio](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/Screenshot%202022-01-27%20at%208.54.07%20PM.png)

After you install android studio open it and click next. You will get a prompt to choose SDK and the required package need to be installed. Agree on all of it and press finish. 

![android studio package](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/Screenshot%202022-01-27%20at%208.56.59%20PM.png)

Android studio will start downloading all of your required SDK and tools. Please make sure that your internet connection is stable. The time taken to install these tools will take up to 5 - 20 min (Depending on internet speed and system).

If you are using a low spec device it will not be a problem in most cases because we will be not running anything on android studio. We are just using android studio to install the required tools.

After installation we recommend you, open SDK manager from the more action button.

![more action button](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/Screenshot%202022-01-27%20at%209.08.33%20PM.png)

We recommend you install the SDK you want before setting up the flutter. So that, when you are running the flutter for the 1st time the time taken, will be decreased because we already have the SDK.

Now choose the SDK tool and then choose the hide obsolete package. Mark the android SDK command-line tool and install it.

![sdk tool](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/Screenshot%202022-01-28%20at%2012.43.36%20PM.png)

# Xcode
`The Xcode installation is only for mac users.`

You can install Xcode from the AppStore or website. After installation open the Xcode so that it will download the required tools.

![xcode install](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/Screenshot%202022-01-27%20at%209.13.28%20PM.png)

After this run the below commands.

``` 
sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer

sudo xcodebuild -runFirstLaunch

sudo xcodebuild -license

sudo gem install cocoapods
```

We doing the `sudo xcodebuild -runFirstLaunch` you may face and issues like:
```
objc[8902]: Class AMSupportURLConnectionDelegate is implemented in both /usr/lib/libauthinstall.dylib (0x201c0eb90) and /Library/Apple/System/Library/PrivateFrameworks/MobileDevice.framework/Versions/A/MobileDevice (0x103be02c8). One of the two will be used. Which one is undefined.
```

If this issues comes up Their is two [soloution](https://github.com/evolvingkid/flutter-workshop-1/tree/master/installation/IOS_ISSUES#class-amsupporturlconnectiondelegate-is-implemented-issues).

## Flutter installation

[Download the needed SDK from flutter official site.](https://docs.flutter.dev/get-started/install)

Setup your path to SDK. It differ from system to system. 

## Flutter Verification

To verify the flutter installation you can run flutter doctor.

```
flutter doctor
```

![doctor image](https://github.com/evolvingkid/flutter-workshop-1/blob/master/installation/Screenshot%202022-01-28%20at%208.06.14%20PM.png)

Run the `flutter doctor --android-licenses` command to solve the android warning.

`Chrome - develop for the web` error is showing because i didn't install google chrome in my device. And not planning to do flutter web any time soon.

`No devices available` warning is not an issues leave it for now.

# Extras

* In the future, if you want to have multiple flutter versions for your projects then you can use [fvm](https://fvm.app/) to have a different flutter version for your project.
