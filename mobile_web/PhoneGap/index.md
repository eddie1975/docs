---
title: 'PhoneGap'
notes:
  - "This is a vendor specific technology that should not be included in an industry standard documentation resource.\n Eliezerb:\nShould be deleted or moved to tutorials section"
readiness: 'Not Ready'
summary: 'PhoneGap is an application framework that enables you to build natively installed applications using HTML and JavaScript.  The easiest way to think of PhoneGap is a web view container that is 100% width and 100% height, with a JavaScript programming interface that allows you to access operating system features.'
tags:
  - Concept_Pages
  - Developer_Tools
uri: 'mobile web/PhoneGap'

---
## Summary

PhoneGap is an application framework that enables you to build natively installed applications using HTML and JavaScript. The easiest way to think of PhoneGap is a web view container that is 100% width and 100% height, with a JavaScript programming interface that allows you to access operating system features.

## Introduction

PhoneGap is a distribution of Apache Cordova, a top level open source project of the Apache Software Foundation driven by a vibrant community. The purpose of this page is to share some basic information about PhoneGap like how it works, how to extend it, how it's born, etc.

## How it works

A PhoneGap application is a “native-wrapped” web application through the web browser native widget most of the mobile development SDKs provide as a part of their UI framework (this widget is known as “web view”, following the links to get more information about the web view in iOS <http://developer.apple.com/library/ios/#documentation/uikit/reference/UIWebView_Class/Reference/Reference.html> and the one in Android <http://developer.android.com/reference/android/webkit/WebView.html>).

In purely native applications, web view controls are used to display HTML content either from a remote server, or local HTML packaged along with the native application in some way. The native “wrapper” application generated by PhoneGap loads the end developer’s HTML pages into one of these web view controls, and displays the resulting HTML as the UI when the application is launched. One of the benefits of this approach is that the app functions offline and that there is lower latency for retrieving assets, and available bandwidth is less of a concern. The main benefit is that you won't need to upload your files anywhere to get the full testing experience, it’s enough to open index.html directly from your file system to get the optimal PhoneGap development workflow or even better to open the index.html file with Ripple and check the behavior of the app on several platform. At the end of the day PhoneGap is a very powerful framework based upon web standards to create native mobile apps for several platforms sharing the same code base.

## Getting started

With Apache Cordova 2.x the installation process and the set up of the development environment are pretty straight forward. You can now use the build services provided by Adobe, plus Cordova 2.x ships with a set of command-line tools that make it easier to develop cross-platform applications. To install PhoneGap download the latest distribution from the website <http://phonegap.com/download> and unzip the package. When unzipped you’ll get the following folders:

YourInstallationFolder

<dl>
<dd>
-doc

</dd>
<dd>
-lib

<dl>
<dd>
---android

</dd>
<dd>
---bada

</dd>
<dd>
---badaWac

</dd>
<dd>
---blackberry

</dd>
<dd>
---ios

</dd>
<dd>
---symbian

</dd>
<dd>
---webos

</dd>
<dd>
---windows-phone

</dd>
</dl>
</dd>
</dl>
All the needed tools for each platform are bundled in the archive file and for OS X users it is important to install also ios-sim. The ios-sim tool is a command-line utility that launches an iOS application on the iOS Simulator. To install it’s enough to download it from Github, expand it, and launch a command line tool
` $ curl -L https://github.com/phonegap/ios-sim/zipball/1.3 -o ios-sim-1.3.zip $ unzip ios-sim-1.3.zip $ rake install prefix=/usr/local/`
 Using the command line tool move to the appropriate bin directory for the platform you want to create a project (let say Android for instance)
` $ cd phonegap-phonegap-2.0.0/lib/android/bin`
 In order to run the Android SKD tools, you must add them to the path where the Android tools reside. Use the command line tool and mount the path:
` $ export PATH=$PATH:~/android-sdks/tools/ $ export PATH=$PATH:~/android-sdks/platform-tools/ `
 In order to create a PhoneGap project, all you have to do is run the tool ./create from the bin directory of android:
` $ ./create ~/PhoneGapProjects/HelloWorld/android org.webplatform.mobile.phonegap.HelloWorld HelloWorld`
 The tool actually needs three parameters: the path of the project files, the package of the project, and the name of the project.

In the android folder you will find the following directories:

<dl>
<dd>
-assets

<dl>
<dd>
---www

</dd>
</dl>
</dd>
<dd>
-bin

<dl>
<dd>
---res

</dd>
</dl>
</dd>
<dd>
-cordova

</dd>
<dd>
-gen

</dd>
<dd>
-libs

</dd>
<dd>
-res

</dd>
<dd>
-src

</dd>
</dl>
In the assets/www folder you can edit the HTML/CSS/JS in order to make the app working as per your requirement, in order to debug the app move to the /cordova folder and run the *./debug* and *./emulate* commands. In order to be successful you need to have configured previously some virtual devices using the Android SDK.

## How to extend it

The PhoneGap application container exposes native operating system functionality to JavaScript-based applications. All Cordova APIs consist of two related parts: a JavaScript-based interface that can be accessed within your applications, and the corresponding native class for performing operations in native code. Typically, the JavaScript classes and the native classes have APIs that mirrors each other, so that they are easy to follow. Imagine the JavaScript API as a facade to access the plugin without worrying about the native code that works behind the scene. For instance in Android is the *org.apache.cordova.api.Plugin* class is the parent class that the main plugin class have to extend. The JavaScript counterpart relies on the the *cordova.exec* command in order to handle the communication with the native code. Here <https://github.com/phonegap/phonegap-plugins/tree/master/Android> you can find a list of plugins for Android and here <http://docs.phonegap.com/en/2.1.0/guide_plugin-development_index.md.html> some documentation about how to extend PhoneGap.

## How it's born

PhoneGap was originally developed by Nitobi, a company acquired by Adobe in 2011. After it was acquired, Nitobi donated the PhoneGap code base to the Apache Software Foundation (ASF) under the project name Cordova, which is the name of the street in Vancouver where Nitobi’s offices were located and where the company created the first version of the framework. One of biggest advantages to move the code base to the ASF is that big companies can easily contribute to the project (many companies are not only comfortable with the Apache organization and license, but already have a Contributor License Agreement [CLA] with Apache); furthermore, the project is now under an open and transparent government: its community! PhoneGap is a free and openly licensed distribution of Apache Cordova. Picture Cordova to be the engine upon which PhoneGap and its related services (i.e. emulation and build services) are built. For existing PhoneGap developers nothing has changed; but for those who are interested in contributing to the project Apache Cordova is a great chance to join a vibrant open source community. Adobe continues to play a major role in the project, investing in its ongoing development, and the company decided to keep the PhoneGap name to describe its own distribution of the Cordova project. Other contributors to the Apache Cordova project include Google, RIM, Microsoft, IBM, Nokia, Intel, and Hewlett-Packard.

## See also

### External resources

-   Apache Cordova incubator web site <http://incubator.apache.org/cordova/>
-   PhoneGap distribution <http://phonegap.com/>
-   PhoneGap building services <http://build.phonegap.com/>
-   Apache Cordova iOS on github <https://github.com/apache/incubator-cordova-ios>
-   Apache Cordova Android on github <https://github.com/apache/incubator-cordova-android>
-   Ripple Emulator <http://ripple.tinyhippos.com/>
-   PhoneGap Blog <http://phonegap.com/blog>
-   Intel OTC <https://01.org/projects/cordova>
-   Mobile App Development Company <http://www.socialcubix.com/mobile-app-development>
