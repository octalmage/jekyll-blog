---
layout: post
title: "Google Music Hacking"
---

I've been using [cycript](http://www.cycript.org/) for testing and there's a steep learning curve. So far this guide: 

[http://highaltitudehacks.com/2013/07/02/ios-application-security-part-5-advanced-runtime-analysis-and-manipulation-using-cycript-yahoo-weather-app/](http://highaltitudehacks.com/2013/07/02/ios-application-security-part-5-advanced-runtime-analysis-and-manipulation-using-cycript-yahoo-weather-app/)

with this: 

[http://resources.infosecinstitute.com/penetration-testing-for-iphone-applications-part-5/](http://resources.infosecinstitute.com/penetration-testing-for-iphone-applications-part-5/)

has been very helpful. Also this: 

[http://iphonedevwiki.net/index.php/Cycript_Tricks](http://iphonedevwiki.net/index.php/Cycript_Tricks)

A few instresting commands (get printMethods from above link): 

```
UIApp.windows
UIApp.keyWindow
```

```
printMethods(AppDelegate)
```

You can also access these varibles: 

[https://gist.github.com/octalmage/7410d7442c7940baea11#file-play_music-h-L1095](https://gist.github.com/octalmage/7410d7442c7940baea11#file-play_music-h-L1095)

With this: 

```
UIApp.delegate.appVersion
```
