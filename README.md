ScreenFilter
============

Attempt to mimic the screenfilter by https://play.google.com/store/apps/details?id=com.haxor&amp;hl=en.
Because I think it's the most essential apps with simple user interaction. 
Thus is good as a learning project.

The design/idea used in this project is from reverse engineering the above apps. 

Some behaviors of the ScreenFilter apps:
- When started, it doesn't appear on the "Recent App" list. 
  > This is done by declaring the acitivty with:  
      android:excludeFromRecents="true"
  
- Show 1 process and 1 service 

- It continue to function even in lock screen

- Should not be killed
  > This is done by calling startForeground
  > Example of startForeground: https://github.com/commonsguy/cw-android/tree/master/Notifications/FakePlayer
  
TODO:
Critical:
- getNotification crash need to be fixed.

Enhancement:
- Add color selection screen
- Add brightness adjustment control

