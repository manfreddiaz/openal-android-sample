# OpenAL for Android Sample
At this point, it is hard to find some working examples of 3D audio/spatialization on the Android platform that could be easily prototyped. Hence, I shared this sam application showing 3D audio rendering, using the bit old [openAL4android](http://pielot.org/2011/11/openal4android-2/) library.

Hope it helps!
  

## Ready For

* Android SDK v26.0.0
* Android Studio v2.3.3
* Gradle Plugin v2.3.3
* Tested On: 
    * *Android 7.0 Nougat*
    * *Android 6.0 Marshmallow*

## Remarks

* **IMPORTANT**: to make a compatible *.wav* file, the *RIFF WAVE* headers should be present on the file.
  Common audio/video conversion libraries tried (sox, ffmpeg) does not trivially generate the proper *.wav* file headers. Only [Audacity](http://www.audacityteam.org/download/windows/) for Windows 10 did the trick.  
* *libopenal.so* and *libopenalwrapper.so* are compiled for 32-bits platforms (ARMEABI v7a).
* *gradle.properties* includes the **android.useDeprecatedNdk=true** option which may not be available in future versions of Android Gradle plugin.