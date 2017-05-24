---
layout: post
title: "Open Live Writer Version 0.6.2 Is Now Available"
date: 2017-05-24 05:22:23 +0530
categories: [news, release]
author: jongalloway
download: true
---

We're happy to announce a new release of Open Live Writer. We hope you enjoy the new features as much as we enjoyed working on them. Read on to learn more about what issues have been fixed and what features have been added.

The next time you start Open Live Writer and are connected to the internet, it should get updated automatically. But if you can't wait to try out the goodness, download the [updated setup here](https://openlivewriter.azureedge.net/stable/Releases/OpenLiveWriterSetup.exe).

## Release Notes

> Note: Our previous code signing certificate has expired, so this release is signed by a new code signing certificate. Because of this, you may receive warnings from Windows Defender SmartScreen when you run
the installer, indicating that the program is not commonly downloaded and may be unsafe. For more information, see [this help page](http://openlivewriter.org/tutorials/unrecognizedApp.html).

This is primarily a maintenance release to handle issues with publishing images due to Google Blogger. They'd made some changes to how images are uploaded to Google Photos that prevent Open Live Writer from automatically configuring photo publishing. We've added some extra steps to try to configure it, and if we can't set it up for you automatically we link to a help page that shows you how to set it up.

We also added in a few smaller bug fixes and improvements listed below, mostly submitted by the community. Thanks!!!

We added a few features for better High DPI monitor support.

As part of this release, we put a lot of work into making it easier for us to publish new releases. We've automated our build and sign process, so each code check-in will build a new installer for us. There's still some work to do on the Windows Store release process, but we've got a good start on that as well. Well this doesn't immediately translate to any new feature in this release today, it will help you get more frequent updates with both bug fixes and new features going forward.

Special thanks to our contributors for this release:
@ScottIsAFool @vhanla @hashhar @zivkan @paulcbetts @onovotny @kathweaver @gruenwaldt @flcdrg @nimesh-madhavan @lextm 

### Bug fixes

#562 Error: Can't Publish Files- The remote server returned an error: (501) Not Implemented
> This is the master issue for the Google Blogger image publishing problem. Other issues associated with this problem include #608, #600, and #564

#437 Blogger dynamic templates
#438 Fixed WordCounter regex to support Hebrew/Arabic
#521 Support atompub service link with relative url
#487 Adding new intillesense db file to gitignore. Minor annoyance

### Improvements

#589 Several NuGet packages should be updated

### Features

#450 Fix scaling of categories dropdown and options dialog
#585 Implement per-monitor DPI Support
#180 Add support to CSS3 templates
