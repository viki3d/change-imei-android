# Change-IMEI-Android

## What is Change-IMEI-Android ?

<p>
Change-IMEI-Android is an Android App, which can help you to change(*spoof) the IMEI of your phone.
</p>

<p>
This app is free. No advertisements. Double-SIM phones support.
</p>


<p>
Your IMEI is not actually changed. The IMEI is physically stored in phone as a file. This file is not modified.
Changing of IMEI is done in the following way: The Android OS is patched, so when it read the IMEI from the file - 
the result is replaced with the user's predefined value. This happens in the memory (runtime). The final result
is: Android OS reads the real IMEI but reports the predefined value. This is called <i>IMEI spoofing</i>.
</p>

<p>
<i>Change-IMEI-Android</i> is not a standalone app. It is just a module for a framework called EdXposed.
This framework is starting before the Adroid OS, loads it's modules, so then can work.
</p>

<b>Prerequisites</b>
<p>
To be able to run this app - you need to complete this steps:
	<ol>
		<li>Unlock your phone's bootloader</li>
		<li>Root your phone</li>
		<li>Install [Magisk](https://github.com/topjohnwu/Magisk/releases) (flash from Recovery /like TWRP/)</li>
		<li>Install [Magisk Manager] (https://github.com/topjohnwu/Magisk/releases) (Android app, managing Magisk) more info [here](https://magiskmanager.com/)</li>
		<li>Install EdXposed framework (from Magisk as Magisk module). This will install EdXposed framework + EdXposed App</li>
		<li>Install Change-IMEI-Android (as EdXposed module) download [here]()</li>
	</ol>
</p>

<p>
How to run/use the app:
	<ol>
		<li>Ensure all prerequisites are met</li>
		<li>Run the EdXposed App and activate the module <i>Change-IMEI-Android</i></li>
		<li>Open the App Change-IMEI-Android and check what you want to spoof: IMEI-1, IMEI-2, or else; Set wanted values</li>
		<li>Restart phone</li>
		<li>Check if everything is ok by opening Settings; If something is wrong - open EdXposed App and see Logs.</li>
	</ol>

</p>

<b>Supported Android versions</b>
<p>
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
	</ul>
</p>


