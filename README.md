# React-Native-OneSignal
>     react-native init onesignalexample //Init a project
>     yarn add react-native-onesignal // Add dependencies
>     react-native link react-native-onesignal // Link One Signal Plugin

In android/app/build.gradle upgrade buildToolsVersion to 23.0.2<br/>
Add this to android.defaultConfig

>      manifestPlaceholders = [manifestApplicationId: "${applicationId}",
>      onesignal_app_id: "YOUR_ONESIGNAL_ID",
>      onesignal_google_project_number: "YOUR_GOOGLE_PROJECT_NUMBER"]

In App.js
>     import OneSignal from 'react-native-onesignal';


>       componentDidMount() {
>       OneSignal.configure({});
>       }
