# Awesome Full Body Tracking
Here is a _(hopefully maintained)_ list of open-source projects for VR full-body tracking.

### KinectToVR
Provides advanced features for Kinect body tracking like simulated tracker flip, automatic calibration to your VR headset, stable foot rotation for the original Xbox 360 Kinect model and more.

**Website: https://k2vr.tech**  
**Source: https://github.com/kinecttovr**  
**Demonstration: https://imgur.com/ThSjFHD**

### SDraw's driver (`KinectV1` and `KinectV2`)
Focusing on simplicity, this driver doesn't feature some of the more useful features of KinectToVR, but it has the huge added bonus of allowing you to spawn as many virtual trackers as there are tracked joints on the Kinect.

**Source/Website:  
https://github.com/SDraw/driver_kinectV1/ (Kinect 360)  
https://github.com/SDraw/driver_kinectV2/ (Kinect One)**

### SlimeVR
Use any number of Slime trackers (open source hardware) or OwOTrack-compatible phones (see below) to do body tracking using only IMUs. With 5 devices, you can do lower body tracking like is supported in most games. with 7 devices, you can add foot rotation. Using less trackers it's also possible to add elbow tracking or knee tracking to existing tracked setups.

**Official Website: https://www.crowdsupply.com/slimevr/slimevr-full-body-tracker**  
**Source: https://github.com/SlimeVR/**  

### OwOTrack
Using an Android or iOS device (the iOS version isn't opensource because of Apple's App Store publishing limitations) you can emulate a waist tracker that's very close in functionality to a real Vive tracker. The app also includes a feature for hip-guided locomotion similar to how DecaMove works.

Binaries are only distributed through MEGA on the Discord server.

**Website: https://discord.gg/ttDkJqKDXX**  
**Source:  
https://github.com/abb128/owo-track-driver (SteamVR driver)  
https://github.com/abb128/owo-track-overlay (Overlay built with Godot, has main project info)  
https://github.com/abb128/owoTrackVRSyncMobile (Android app)**

### AprilTag
Print or draw some QR-code looking markers (QR Code is only one type of what is called a 2D barcode) and tape them to cardboard then use a webcam or your phone camera to track them. Only one camera is supported but trackers can be made with 4 sides to be visible all around, and you can replace the waist tracker with OwOTrack for a very solid experience.

**Source/Website: https://github.com/ju1ce/April-Tag-VR-FullBody-Tracker**

### AirPose
Use a webcam and Google's MediaPipe machine learning body tracking model to create trackers. Be warned that this uses a lot of CPU and most computers won't be able to run it while keeping VR at a reasonable framerate.

**Source/Website: https://github.com/justinliang1020/AirPose**

### ALVR (tracker proxy)
It's possible to use an Oculus Quest headset and controllers as trackers, by wearing the headset on your waist and putting the controllers on your feet, there is a feature of ALVR that allows turning the devices created by the driver to be nothing more than trackers instead of full-blown VR devices, so you can use another headset alongside. (If you have a Quest/Quest 2 and haven't checked out ALVR for it's VR streaming, you should, it's amazing.)

**Website: https://alvr-org.github.io**  
**Source: https://github.com/alvr-org**

### OculusTouchLink
This started out as a SteamVR driver for using the Oculus Rift's controllers with different headsets, but was repurposed by me to spawn Vive trackers, then [AeroScripts](https://github.com/aeroscripts) modified it further to support the "tracked object" third controller that is normally used by LIV. There are no public binaries of either my or Aero's forks of the driver, but you can throw me a ping on Discord or Twitter if you want it.

**Source:  
https://github.com/mm0zct/Oculus_Touch_Steam_Link (Original repo)  
https://github.com/TripingPC/Oculus_Touch_Steam_Link (My fork, spawns 2 trackers and reports it's tracking space as `lighthouse`)  
https://github.com/AeroScripts/Oculus_Touch_Steam_Link (AeroScript's fork, spawns 3 trackers and reports it's tracking space as `oculus` (I have a separate binary that reports as `lighthouse`))**

### k4a_openvr
Full-body tracking with a Kinect Azure DK. Requires a very strong GPU to use alongside VR games. There are no distributed binaries because the terms of the K4ABT SDK prohibit it. And the app must be built with it.

**Source: https://github.com/conatsera/K4A_OpenVR**