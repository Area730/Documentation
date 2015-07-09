####IOS Build
This section explains how to create IOS build from unity.  
  
##Exporting from unity  
1. Go to Build Settings -> Player Settings -> Other Settings  
2. In **Configuration** section  
	1. Choose **Scripting Backend** to **IL2CPP**  
	2. Choose **Architecture** to **Universal**  
3. Press Build  


##XCode build  
  
If AdMob is used for mediation:  
	1. Go to **General -> Linked frameworks and Libraries** and add [GoogleMobileAds.framework](https://developers.google.com/mobile-ads-sdk/download#downloadios)   
	2. Go to **Build settings** and set **Enable Modules(C and Objective C)** to **true**  

May be also needed (add these step by step if needed):  
	3. Go to *Linking* and add  **-Objc** flag to **Other Linker Flags**  
	4. Set **Allow non-modular Includes in Framework Modules** to **YES**  
  
In *Architectures* set **Build Active Architecture Only** to **NO**  
  
If **GoogleAdsFramework** is added but you have NotFoundException, remove it and add again  
  
--------------

The following frameworks may also be required  
	* CoreTelephony  
	* iAd  
	* EventKit  
	* EventKitui  
	* Adsupport  
	* AVFoundaion  
	* AudioToolbox  
	* CoreGraphics  
	* CoreMedia  
	* MessageUi  
	* StoreKit  
	* SystemConfiguration  
