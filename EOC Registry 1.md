```dart
@override
void initState() {
  super.initState();

  // Enable wakelock
  Wakelock.enable();

  // Check if wakelock is enabled
  Wakelock.enabled.then((isEnabled) {
    debugPrint("Wakelock is ${isEnabled ? 'enabled' : 'disabled'}");
  });
}
```

## Wake lock Plus 
 ```
 Building with plugins requires symlink support.

Please enable Developer Mode in your system settings. Run
  start ms-settings:developers
to open settings.
```

so i need to win+ r  and 
ms-settings:developers 
then turn on developer mode 
```

dependencies:  
  
  win32: ^5.5.3  
  flutter:  
    sdk: flutter  
  wakelock_plus: ^1.1.4  # Use the latest version  
  shared_preferences: ^2.1.1  
  
  nfc_manager: ^3.5.0  
  
  # The following adds the Cupertino Icons font to your application.  
  # Use with the CupertinoIcons class for iOS style icons.  cupertino_icons: ^1.0.8  
  
dev_dependencies:  
  flutter_test:  
    sdk: flutter  
  
# Add this section  
dependency_overrides:  
  win32: ^5.5.3
```

## Make Font smaller 

#### Field box change 

#### Reload not performed Analysis issuse find


## > NDK from ndk.dir at C:\android-ndk-r27c-windows\android-ndk-r27c had version [27.2.12479018]

Open your android/build.gradle.kts file and find the line that specifies the NDK version (around line 16). Change it to match the version you have installed:

kotlin

android {
    // Change this line
    ndkVersion = "27.2.12479018"  // Match the version you have installed
}


## how not to Recommandation IME Responsive 
![[EOC Always on Function.png|375]]
child: Scaffold(
resizeToAvoidBottomInset: false, 

####  how now to show overflow ? 
![[EOC Always on Function-1.png|300]]
debugPaintSizeEnabled = false;
#✍️ 