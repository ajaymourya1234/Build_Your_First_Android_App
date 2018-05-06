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
**Run on a real device**<br /><br />
Set up your device as follows:<br />

1. Connect your device to your development machine with a USB cable. If you're developing on Windows, you might need [install the appropriate USB driver](https://developer.android.com/studio/run/oem-usb).
2. Enable **USB debugging** in the **Developer options** as follows.<br />
First, you must enable the developer options:

a. Open the **Settings** app.<br />
b. (Only on Android 8.0 or higher) Select **System**.<br />
c. Scroll to the bottom and select **About phone**.<br />
d. Scroll to the bottom and tap **Build number** 7 times.<br />
e. Return to the previous screen to find **Developer options** near the bottom.<br />

Open **Developer options**, and then scroll down to find and enable **USB debugging**.<br />

Run the app on your device as follows:<br />

1. In Android Studio, click the **app** module in the **Project** window and then select **Run > Run** (or click **Run**  in the toolbar).
2. In the **Select Deployment Target** window, select your device, and click **OK**.
<img src="https://developer.android.com/training/basics/firstapp/images/run-device_2x.png">
Android Studio installs the app on your connected device and starts it. You should now see "Hello World!" displayed in the app running on your device.<br />

**Run on an emulator**<br /><br />
Run the app on an emulator as follows:<br />

1. In Android Studio, click the **app** module in the **Project** window and then select **Run > Run** (or click **Run**  in the toolbar).<br />
2. In the **Select Deployment Target** window, click **Create New Virtual Device**.<br />

<img src="https://developer.android.com/training/basics/firstapp/images/run-avd_2x.png">

3. In the **Select Hardware** screen, select a phone device, such as Pixel, and then click **Next**.<br />
4. In the **System Image** screen, select the version with the highest API level. If you don't have that version installed, a **Download** link is shown, so click that and complete the download.<br />
5. Click Next.<br />
6. On the **Android Virtual Device (AVD)** screen, leave all the settings alone and click **Finish**.<br />
7. Back in the **Select Deployment Target** dialog, select the device you just created and click **OK**.<br />
Android Studio installs the app on the emulator and starts it. You should now see "Hello World!" displayed in the app running on the emulator.
