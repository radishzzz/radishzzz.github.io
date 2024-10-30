---
title: Ultimate Samsung One UI Optimization Guide
categories:
  - en
  - Tutorials
tags:
  - Android
  - Samsung
  - One UI
thumbnail: 'https://image.radishzz.cc/image/01-oneui/01.webp'
excerpt: The ultimate guide to take you from zero to hero.
abbrlink: d88c9984
date: 2024-10-30 00:00:00
---


{% note info  %}
<i class="fa-solid fa-earth-americas mr-2"></i>This article is also available in [简体中文](../../posts/384776b2/).
{% endnote %}

{% note info  %}
<i class="fa-solid fa-circle-info mr-2"></i>View table of contents by switching to Desktop Mode.
{% endnote %}

This article is a mega root-free optimization guide for Samsung One UI, which is designed to help you improve your device's battery life and smoothness, and solve the problems of excessive power consumption, lagging and frame dropping. The guide describes various optimization methods and principles in detail. By following these methods, your samsung device will get superb battery life and a silky smooth experience, as if it has been reborn!

This guide is based on One UI 6.1, and has been remodeled by combining a lot of experience from previous users and personal experience. It's very long and will take about 30 minutes to read. You can get a general idea of what to expect by looking at the table of contents on the right. If you're ready, let's get started!




## The Wiping and Flashing

{% note info  %}
This chapter introduces that the effect and method of Wipe Data and Cache and Flashing ROM. This is not a required step unless you are a professional.
{% endnote %}

