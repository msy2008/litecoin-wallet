# LITECOIN WALLET

Welcome to _Litecoin Wallet_, a standalone Bitcoin payment app for your Android device!
This wallet for Litecoin is a fork of bitcoin.

This project contains several sub-projects:

 * __wallet__:
     The Android app itself. This is probably what you're searching for.
 * __market__:
     App description and promo material for the Google Play app store.


### PREREQUISITES FOR BUILDING

You'll need git, a Java 8 or 11 SDK and Gradle 4.4 (or later) for this. We'll assume Ubuntu 20.04 LTS (Focal Fossa)
for the package installs, which comes with OpenJDK 8, OpenJDK 11 and Gradle 4.4.1 out of the box.

    # first time only
    sudo apt install git gradle openjdk-8-jdk

Create a directory for the Android SDK (e.g. `android-sdk`) and point the `ANDROID_HOME` variable to it.

Download the [Android SDK Tools](https://developer.android.com/studio/index.html#command-tools)
and unpack it to `$ANDROID_HOME/`.

Finally, the last preparative step is acquiring the source code. Again in your workspace, use:

    # first time only
    git clone -b master https://github.com/msy2008/litecoin-wallet.git litecoin-wallet
    cd litecoin-wallet


### BUILDING

You can build all sub-projects in all flavors at once using Gradle:

    # each time
    gradle clean build

For details about building the wallet see the [specific README](wallet/README.md).
