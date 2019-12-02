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

* app > res > layout > activity_main.xml

* app > manifests > AndroidManifest.xml

* Gradle Scripts > build.gradle

## Running your first App

After forking or downloading this repository, in the "Welcome to Android Studio" window, select the second option: "Open an Existing Android Studio Project", and then select the correct path for the project on your computer.

