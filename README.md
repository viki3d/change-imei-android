# Change-IMEI-Android

## What is Change-IMEI-Android ?

<p align="justify">
Change-IMEI-Android is an Android App, which can help you to change(*spoof) the IMEI of your phone.
</p>

<p align="justify">
This app is free. No advertisements. Double-SIM phones support.
</p>


<p align="justify">
Your IMEI is not actually changed. The IMEI is physically stored in phone as a file. This file is not modified.
Changing of IMEI is done in the following way: The Android OS is patched, so when it read the IMEI from the file - 
the result is replaced with the user's predefined value. This happens in the memory (runtime). The final result
is: Android OS reads the real IMEI but reports the predefined value. This is called <i>IMEI spoofing</i>.
</p>

<p align="justify">
<i>Change-IMEI-Android</i> is not a standalone app. It is just a module for a framework called EdXposed.
This framework is starting before the Adroid OS, loads it's modules, so then can work.
</p>

<b>Prerequisites</b>
<p align="justify">
To be able to run this app - you need to complete this steps:
	<ol>
		<li>Unlock your phone's bootloader</li>
		<li>Root your phone</li>
		<li>Install <a href='https://github.com/topjohnwu/Magisk/releases' target="_blank">Magisk</a> (flash from Recovery /like TWRP/)</li>
		<li>Install <a href='https://github.com/topjohnwu/Magisk/releases' target="_blank">Magisk Manager</a> (Android app, managing Magisk) more info 
			<a href='https://magiskmanager.com' target="_blank">here</a></li>
		<li>Install Riru (from Magisk as Magisk module). This injects into Android Zygote process. Required by all Riru Modules (EdXposed)</li>
		<li>Install Riru-EdXposed framework (from Magisk as Magisk module). This will install EdXposed framework + EdXposed Android Manager App</li>
		<li>Install Change-IMEI-Android. Download <a href='' target="_blank">here</a></li>
	</ol>
</p>

<b>How to run/use the app:</b>
<p align="justify">
	<ol>
		<li>Ensure all prerequisites are met</li>
		<li>Run the EdXposed App and activate the module <i>Change-IMEI-Android</i></li>
		<li>Open the App Change-IMEI-Android and check what you want to spoof: IMEI-1, IMEI-2, or else; Set wanted values</li>
		<li>Restart phone</li>
		<li>Check if everything is ok by opening Settings; If something is wrong - open EdXposed App and see Logs.</li>
	</ol>

</p>

<b>Supported Android versions</b>
<p align="justify">
This app has been made especially for Lineage OS 17 (with Android 10). 
Older Android versions are not supported since another (older) API is used to read the data (IMEIs, etc).
To cover these old APIs more code is needed (and I have not enought time to support them now).
	<ul>
		<li>Android 11 - ?</li>
		<li>Android 10 - yes</li>
		<li>Android  9 - no </li>
		<li>Android  8 - no </li>
		<li>Android  7 - no (you need Xposed, instead EdXposed)</li>
		<li>Android  6 - no (you need Xposed, instead EdXposed)</li>
		<li>Android  5 - no (you need Xposed, instead EdXposed)</li>
		<li>Android  4 - no (you need Xposed, instead EdXposed)</li>
	</ul>
</p>

<b>Tested configuraions</b>
<p align="justify">
- Magisk v21.4 (21400)
- [Magisk module] Riru v25.4.4.r426
- [Magisk module] Riru-EdXposed v0.5.2.2_4683
</p>

## Changing IMEI

<b>Remarks about changing IMEI</b>
<p align="justify">
In some countries (like UK) changing the IMEI is considered illegal. But tracking people without their explicit knowledge and acceptance is also illegal. This app doesn't actually change your IMEI (but spoof it in runtime). However, if changing IMEI is not allowed in your country - you'd better not use this app or use it on your own risk. 
</p>

