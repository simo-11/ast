# ast
andoid studio tutorial
# Installation
Using android-studio-2024.1.1.12-windows.exe
Android Studio Koala | 2024.1.1 Patch 1
Build #AI-241.18034.62.2411.12071903, built on July 11, 2024
Runtime version: 17.0.11+0--11852314 amd64
VM: OpenJDK 64-Bit Server VM by JetBrains s.r.o.
Windows 11.0
GC: G1 Young Generation, G1 Old Generation
Memory: 2048M
Cores: 20
Registry:
  ide.experimental.ui=true


## issues

### Running Intel® HAXM installer
Intel HAXM installation failed!
For more details, please check the installation log: C:\Users\simon\AppData\Local\Temp\haxm_install-20240714_1817.log
Intel® HAXM installation failed. To install Intel® HAXM follow the instructions found at: https://github.com/intel/haxm/wiki/Installation-Instructions-on-Windows

### Unsupported Gradle JVM.
```
> &"C:\Program Files\Android\Android Studio\jbr\bin\java.exe" -version
openjdk version "17.0.11" 2024-04-16
OpenJDK Runtime Environment (build 17.0.11+0--11852314)
OpenJDK 64-Bit Server VM (build 17.0.11+0--11852314, mixed mode)
Your build is currently configured to use Java 17.0.11 and Gradle 6.7.1.
```

Possible solutions:
 - Upgrade to Gradle 8.5 and re-sync - this was done but build still got error
```
   org.gradle.internal.event.ListenerNotificationException: Failed to notify dependency resolution listener.
```
 - Upgrade to Gradle 7.2 and re-sync

#### Continue with gradle issue
Reproduce by File - Sync Project with Gradle files
https://docs.gradle.org/8.5/userguide/command_line_interface.html#sec:command_line_warnings

# Notes on examples

## Wifi Rtt Scan
https://github.com/android/connectivity-samples/tree/main/WifiRttScan -> C:\Users\simon\AndroidStudioProjects\WifiRttScan

### Defender 
```
> Add-MpPreference -ExclusionPath 'C:\Users\simon\AppData\Local\Programs\Spyder','C:\Program Files\MATLAB','C:\Users\simon\.gradle', 'C:\Users\simon\AndroidStudioProjects', 'C:\Users\simon\AppData\Local\Android\Sdk', 'C:\Users\simon\AppData\Local\Google\AndroidStudio2024.1'
```

