# android-basics

## Build an APK from the CLI

git clone https://github.com/2020-DEV-050/TicTacToe.git

set ANDROID_SDK_ROOT=/Users/johnsmith/Library/Android/sdk

    ./gradlew build
    
## List Android Virtual Devices

    $ /Users/johnsmith/Library/Android/sdk/emulator/emulator -list-avd
    Nexus_5_API_21
    Nexus_5_API_22
    Nexus_5_API_23
    
## Start Android Emulator

    $ /Users/johnsmith/Library/Android/sdk/emulator/emulator -avd Nexus_5_API_21

## List devices

    $ adb devices
    List of devices attached
    emulator-5554   device

## Install app

    $ cd ./app/build/outputs/apk/debug
    $ adb -s emulator-5554 install app-debug.apk
    
## Done
