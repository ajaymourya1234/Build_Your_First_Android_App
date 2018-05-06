## Create an Android project
This lesson shows you how to create a new Android project with Android Studio and describes some of the files in the project.<br />
First, be sure you have installed the latest version of Android Studio.[Download Android Studio here.](https://developer.android.com/studio/)
1. In the Welcome to **Android Studio window**, click **Start a new Android Studio project**.

<img src="https://developer.android.com/training/basics/firstapp/images/studio-welcome_2x.png">

Or if you have a project opened, select **File > New Project**.

2. In the **Create New Project** window, enter the following values:
- **Application Name**: "My First App"
- **Company Domain**: "example.com"<br />

You might want to change the project location. Also, if you want to write a Kotlin app, check the **Include Kotlin support** checkbox. Leave the other options as they are.

3. Click **Next**.
4. In the **Target Android Devices** screen, keep the default values and click **Next**.
5. In the **Add an Activity to Mobile** screen, select **Empty Activity** and click **Next**.
6. In the **Configure Activity** screen, keep the default values and click **Finish**.<br />
After some processing, Android Studio opens the IDE.
<img src="https://developer.android.com/training/basics/firstapp/images/studio-editor_2x.png">

Now take a moment to review the most important files.<br />
First, be sure the **Project** window is open (select **View > Tool Windows > Project**) and the **Android** view is selected from the drop-down list at the top of that window. You can then see the following files:<br />

**app > java > com.example.myfirstapp > MainActivity**<br />
This is the main activity (the entry point for your app). When you build and run the app, the system launches an instance of this Activity and loads its layout.<br />

**app > res > layout > activity_main.xml**<br />
This XML file defines the layout for the activity's UI. It contains a TextView element with the text "Hello world!".<br />

**app > manifests > AndroidManifest.xml**<br />
The manifest file describes the fundamental characteristics of the app and defines each of its components.<br />

**Gradle Scripts > build.gradle**<br />
You'll see two files with this name: one for the project and one for the "app" module. Each module has its own build.gradle file, but this project currently has just one module. You'll mostly work with the module's build.gradle file to configure how the Gradle tools compile and build your app. For more information about this file, see Configure Your Build.<br />

## Run Your App
Run on a real device
