cordova-plugin-firebasex-test
============================
This repo contains tested a Cordova app project to test cordova-plugin-firebasex plugin written by dpa99c

 CLI build instructions

    git clone https://github.com/dpa99c/cordova-plugin-firebasex-test.git && cd cordova-plugin-firebasex-test
    npm install
    
    cordova platform add ios
    cordova run ios
    
    cordova platform add android
    cordova run android

 Testing Cloud Messaging
If you want to test FCM using this project, you'll need to do the following:
 Android
- Change the package ID in the [config.xml](https://github.com/dpa99c/cordova-plugin-firebasex-test/blob/master/config.xml#L2) to another package ID.
- Set up a Firebase project and add an Android app which is configured for your package ID.
- Download the `google-services.json` for your app and overwrite the [one bundled with this project](https://github.com/dpa99c/cordova-plugin-firebasex-test/blob/master/www/google-services.json).
- Build and run your project on an Android device.

You can send notification (but not data) messages using the Firebase Console.

Here is my working example screenshots.

![1ce91782-99ff-41ba-b741-4ca49ab9d0c5](https://user-images.githubusercontent.com/96186474/149462673-01221c18-0cf5-4bc5-becc-05c09561fb54.jpeg)
![53ce1cd1-edcb-4c93-9ab5-c142e92c74d7](https://user-images.githubusercontent.com/96186474/149462685-ba01a381-ed1e-4d55-93df-853fe22d953f.jpeg)
