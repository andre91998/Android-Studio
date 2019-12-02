# Hello World Android App

## Important Concepts

* Apps provide multiple entry points

    Android apps are built as a combination of components that can be invoked individually. For example, an activity is a type of app   component that provides a user interface (UI).

    The "main" activity starts when the user taps your app's icon. You can also direct the user to an activity from elsewhere, such as from a notification or even from a different app.

Other components, such as broadcast receivers and services, allow your app to perform background tasks without a UI.

* Apps adapt to different devices

    Android allows you to provide different resources for different devices. For example, you can create different layouts for different screen sizes. The system determines which layout to use based on the screen size of the current device.

    If any of your app's features need specific hardware, such as a camera, you can query at runtime whether the device has that hardware or not, and then disable the corresponding features if it doesn't. You can specify that your app requires certain hardware so that Google Play won't allow the app to be installed on devices without them.

## Most Important Files 

Your app project has many files, here are the most important ones for you to understand at this moment:

* app > java > com.example.myfirstapp > MainActivity

    This is the main activity. It's the entry point for your app. When you build and run your app, the system launches an instance of this Activity and loads its layout.

* app > res > layout > activity_main.xml

    This XML file defines the layout for the activity's user interface (UI). It contains a TextView element with the text "Hello, World!"

* app > manifests > AndroidManifest.xml

    The manifest file describes the fundamental characteristics of the app and defines each of its components.

* Gradle Scripts > build.gradle

    There are two files with this name: one for the project, "Project: My First App," and one for the app module, "Module: app." Each module has its own build.gradle file, but this project currently has just one module. Use each module's build.file to control how the Gradle plugin builds your app. For more information about this file, see Configure your build.

## Running your first App

After forking or downloading this repository, in the "Welcome to Android Studio" window, select the second option: "Open an Existing Android Studio Project", and then select the correct path for the project on your computer.

You can also just select "Start a new Android Studio Project" because Android Studio generates a "Hello World" app as a default new project. If you do this, select "Empty Activity" in the "Choose your project" window.

#### Running on your Android Device

* Set up your Device
    * Connect your device to your development machine with a USB cable. If you developed on Windows, you might need to install the appropriate USB driver for your device.
    * Perform the following steps to enable USB debugging in the Developer options window:
        * Open the Settings app.
        * If your device uses Android v8.0 or higher, select System. Otherwise, proceed to the next step.
        * Scroll to the bottom and select About phone.
        * Scroll to the bottom and tap Build number seven times.
        * Return to the previous screen, scroll to the bottom, and tap Developer options.
        * In the Developer options window, scroll down to find and enable USB debugging.

* Running the App on your Device:
    * In Android Studio, select your app from the run/debug configurations drop-down menu in the toolbar.
    * In the toolbar, select the device that you want to run your app on from the target device drop-down menu.
    * Click **Run**: Android Studio then installs your app on your connected device and starts it.
