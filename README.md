# android-cli

How to build and launch an Android app from the CLI

## Build APK

    $ git clone https://github.com/2020-DEV-050/TicTacToe.git

    $ export ANDROID_SDK_ROOT=/Users/johnsmith/Library/Android/sdk

    $ ./gradlew build
    
## Launch Android Emulator

### List Android Virtual Devices

    $ /Users/johnsmith/Library/Android/sdk/emulator/emulator -list-avd
    Nexus_5_API_21
    Nexus_5_API_22
    Nexus_5_API_23
    
### Launch Android Emulator

    $ /Users/johnsmith/Library/Android/sdk/emulator/emulator -avd Nexus_5_API_21

## Install app

    $ adb devices
    List of devices attached
    emulator-5554   device

    $ cd ./app/build/outputs/apk/debug
    
    $ adb -s emulator-5554 install app-debug.apk
