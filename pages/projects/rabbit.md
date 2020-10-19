---
title: Rabbit
type: project
category: Typography and Fonts
description: Zawgyi to Unicode Converter
creator: ---
link: https://github.com/Rabbit-Converter/Rabbit
language: Java,Javascript
contact: archimedes557@gmail.com
documentation: https://github.com/Rabbit-Converter/Rabbit/blob/master/README.md
added_time: Sun Oct 16 2020 09:55:15 GMT+0630 (Myanmar Time)
---


# Rabbit

Zawgyi to Unicode has been written in [2011](https://github.com/saturngod/ZG2Uni_JS/commits/master). Now, unicode to zawgyi has been finished.

### Why another converter ?

When I was writting [ZG2uni](https://github.com/saturngod/ZG2Uni_JS/) , [Parabaik](https://github.com/ngwestar/parabaik) was not opensource. At that time, I need to use for [MYSTERY ZILLION](http://www.mysteryzillion.org) for converting the whole database to Unicode. So, I wrote ZG2Uni (of course , it has some bugs and some rule missing). 

For Unicode to zawgyi , ~~Parabaik is the GPL license and cannot use in iOS app and Android App~~ Parabaik is the LGPL license. So, decided to write new one with **WTFPL license**.

> I cannot promise , it's correct 100% after converting.

> If you are not using in app or program and just for converting the text , please use [Parabaik](https://github.com/ngwestar/parabaik)

### Demo

- [Web](http://saturngod.github.io/Rabbit/)
- [Android](https://play.google.com/store/apps/details?id=com.comquas.rabbitzawgyiunicodeconverter)

# To Support Other Languages
Todo

- [x] Java
- [x] Objective-C
- [x] Swift
- [x] Python
- [x] PHP
- [x] Ruby
- [x] C#
- [x] Kotlin

## For Java

- required [java-json](http://www.java2s.com/Code/JarDownload/java/java-json.jar.zip) or you can find in `java-json` folder

## For C-Sharp

- add `System.Web.Extensions` in **Reference** for mono

## Build

All the rule are under `source/rule` folder

All the langue template and compile script are under `source/lang` folder

To Build 

```
cd source
node build.js
```

You can get build result under the `output` folder.

## Changelog

### 19/05/2020
- support typescript

### 11/08/2019
- add go lang

### 3/10/2018

- add kotlin and using hash map instead of json. Thanks @vincent-paing
- remove swift 1 and 2 in compile list. No more support.
