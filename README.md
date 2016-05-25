JUCI WebGUI Mobile SDK 
---

	Last update: 24 May 2016
	Author: Martin Schröder <mkschreder.uk@gmail.com>

When I first created JUCI project (http://github.com/mkschreder/juci), mobile
support was there from the start - but the default mobile support was only
concerned about making the JUCI interface adjust itself to the narrow screen of
a mobile browser (basically what commonly is called "responsive design").
Creating native mobile applications was not supported by original code. 

Since JUCI version 2.16.05, you can build a juci js library which you can then
embed into applications such as this example application to allow you to use
the same code to access remote objects as is used in the main web application.
This approach is very powerful because it allows maximal code reuse while still
allowing you to use native mobile phone functions through the Apache cordova
bridge (phonegap). 

This project will show you how to create native mobile applications that can
connect to a router running JUCI API and allow you to configure that device or
other devices that are connected to it using a native mobile app. 

JUCI Project and all projects that it consists of are given to you free of
charge under the terms of GNU General Public License v3. You are free to use
JUCI or any of the surrounding projects in any commercial or non-commercial
application. You are free to modify the code and base your own software on it. 

Cordova and it's libraries are distributed to you under the Apache license. 

Instructions
---

In order to build this project you will need phonegap. So install it now. 

	sudo npm install -g phonegap

Next, if you are going to be building for android, download the latest version of Android SDK. 

Building the android application is then done like this: 
	
	phonegap build android

To run on device do this: 
	
	phonegap run android --device

To run in local server which you can access with your browser do this: 

	phonegap serve --browser