![ROM Flashing](https://image.radishzz.cc/image/01-oneui/02.webp)  

To decorate a house, it is best to start with a clean house. Similarly, if you want to optimize your device, the best place to start is with a clean system. A clean system can lay a good software foundation for the device, avoiding the impact of application uninstallation residues, system upgrade conflicts, device cache accumulation and other issues. So how do you get a clean system? There are three ways:

> - **Factory Reset**: Removes all user data, apps, personalization settings, restoring the device to its original factory state.
> - **Wipe Data and Cache**: Performs two wipe operations: wipe data/factory reset and wipe cache partition.
> - **Flashing ROM**: Installs a system firmware to completely reinstall the device's operating system.

**Ranking of cleaning results: Flashing ROM > Wipe Data and Cache > Factory Reset**. For most people, Factory Reset is enough. But for those of you who are able to read this article, you should not be limited to just that. Next I will describe the exact steps of Wipe Data and Cache and Flashing ROM. Newbies can try to simply Wipe Data and Cache, while veterans can just Flashing ROM. Please remember to backup important data before operation!

### Wipe Data and Cache

![Recovery Mode](https://image.radishzz.cc/image/01-oneui/03.webp)

> 1. Log out of your Samsung account and Google account and switch off your phone.
> 2. Press and hold the Power button and Volume + button while connecting to the computer with the data cable to enter the interface as above.
> 3. Select `Wipe data/factory reset` and then select `Factory data reset` to confirm.
> 4. Select `Wipe cache partition` then select `Yes` to confirm.
> 5. Select `Reboot system now`.

### Flashing ROM

![Flash Tool for Samsung Devices - Odin3](https://image.radishzz.cc/image/01-oneui/04.webp)  

#### Tools to prepare

- [Samsung Android USB Driver for Windows](https://developer.samsung.com/android-usb-driver)
- [Flash Tool for Samsung Devices Odin3](https://odindownloader.com/)
- Samsung Firmware download from [SamFirm](https://samfirmtool.com/) [Frijia](https://github.com/SlackingVeteran/frija) [Bifrost](https://github.com/zacharee/SamloaderKotlin) [SamFw](https://samfw.com/) 
- [Recommended Video Tutorials](https://youtu.be/vWX1fcrPeCA?si=kcBz6XiCUU4nlwQw)

#### Complete set of steps

> 1. Log out of your Samsung account and Google account and switch off your phone.
> 2. Install the above USB Driver and Odin3 on your computer.
> 2. Download the correct firmware and unzip it to get `BL`, `AP`, `CP`, `CSC`, `USERDATA` 5-piece set.
> 3. Open Odin3, select `BL`, `AP`, `CP`, `CSC` and import the files with corresponding names. It will take about three minutes to import `AP`, just be patient.
> 4. With the device switched off, press and hold the Volume + and Volume - keys at the same time and connect the device to the computer with the data cable, then release when the screen lights up. When the download icon appears, press the Volume + key again to enter the Downloading mode.
> 5. Check the `ID:COM` box on the top left corner of the Odin3, if it shows `0:COM+number`, it means the device is connected successfully, click `Start` to start flashing.
> 6. When Odin3 shows `PASS`, it means the flashing is completed and the device will reboot automatically.




## Application Installation

{% note info  %} 
This chapter suggests that we should avoid installing the latest version of the application.
{% endnote %} 

![国产应用](https://image.radishzz.cc/image/01-oneui/05en.webp)  

When setting up a new phone or after flashing a new Rom, I recommend against directly installing apps from the app store or using Smart Switch Mobile to restore apps, as this automatically installs the latest versions.

You might wonder: "Aren't the latest versions better?" Actually, no. Most apps become increasingly bloated with updates. They may add annoying ads or unnecessary new features that consume more CPU power and battery life, which is something we want to avoid.

Using older versions of apps is a smart approach, and it's best to avoid updating them unnecessarily. Older versions typically maintain core functionalities while using fewer system resources, helping prevent your device from becoming sluggish.

Besides older versions, consider open-source alternatives and cracked apps. Open-source alternatives usually offer cleaner interfaces and additional features, like NewPipe for example. Cracked apps can give you access to premium features at no cost, such as Spotify Premium.

### Download Sources

Here are some reliable sources for finding app packages. If you're willing to put in the effort, consider building your own collection of older app versions. This will also make future phone switches much easier.

Recommended Priority:  
**Older Versions > Open-Source Alternatives > Modified Versions**

> - [Apkmirror](https://www.apkmirror.com/)（Google Play Store Mirror）
> - [Droid-ify](https://f-droid.org/packages/com.looker.droidify/)（F-Droid）
> - [LiteApks](https://liteapks.com/)（Cracked Apps）
> - [My Collection](https://www.123pan.com/s/2xiAjv-fBzPh.html)（For Reference Only）




## System Settings

{% note info  %}
This guide covers non-essential features in your system settings and provides recommendations on which ones to enable or disable.
{% endnote %}

![System Settings](https://image.radishzz.cc/image/01-oneui/06.webp)  

You can locate these features by following our step-by-step guide or by using the search function in Settings. Keep any default settings that you find useful. Since feature names and locations may vary between system versions, please look for similar options on your device.

1. **Samsung Account**
> - Security and privacy - Personalization - Stop customizing all devices (Stop all personalization)
> - Security and privacy - Get news and special offers (Off)
> - Samsung Cloud - All options (Enable as needed)
> - Galaxy AI - Process data only on device (Enable as needed)
> - Find My Mobile - All options (Enable as needed)

2. **Connections**
> - Wi-Fi - Three dots menu - Intelligent Wi-Fi - Show network quality info (On) - Other features (All off)
> - Ultra-Wideband (UWB) (Off)
> - Data usage - Data saver (Off)
> - More connection settings - Nearby device scanning (Off)

Regarding Wi-Fi power saving mode, although it claims to reduce battery consumption, it also decreases data throughput. The device only sends and receives data during periodic wake-ups, which may affect real-time message reception in apps like WhatsApp and Messenger , so it's recommended to turn it off.

3. **Connected devices**
> - All features (Enable as needed)

4. **Notifications**
> - App notifications (Enable as needed)
> - - Advanced settings - Manage notification categories per app (on)

5. **Display**
> - Dark mode (Enable as needed)
> - Adaptive brightness (Enable as needed)
> - Screen resolution (QHD+ recommended)
> - Screen timeout - Keep screen on while viewing (Off)
> - Navigation bar - Circle to  Search (Enable as needed)
> - Accidental touch protection (off)
> - Touch sensitivity (Off)

6. **Battery**
> - Battery protection (Enable as needed)
> - Charging settings - All options (All on)  
>     _**Power saving ↓**_
> - Limit CPU speed to 70% (On)
> - Other options (All off)
> - Three dots menu - Adaptive power saving (Off)  
>     _****Background usage limits ↓**_
> - Three dots menu - Adaptive battery (Off)
> - Put unused apps to sleep (On)
> - First add all apps to Deep sleeping apps, then move frequently used apps to Sleeping apps, leave Never auto sleeping apps empty

Regarding battery settings, I've turned off Adaptive power saving/battery and actively manage background processes by assigning apps to sleeping or deep sleeping states. If you find this troublesome, you can keep the default options.

7. **Home screen**
> - Add media page to Home screen (Off)
> - Lock Home screen layout (On)
> - Swipe down for notification panel (On)
> - Search from Home (Off)
> - Rotate to landscape mode (Off)

8. **Lock screen and AOD**
> - Extended unlock - On-body detection (off)
> - Always On Display (Enable as needed)
> - Touch and hold to edit (Off)  
>     _**Secure lock settings ↓**_
> - Auto lock after screen turns off (5 seconds)
> - Lock instantly with Side button (On)
> - Auto factory reset, Lock network and security, Show lockdown option (Off)

9. **Security and privacy**
> - Auto blocker (All off)
> - More security settings - Install unknown apps (All denied, enable as needed)
> - More security settings - Galaxy system app updates (Off)
> - Permission manager (Check individually, disable unnecessary permissions)
> - Additional privacy controls - Alert When clipboard accessed (on)
> - More privacy settings - Send diagnostic data, Android personalization services, Usage and diagnostics (Off)  
>     _**App security ↓**_
> - App Protection - Three dots menu - App Protection Settings - Auto scan app daily, Auto scan when installing apps (All off)
> - Google Play Protect - Settings - Scan apps with Play Protect, Improve harmful app detection (Off)  
>     _**Biometrics ↓**_
> - Show unlock transition effect (Enable as needed)
> - Fingerprints - Delete all registered fingerprints, alternately register all fingers into one fingerprint entry, ensure complete coverage with each press and maintain pressure until prompted to lift
> - Fingerprints - Fingerprint always on (Enable as needed)

10. **Location**
> - Location services - All options (All off)

11. **Safety and emergency**
> - All options (All off)

12. **Google**
> - Find My Device (Off)
> - All services - Ads - Delete advertising ID - Ad privacy - All options (Off)

13. **Advanced features**
> - Smart suggestions (Off)
> - S Pen - More S Pen settings - S Pen unlock, Allow multiple S Pens, Keep S Pen connected (Off)
> - One-handed mode (Enable as needed)  
>     _**Motions and gestures ↓**_
> - Double tap to turn on screen, Double tap to turn off screen (On)
> - Palm swipe to capture (Off)
> - Other options (Enable as needed)

14. **Device care**
> - Memory - Excluded apps - Plus icon at top right (Add apps that need real-time messages)
> - Memory - RAM Plus (On for 8GB, Off for 12GB)
> - Performance profile (Light)
> - Auto optimization - Auto restart (Off)

Regarding RAM Plus, it uses storage space as additional RAM, which helps devices with low memory or high-load scenarios (like gaming). However, if the device has sufficient RAM, enabling RAM Plus provides no benefit and may slightly decrease device performance due to frequent data read/write. Therefore, it's recommended to enable for 8GB and disable for 12GB models.

15. **Apps**
> - Click the icon in the center on the right - Show system apps (On)
> - Search One UI Home and open - Battery (Unrestricted)
> - Search System UI and open - Battery (Unrestricted)

16. **Accessibility**
> - Vision enhancements - Reduce transparency and blur (Enable as needed)

17. **Software update**
> - Auto download over Wi-Fi (Off)

18. **Developer options**
> - _**How to open: About phone - Software information - Tap Build number repeatedly**_
> - Logger buffer sizes (Off)
> - System tracing - Trace debuggable apps (Off)
> - Wi-Fi scan throttling (On)
> - Suspend execution for cached apps (Keep device default, which equals On)
> - Predictive back animations (On)

### Other Settings

19. **Turn off automatic app updates**
> - _**Open Play Store - Profile icon - Settings - Network preferences**_
> - Auto-update apps (Off)
> - Auto-play videos (Off)  
>     _**Open Galaxy Store - Menu icon - Settings**_
> - Auto update apps (Never)
> - Auto play videos (Never)

20. **Limit background running of apps**
> - _**Only for infrequently used apps**_
> - Return to home screen - Long press app - Tap ⊙ in top right
> - Mobile data - Allow background data usage (Off)
> - Battery (Restricted)
> - Assign to sleeping or deep sleeping as needed

21. **Keep apps running in background**
> - _**Only for apps requiring real-time messages**_
> - Return to home screen - Long press app - Tap ⊙ in top right
> - Mobile data - Allow background data usage (On)
> - Battery (Unrestricted)
> - Open Settings - Search Excluded apps - Plus icon (Add apps)

22. **Minimize app notifications**
> - _**You can keeps app notifications while hiding their status bar icons**_
> - Open Settings - Search Manage notifications categories for each app (On)
> - Open notification panel - Long press notification - Settings - Notification categories - Tap highlighted option - Minimize notifications (On)

### Good Guardians Settings

The following apps are from Samsung's official Good Guardians plugin, available in the Galaxy Store. Note that these apps need to remain running in the background to be effective, please refer to step 22 for setup.

24. **Thermal Guardian (manages device temperature)**
> - Heat threshold (Set to minimum)
> - Additiional settings (Only check Limit CPU boost when heating)
> - Regarding heat threshold, from left to right the levels are 37, 38, 39, 40, 41 degrees. There are different opinions about setting it higher or lower. I recommend setting it lower to reduce device heating.

25. **Memory Guardian (manage device memory)**
> - Bottom options - Custom (Quick switching mode)

26. **Battery Guardian (manage device battery Health)**
> - App power saving (On) - Enter - Three dots menu - Sleep/Deep Sleep that you can't find in the settings is hidden here
> - Power saving during bedtime (On)
> - Set sleep time (00:00-23:59)
> - Screen Curtain is worth paying attention to

27. **App Booster (improve device Performance)**
> - Optimize after app/system updates
> - Recommended to run once per month




## Shizuku

{% note info  %}
This chapter mainly introduces Shizuku and related tool applications, along with some usage tips.
{% endnote %}

![Shizuku](https://image.radishzz.cc/image/01-oneui/07en.webp)

As the core focus of this chapter, let's first introduce Shizuku. It enables other applications to directly access system APIs without requiring root access. Let's take a practical example. Traditionally, if you wanted to disable Bixby Vision, you would need to root your device to gain full control. But Shizuku offers a more elegant solution. It obtains the necessary permissions through user authorization to manage system APIs. Once configured, other applications can work through Shizuku to access these system APIs, allowing them to perform advanced operations like disabling system apps, including Bixby Vision.

> - [Official Documentation](https://shizuku.rikka.app/)
> - [App Download Page](https://shizuku.rikka.app/download/)
> - [User Manual](https://shizuku.rikka.app/guide/setup/)

After installation, Shizuku requires user authorization before it can take control of system APIs. According to the user manual, there are three ways to start Shizuku. we typically recommend using the Wireless debugging method. Here are the specific steps:

### Start Shizuku

> 1. Make sure your device is connected to Wi-Fi and Developer options is enabled.
> 2. Open Shizuku and tap Pairing.
> 3. Go to Developer options.
> 4. Scroll down to find and enable USB debugging.
> 5. Find Wireless debugging and tap to enter its submenu.
> 6. Turn on Wireless debugging, then tap Pair device with pairing code.
> 7. Find Shizuku in the notification panel, enter the pairing code and send.
> 8. Once paired successfully, return to Shizuku's main page and tap Start.
> 9. Wait a moment, it will automatically return to the main page. When it shows Shizuku is running, the startup is successful.
> 10. Open Authorized 0 applications, grant the necessary permissions.

### Tool Applications

After successfully starting Shizuku, you can enjoy using various applications that support it. Here are some that I particularly recommend.

#### [Sam Helper](https://sam-helper.en.uptodown.com/android/download)

Sam Helper is a specialized toolkit designed specifically for Samsung devices. This comprehensive tool offers a wide range of features including Baronmeter Test, Shizuku Terminal, and System Settings. It also integrates all applications from Good Lock and Galaxy Labs, making system customization more accessible to users. Additionally, Sam Helper enables several useful functions:

##### **Check Battery Health**

![How to check battery health](https://image.radishzz.cc/image/01-oneui/08en.webp)

> 1. Tap the second icon in the top-right corner to access Shizuku Terminal
> 2. Enter and run the following command: `dumpsys battery | grep -i msave`
> 3. Check the output
> 5. Fifth line: Battery cycle count 487.56
> 6. Sixth line: Battery health 93%

##### **120Hz in Power Saving Mode**

By default, One UI doesn't allow 120Hz refresh rate in power saving mode. If you want to enjoy both power saving benefits and 120Hz smooth display experience, you can use the following method:

![120Hz in Power Saving Mode](https://image.radishzz.cc/image/01-oneui/09en.webp)

> 1. Enable Power saving mode
> 1. Go to Sam Helper - System Settings - Screen Refresh Rate (Seamless)
> 1. Open the Phone app and tap any number, for example `0`
> 1. Tap the button on the left to start a video call
> 1. Hang up after 3 seconds, and you're done
> 2. Some people will fail because there is no  video call button.

##### **Disable System Updates**

If you want to prevent system upgrades or disable  notifications to update, you can disable system updates completely.

![Disable System Updates](https://image.radishzz.cc/image/01-oneui/10en.webp)

> 1. Tap the second icon in the top-right corner to access Shizuku Terminal
> 2. Enter and execute these commands separately:
      `pm disable-user com.wssyncmldm`
      `pm disable-user com.sec.android.soagent`
> 3. To re-enable system updates, execute these commands:
      `pm enable com.wssyncmldm`
      `pm enable com.sec.android.soagent`

#### [Battery Guru](https://liteapks.com/battery-guru.html)

![Battery Guru](https://image.radishzz.cc/image/01-oneui/11en.webp)

Battery Guru is a comprehensive battery health management tool. It offers multiple features such as real-time current monitoring, battery capacity estimation, and app power consumption statistics to help users monitor and manage battery usage, ultimately extending battery life.

Users can identify abnormal power drain through real-time current monitoring and power consumption graphs. The app also allows modification of the device's Doze mode settings, helping devices enter deep Doze mode more quickly after screen-off to reduce standby power consumption.

##### Doze Mode

![Doze Mode](https://image.radishzz.cc/image/01-oneui/12en.webp)

> 1. On the app's home page, go to Settings (top-right) - Permission Manager - enable Allow post notifications and Modify system settings
> 2. Open Sam Helper's tShizuku Terminal and execute these commands one by one:
>     `pm grant com.paget96.batteryguru android.permission.BATTERY_STATS`
>     `pm grant com.paget96.batteryguru android.permission.PACKAGE_USAGE_STATS`
>     `pm grant com.paget96.batteryguru android.permission.WRITE_SECURE_SETTINGS`
>     `pm grant com.paget96.batteryguru android.permission.DUMP`
> 3. App homepage - Tools at the bottom - System battery saver - Configure
> 4. Doze optimization, Re-apply Doze parameters and Wait for unlock (on)

![System battery saver ](https://image.radishzz.cc/image/01-oneui/13en.webp)

> 5. Set up as shown
> 6. The application needs to be kept running in the background, please refer to step 21 of the System Settings.

#### [App Ops](https://appops.rikka.app/)

![App Ops](https://image.radishzz.cc/image/01-oneui/14en.webp)

App Ops is a powerful application behavior management tool. It modifies system appops settings to control app permissions and monitor sensitive permission usage. Compared to Android's built-in permission management, App Ops offers more extensive permission control options.

For example, you can use App Ops to disable permissions for problematic apps, such as motion sensors, clipboard access, calendar access, and device ID reading. This helps prevent personal privacy leaks, the features not available in the default  system setting.

#### [Scene](http://vtools.omarea.com/) 

![Scene](https://image.radishzz.cc/image/01-oneui/15en.webp)

Scene is a comprehensive toolkit that combines performance monitoring, charging statistics, app management, screen testing, and many other features in a clean, user-friendly interface. It offers three working modes: Basic Mode, ADB Mode, and ROOT Mode. After granting Shizuku permissions, you can activate ADB Mode and use these features for free (ROOT Mode requires payment).

##### dex2oat

A notable feature in Scene is forced dex2oat compilation. While this works similarly to App Booster mentioned earlier, Scene provides more compilation modes. Using the `everything` mode for compilation can maximize device performance and smoothness.

#### [SD Maid](https://liteapks.com/sd-maid-2-se-system-cleaner.html) 

![SD Maid](https://image.radishzz.cc/image/01-oneui/17en.webp)

A comprehensive system cleaning tool that helps users clear unnecessary files, cache, logs and free up storage space. After granting accessibility permissions, SD Maid can automatically clean cache for all apps which equivalent to manually clearing cache for each app through system settings.

#### [RootlessJamesDSP](https://play.google.com/store/apps/details?id=me.timschneeberger.rootlessjamesdsp) 

![RootlessJamesDSP](https://image.radishzz.cc/image/01-oneui/18en.webp)

An advanced audio processing tool that doesn't require root access. It offers extensive audio processing features including:

- Dynamic range compression/expansion
- Dynamic bass boost
- Multi-mode equalizer
- Soundfield expansion

Compared to Sound Assistant, it's far more capable. Even when compared to root-required ViPER4Android, JamesDSP proves to be more flexible and modular, with support for importing configurations to adjust parameters.

Users can leverage it to personalize device audio and optimize sound quality for both speakers and headphones. The main drawbacks are that it needs to run constantly in the background and doesn't support Spotify.

### [App Collection](https://github.com/ThePBone/awesome-shizuku)

The collection includes virtually all utility apps that support Shizuku functionality. You can explore and try them out.




## Lycan

{% note info  %}
This is an advanced guide that introduces the features and installation methods of Lycan, along with related technical knowledge. Not recommended for beginners.
{% endnote %}

![Lycan](https://image.radishzz.cc/image/01-oneui/19.webp)

Lycan is an application exclusively designed for Samsung devices. It's essentially a repackaged version of CCSWE App Manager 6.2.0, with only one Version 5.0.0 currently available. These two applications are identical (as shown in the image above, which is actually CCSWE). I've found a cracked version of [CCSWE App Manager](https://apkmb.com/ccswe-app-manager-samsung/) (the original version requires payment). Testing confirms that it can be installed and activated using Lycan's activation method, and the two apps can be installed over each other.

![Lycan installing over CCSWE App Manager](https://image.radishzz.cc/image/01-oneui/20.webp)

Both applications share identical functionality. According to CCSWE App Manager's Google Play description, it's designed for users who want to disable applications and packages to improve performance. This allows us to disable certain system applications that cannot be uninstalled. Additionally, Lycan can disable an app components to forcefully manage bloated, intrusive applications, effectively optimizing your device.

### App Components

![Four Basic App Components](https://image.radishzz.cc/image/01-oneui/21.webp)

Due to Android's highly open nature, many problematic applications register multiple `Services` and `Receivers` to maintain background presence. Sometimes, when you open just one app, it triggers a chain reaction that awakens multiple app services in the background, consuming CPU resources and battery power. Lycan helps address this issue by managing Android's four fundamental components:

- **Activity**
  An `Activity` represents the user interface window for interaction with the application. Each `Activity` corresponds to a screen where users can perform specific operations. When opening a new screen, the previous `Activity` is paused and pushed onto the back stack, allowing users to return to previously opened screens through the back navigation.

- **Service**
  `Services` perform long-running operations in the background without providing a user interface. For example, music playback continues in the background even when users switch to other `Activities`.

- **Broadcast Receiver**
  `Broadcast Receivers` listen for and respond to system-wide or application-specific broadcast messages. Applications can use them to react to external events (such as incoming calls or network connectivity changes) and trigger responses like launching `Activities` or `Services`.

- **Content Provider**
  `Content Providers` manage data storage and retrieval, enabling data sharing between applications without requiring storage permissions.

##### Effects of Component Disabling

- Disabling Activities: Disabling an `Activity` prevents the corresponding application screens from displaying or functioning properly. Only consider disabling `Activities` that are non-essential to core functionality or don't require user interaction, such as advertising pages or update screens.
- Disabling Services: `Services` are fundamental for background operations. Disabling them reduces RAM usage during app operation and minimizes CPU wake-ups when the app is in the background.
- Disabling Broadcast Receivers: By disabling unnecessary `Broadcast Receivers`, you can prevent unrelated applications from being awakened when system events occur.
- Disabling Content Providers: Disabling `Content Providers` prevents inter-application data sharing. This is generally not recommended as it may break essential functionality that relies on data exchange between apps.

##### Component Identification

Disabling unnecessary components can significantly improve app performance and reduce memory usage after app closure. However, to disable components effectively, we must first understand how to identify them. Components can be preliminarily assessed by analyzing their naming patterns, which helps determine whether disabling is appropriate. Here are some common keywords:

- Ad/Ads (advertise)
- Auth（Third-party authentication）
- Backup
- Camera
- Debug
- Dialog
- Download
- f（Location services）
- FloatWindow
- Gcm (Google Cloud Messaging)
- Install
- Media
- Message
- Notify
- Notification
- Pay
- Push
- Sdk (Connect different applications)
- Share
- Sync
- Update
- Upload
- Wallet
- Widget

##### LibChecker

For more precise component identification, you can use [LibChecker](https://play.google.com/store/apps/details?id=com.absinthe.libchecker&hl=en_US) as a supplementary tool. This application allows you to view and analyze an app's four components and native libraries, providing detailed descriptions for each.

![Libchecker](https://image.radishzz.cc/image/01-oneui/22.webp)

However, these optimizations come with risks. After disabling components, applications may experience issues such as white screens or crashes. You can troubleshoot by identifying and re-enabling the relevant components, or simply uninstall and reinstall the application to restore normal functionality.

### How to Disable Application

Disabling applications carries a higher risk compared to disabling components. Many users attempt to improve battery life by disabling system applications they believe are unnecessary. However, if a critical system process is disabled, the device may become stuck at the boot screen and fail to enter the system, leaving a factory reset as the only solution.

Therefore, it's recommended to reference verified disable lists and customize them according to your specific needs. You can refer to the [List of Samsung Bloatware Safe to Remove](https://www.minitool.com/news/list-of-samsung-bloatware-safe-to-remove.html) as a guide. I've also shared my personal [Disable List](https://1drv.ms/u/c/faeb19ea3240a386/EUBpSKSkfyBKqSxuuFXYjG4B9LoYWiga64fu8PA1dhss8w), which can be directly imported into Lycan. Remember to adjust the list based on your individual requirements.

{% folding white::Error List %}

> Apps: com.samsung.android.app.appsedge
> Split-screen multitasking not available.

> Emergency Launcher: com.sec.android.emergencylauncher
> Power saving mode not available.

> Sound Quality and Effects: com.sec.android.app.soundalive
> Global Dolby effects cannot be enabled .

> Samsung Core Services: com.samsung.android.scs
> Side panel rectangular screenshots unable to automatically detect and select images. Contact search unavailable, cannot select screenshots manually.

> Samsung Multi Connectivity: com.samsung.android.mcfserver
> Multi-connection unavailable, headphones cannot switch freely.

> Tethering: com.google.android.networkstack.tethering  
> App unresponsive when opened, Settings-Connections crashes.

> Samsung Device Health Manager Service: com.sec.android.sdhms
> Samsung Device Health crashes on launch.

> Settings Bixby: com.samsung.android.app.settings.bixby
> Samsung Cloud backup and restore unavailable.

> Factory Test Provider: com.samsung.android.app.providers.factory
> *#0*# code not working.

> SumeNNService: com.samsung.android.sume.nn.service 
> Photo Remaster Service: com.samsung.android.photoremasterservice
> Photo remastering in Gallery unavailable.

> DRParser Mode: com.sec.android.app.parser
> Gallery remastering and *#0*# code not working.

> Service Mode: com.sec.android.app.servicemodeapp
> *#06# code not working.

> Sec Media Storage: com.samsung.android.providers.media
> Screenshots blocked due to security policy.

> Network Manager: com.google.android.networkstack
> Mobile network unavailable.

> VPN Dialogs: com.android.vpndialogs
> VPN service unavailable.

> Media: com.google.android.providers.media.module
> File access denied.

> Key Chain: com.android.keychain
> Cannot access Security & Privacy - Other Security Settings.

> Input Devices: com.android.inputdevices
> Reduced screen sampling rate, touch response lag.

> WLAN Test: com.sec.android.app.wlantest
> WiFi auto-reconnect not working.

> Captive Portal Login: com.google.android.captiveportallogin
> Cannot log into WiFi networks.

> Global Post ProcMgr: com.samsung.android.globalpostprocmgr
> Camera preview abnormal after taking photos.

> Tx Pwr Admin: vendor.qti.data.txpwradmin
> Fast charging not working.

> Biometrics: com.samsung.android.biometrics.app.setting
> Cannot register fingerprints.

> Call Settings: com.samsung.android.app.telephonyui
> Cannot switch SIM cards and mobile data in status bar, mobile network options missing in settings.

> Ifaa Manager Application: org.ifaa.aidl.manager
> Alipay fingerprint payment unavailable.

> Sec Video Engine Service: com.sec.sve
> Camera cannot be activated during voice calls.

> CMH Provider: com.samsung.cmh
> App crashes when saving remastered photos.

> Badge Provider: com.sec.android.provider.badge
> SMS notification badges not showing.

> Samsung Keyboard: com.samsung.android.honeyboard
> Side screen clipboard unavailable.

> Call BG Provider: com.samsung.android.callbgprovider
> Call background missing.

> Intent Resolver: com.android.intentresolver
> Share menu crashes.

> Samsung Text-to-Speech Engine: com.samsung.SMT
> Handwriting input not working.

> Settings Suggestions: com.android.settings.intelligence
> Battery widget unavailable

> Always On Display: com.samsung.android.app.aodservice 
> Screen-off notifications unavailable.

> Container Service: com.samsung.android.container 
> Noise cancellation and ambient sound options missing in Bluetooth settings.

> Cell Broadcast Service: com.google.android.cellbroadcastservice
> Cannot send MMS, network error.

> Sticker Center: com.samsung.android.stickercenter
> Gallery editor crashes.

> Handwriting Service: com.samsung.android.sdk.handwriting
> SPen writing input not working.

> Samsung Text-to-Speech Engine: com.samsung.SMT
> Speech-to-text not working.

> Factory Camera: com.sec.factory.camera
> Filter Provider　com.samsung.android.provider.filterprovider
> Camera filter selection and addition abnormal.

> App Linker: com.sec.android.app.applinker
> App badges not working.

> TxPwrAdmin: vendor.qti.data.txpwradmin
> Fast charging not working.

> Soter Sskds Service: com.samsung.android.sskds
> Cannot enable fingerprint payment.

> Spritewallipaper: com.samsung.android.wallpaper.live
> Live wallpaper not working.

> Samsung Editing Assets: com.sec.android.app.ve.vebgm
> No sound in Gallery Stories.

> Companion Device Manager: com.android.companiondevicemanager
> Watch reconnection issues.

> Wallpaper Services: com.samsung.android.dynamicock
> Cannot display content directly on lock screen.

> Android Shared Library: com.google.android.ext.shared
> Smart Suggestions: com.samsung.android.smartsuggestions
> Cannot automatically detect and select URLs.

> Bluetooth Pairing Request: com.android.settings.bluetooth.BluetoothPairingRequest
> Headphone pairing popup not showing.

> Continuity Service: com.samsung.android.mcfds
> Multi-screen connectivity not working.

> Contacts Storage: com.samsung.android.providers.contacts
> Contacts functionality abnormal.

> Calendar Storage: com.android.providers.calendar
> Cannot create new events.

> Keychain: com.android.keychain
> Cannot access Security & Privacy - More Security Settings.

> Shell: com.android.shell
> Cannot open LSP.

> AR Emoji: com.samsung.android.aremoji
> Call background not working.

> Connectivity Overlay: com.samsung.android.ConnectivilyOverlay
> Connectivity Ux Overlay: com.samsung.android.ConnectivityUxOverlay
> Cannot connect to SPen.

> Galaxy Editing Service: ccm.samsung.android.globulpostprocmgr
> Camera app crashes.

> Configuration Update: com.samsung.android.cidmanager 
> DiagMon Agent: com.sec.android.diagmonagent
> Adreno Graphics Drivers: com.qualcomm.qti.gpudrivers.kalama.api33
> SumeNNService: com.samsung.android.sume.nn.service
> Abnormal battery drain.
{% endfolding %}

### Installation Guide

Lycan relies on the Samsung Knox SDK, but it cannot directly obtain Knox permissions. Since Splashtop-Add-on-Samsung shares the same package name as Lycan, the system treats them as the same application. The process works by first having Splashtop-Add-on-Samsung obtain and activate Knox permissions, then replacing it with Lycan, effectively transferring the activated Knox permissions.

#### [Required Tools](https://1drv.ms/f/c/faeb19ea3240a386/EsFDMom4zDxOl_B4deCiJ00BBrPno51SScWBg0dfJUdq6g)

1. Lycan APK
2. Splashtop-Add-On-Samsung APK
3. Sam Helper APK
4. Island APK

#### Complete Steps

{% note red warning %}
Not compatible with some One UI 6.1 and later system versions. Due to enhanced Knox security levels in the October 2024 system update, it's no longer possible to disable KLMS Agent version 1.2.14 via ADB. Therefore, Step 1 will fail, showing Failed to change state of package.
{% endnote %}

> - ***1. Enable Knox Permissions***
> - Run the following command in Sam Helper:
> `pm enable com.samsung.klmsagent`

> - ***2. Activate Knox Permissions***
> - Open Island and create a work profile.
> - Open the system's My Files app, tap on the Splashtop-Add-On-Samsung APK.
> - Choose **Work Profile** as the installation target, not Personal.
> - Select Island APK under the **Work Profile** and install.
> - Launch Splashtop-Add-On-Samsung and follow prompts to activate Knox permissions.

> - _**3. Disable Knox Permissions**_
> - Run the following command in Sam Helper:  
>     `pm disable-user com.samsung.klmsagent`

> - _**4. Transfer Knox Permissions**_
> - Locate and open Island Settings on the home screen.
> - Select Destroy permanently then choose DESTROY.
> - Install Lycan and follow prompts to activate Knox permissions.

> - _**5. Restore Knox Permissions**_
> - Repeat Step 1, installation complete.

#### Common Issues

1. Can it be installed on One UI 6.1?  
    Not guaranteed. This guide only works for One UI 1.0 to some One UI 6.1 versions.
2. How do I know if installation was successful?  
    All apps should be visible on the main page.
3. Apps not showing on main page?  
    Simply restart your device.
4. Activation failed with error 204/301?  
    Try a clean uninstall and restart the process from the beginning.
5. Splashtop-Add-on-Samsung activation failed with error 301?  
    Clear app data and grant all requested permissions.
6. Can't uninstall Splashtop-Add-on-Samsung?  
    Search for Device Admin Apps in Settings and revoke its authorization.
7. "Package conflicts with existing package" error?  
    Ensure both Lycan and Splashtop-Add-on-Samsung are completely uninstalled (see installation principles above).
8. Does it need to run in the background?  
    No, it doesn't need to
9. How to uninstall?  
    Click uninstall in the sidebar and choose "Don't keep data."
10. Will it trigger Knox fuse or compromise system security?  
    No, it won't have any such impacts.
11. Should I enable all apps before system updates?  
    Not necessary. Testing shows no issues even with major updates.

### Usage Guide

![Lycan Usage Guide](https://image.radishzz.cc/image/01-oneui/25.webp)

- **Disable Apps**: Home - Tap app icon - Tap `Disable` or `Enable` at bottom left (use top right to select all)
- **Disable Components**: Home - Tap app icon - Tap component icon - Tap `Disable` or `Enable` at bottom (use top right to select all)
- **Add to Favorites**: Home - Tap app icon - Tap heart icon at bottom right - Choose default folder or create new
- **Import/Export App Disable List**: Home - Sidebar - Favorites - Three dots menu - Import/Export
- **Import/Export Component Disable List**: Home - Sidebar - History - Three dots menu - Import/Export




## Adhell 3

{% note info %}  
This is an advanced chapter, which introduces the features and installation of the app Adhell 3.
{% endnote %}

![Adhell 3](https://image.radishzz.cc/image/01-oneui/27en.webp)

Adhell 3 is an application exclusively for Samsung devices. It was originally developed by Samsung developer FiendFyre but was later forced to be taken down. Subsequently, Adhell 2 was released but also ceased service after some time. It wasn't until 2017 that Adhell 3 emerged.

Its ad-blocking functionality relies on the Samsung Knox SDK, which is why it only works on Samsung devices. It acts as a front-end for the Samsung Knox SDK, writing your rule configurations (ad domains, firewall rules, whitelists) directly into Knox, eliminating the need for background processes. Adhell 3 offers four major functions.

### Four Functions

- **Domain rules**: Implements ad blocking through host file subscriptions and local domain rules, effectively filtering ads across system components, including app splash screens, content feeds, and modal advertisements.
- **Firewall rules**: Provides fine-grained control over cellular/WiFi permissions and custom rule creation (e.g., `com.android.chrome|*|53` blocks Chrome's DNS queries through port 53).
- **App disabler**: Manages system application states and permissions.
- **App Component**: Controls application components and permission frameworks.

Note: Due to potential stability issues, it's recommended to primarily utilize the Domain rules.

#### Common Issues

1. What is the scope of blocking?  
    System-wide ad blocking across all applications and services.
2. Battery consumption concerns?  
    Adhell itself doesn't consume battery as it doesn't maintain background processes. Any unusual battery drain typically occurs when blocked ads continuously attempt to reload in the background.
3. How does it differ from Adguard?  
    Adguard operates through a VPN tunnel, preventing simultaneous VPN usage. Adhell, utilizing Knox framework, doesn't occupy the VPN slot, allowing concurrent VPN connections.
4. Is Lycan still necessary with Adhell?  
    Yes. Adhell lacks batch operation capabilities, requiring manual configuration for each app. Lycan offers more efficient batch management features, making it the preferred choice for system modifications.
5. Recommended host sources?  
       [Ad hosts](https://github.com/otobtc/ADhosts) [AdBlock DNS Filters](https://github.com/217heidai/adblockfilters)
6. Why do some ads still appear?  
    Complete ad elimination isn't guaranteed. Blocking effectiveness depends on your subscribed host sources, which can't possibly contain all ad domains in existence. Some ads inevitably slip through.
7. Should I add as many rules as possible?  
    No. More rules increase rule processing time and network latency. Excessive rules can even cause device boot loops in some cases. We recommend maintaining a balanced, optimized ruleset.

### Installation Guide

Adhell 3 and Lycan share the same Knox SDK implementation foundation. The installation process follows the previously outlined Knox-based deployment methodology.

#### [Required Tools](https://1drv.ms/f/c/faeb19ea3240a386/EsFDMom4zDxOl_B4deCiJ00BBrPno51SScWBg0dfJUdq6g)

1. Adhell 3 APK
2. NotifyRDS-Add-On-Samsung APK
3. Sam Helper APK
4. island APK

#### Complete Steps

{% note red warning %}
Not compatible with some One UI 6.1 and later system versions. Due to enhanced Knox security levels in the October 2024 system update, it's no longer possible to disable KLMS Agent version 1.2.14 via ADB. Therefore, Step 1 will fail, showing Failed to change state of package.
{% endnote %}

> - ***1. Enable Knox Permissions***
> - Run the following command in Sam Helper:
> `pm enable com.samsung.klmsagent`

> - ***2. Activate Knox Permissions***
> - Open Island and create a work profile.
> - Open the system's My Files app, tap on the NotifyRDS-Add-On-Samsung APK.
> - Choose **Work Profile** as the installation target, not Personal.
> - Select Island APK under the **Work Profile** and install.
> - Launch NotifyRDS-Add-On-Samsung and follow prompts to activate Knox permissions.

> - _**3. Disable Knox Permissions**_
> - Run the following command in Sam Helper:  
>     `pm disable-user com.samsung.klmsagent`

> - _**4. Transfer Knox Permissions**_
> - Locate and open Island Settings on the home screen.
> - Select Destroy permanently then choose DESTROY.
> - Install Lycan and follow prompts to activate Knox permissions.

> - _**5. Restore Knox Permissions**_
> - Repeat Step 1, installation complete.

After granting permissions as prompted, entering the main page indicates successful activation. If you see a popup showing License Activation, it means activation has failed. You'll need to start the process again from the beginning.

#### Important Notes

1. It is not recommended to enable firewall rules as this may prevent calls and SMS functionality, limiting the device to data-only internet access.
2. Running Adhell and Clash simultaneously will cause network disconnection. [Clash Meta](https://github.com/MetaCubeX/ClashMetaForAndroid) is recommended as an alternative solution.
3. When domain rules are enabled, the device's hotspot functionality will not work.
4. Some domains, when blocked, will repeatedly attempt connections. It's recommended to add such domains to the Whitelist in the Domains page to prevent abnormal battery drain.
5. Avoid using App Whitelisting, as this will exponentially increase domain rule loading times. Each whitelisted app doubles the loading duration.

### DNS AdBlock

Adhell 3 has not been maintained since 2017 and has developed bugs following the One UI 6.0 upgrade, leading me to discontinue its use. However, there are other effective methods for ad blocking. 

![Adguard DNS](https://image.radishzz.cc/image/01-oneui/28en.webp)

Register with [Adguard DNS](https://adguard-dns.io/) and connect a new device by setting up the private DNS provider hostname as shown in the image. To enhance blocking effectiveness, you can add these blocking lists in AdGuard DNS server settings:

1. `AWAvenue Ads Rule`
2. `1Hosts (Lite)`
3. `HaGeZi's Normal Blocklist`
4. `OISD Blocklist Small`
5. `Steven Black's List`




## Conclusion

![Reddit Post](https://image.radishzz.cc/image/01-oneui/31en.webp) 

This guide was originally written in Chinese, and I hadn't planned on creating an English version. However, when I recently discovered that someone had shared my article on Reddit and it received positive feedback, I realized this guide could potentially help more people beyond just those in China. That's what motivated me to translate it into English, carefully reviewing and refining the content to create this complete English version of the One UI optimization guide. I really hope it can be helpful to all of you.

While some Reddit users criticized my approach, suggesting I was turning the phone into a Nokia 3310, I find that quite amusing. Everything I've recommended is about improving battery life and performance without sacrificing user experience. Notice how I never suggested switching to 60Hz or HD+. I genuinely enjoy tweaking and optimizing phones, and I'm simply sharing my experiences with those who might find it useful. If you disagree with my approach, that's totally fine, but please don't mock it.

![One UI](https://image.radishzz.cc/image/01-oneui/01.webp) 

About the main point of this guide: improving your device's battery life and performance doesn't actually require all these fancy tweaks. If you're a tech enthusiast who enjoys optimizing devices, by all means, go through all the steps. But for most people, day-to-day usability is what matters most, and honestly, many of these optimizations go beyond what's necessary. You can usually achieve great battery life and smooth performance just by following the App Installation and System Settings chapters. There's no need to get too caught up in disabling features and such. The benefits become marginal at that point.

Finally, let me rank the six chapters by their effectiveness in improving fluency and battery life:  
**System Settings > App Installation > The Wiping and Flashing > Shizuku ≈ Lycan > Adhell 3**

{% note info  %}
If you like this guide, feel free to buy me a coffee. I'll be happy to answer any questions for you.
{% endnote %}

{% folding gray::Donate %}
{% tabs First unique name %}
<!-- tab PayPal-->
![qrcode-paypal](https://image.radishzz.cc/image/qrcode-paypal.webp)
<!-- endtab -->
<!-- tab Alipay-->
![qrcode-alipay](https://image.radishzz.cc/image/qrcode-alipay.webp)
<!-- endtab -->
<!-- tab Wechat-->
![qrcode-wechat](https://image.radishzz.cc/image/qrcode-wechat.webp)
<!-- endtab -->
{% endtabs %}
{% endfolding %}