<p align="justify">
Changing IMEI is considered bad in some countries for a purpose to avoid stolen phones to be re-selled. 
However, in some EU countries you will not get any help from authorities or carrier to get your phone back (even you provide them with the original invoice, guarantee and phone box). This means they do not
use IMEI tracking to help you re-gain your phone but just <i>to track you</i>. 
Information about IMEI tracking abusement is available in Internet: tracking women in Saudi Arabia, tracking political oppositionists in Russia, etc.
</p>

<p align="justify">
<b>Invalid IMEI</b><br/>
Your carrier can detect if your IMEI is invalid or has been banned. In these cases - you will not be able to access the carrier's network and can not make phone calls.
There are many IMEI generators in Internet, where you can generate valid IMEI numbers.
</p>

<p align="justify">
<b>Benefits of changing IMEI</b><br/>
	<ul>
		<li>
			<b>Hide your phone model from your carrier.</b> 
			Your IMEI encodes your phone model, so your carrier obtain this information without your agreement and can profile you without your consent by detecting your
			social status (<i>"this person is using cheap/expensive phone - Brand/Model/Color"</i>).
		</li>
		<li>
			<b>Use another SIM card without connecting it to you.</b> 
			Carrier tracks you by maintaining link: Phone/IMEI<-->Sim/PhoneNumber. If you use somebody's else SIM card - this is detected by the carrier.
			This could be very dangerous in China, where such action can damage your 'personal score' if you use SIM card of person with lower score.
			Or even they detect you are using another SIM card.
		</li>
		<li>
			<b>Prevent attacks agains yours personality.</b> 
			Before someone being attacked - a lot of information is being collected about this person. This includes detecting: his/her home location, habits, devices, friends etc.
			Preventing personal data leak is preventing attacks against your personality. GDPR protects european citizens from such illegal data collection.
			However, in many other countries people are tracked in pretext of their good but this information is actually used (only) against them.
		</li>
		<li>
			<b>Broken IMEI.</b>
			Many people flash their phones with the so-called custom ROMs. Without knowing what they are doing - they flash by mistake their /efs partition.
			Without having backup of this partition they can not restore their IMEI. Phone provides a defalt IMEI which is most often banned from carriers.
			In result their device become useless. This app is second chance to use such phone.
		</li>
	</ul>
</p>

<p align="justify">
<b>When changing IMEI is useless</b><br/>
Changing IMEI can not hide you. If you are using a phone (connected to carrier/network) you location is known within few meters. Your locations (daily route map) is stored at carrier's db forever. You are being tracked by: proximity to other phones, IP address, WiFi network, browser's unique id, OS unique id, your accounts etc. So changing your IMEI can achieve only very small piece of privacy and is very naive to consider that spoofing your IMEI can hide you.
</p>

## Xposed, EdXposed, LSPosed
<p align="justify">
	What are Xposed, EdXposed, LSPosed? Initially a Xposed framework was released but for the new Android versions
	another versions of this framework appeared. Briefly:
	<ul>
		<li>Xposed Framework (Dalvik): Android 4.2, 4.3, 4.4, 4.4W </li>
		<li>Xposed: 5.0 up to Android 8.1</li>
		<li>Riru - EdXposed: Android 8.0, 8.1, 9, 10, 11 or above</li>
		<li>Riru - LSPosed: Android 8.0, 8.1, 9, 10, 11 or above</li>
	</ul>
	
</p>

## Update
The module is now (2023) working with current version of LSPosed, which supports Android versions from 8 to lastest (until now) - 14.  
  
Unfortunately the LSPosed framework is so badly designed, so that works only with pre-set apps. This means if you are hiding some of your phone properties like
deviceId, ImeiSlotId, Imei, etc and install a new app - it will see their real values. This fact is critical that make the framework purpose obsolette. Now I should
find some time for 1] patch LSPosed (and make a patch script so the new versions to be automatically patched) so it became reliable 2] Update this module (some more things are added to LSPosed)
3] I'm thinking to release the code but not any time to clean it for the repo; this will be my lowest priority.


## Download
[![change-imei-android](change-imei-android.png "Watch on YouTube")](https://youtu.be/ivDSru1uWS4).  
  
&bull; [Download here](https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/viki3d/change-imei-android/blob/main/Change-IMEI-android.apk)  

