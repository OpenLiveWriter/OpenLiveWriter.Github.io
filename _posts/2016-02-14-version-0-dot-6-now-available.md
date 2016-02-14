---
layout: default
title: "Version 0.6 Now Available"
date: 2016-02-14 05:22:23 +0530
categories: [news, release]
author: hashhar
download: true
---
# Open Live Writer v0.6.0.0 is now available!

After about two months since the initial public release the team and community have managed to add features, fix issues and fulfill the demand for some of the more requested features like spell checking (it will only work on Windows 8 and later though) and support for Blogger categories. We hope you enjoy the new features as much as we enjoyed working on them. Read on to learn more about what issues have been fixed and what features have been added.

The next time you start Open Live Writer and are connected to the internet, it should get updated automatically. But if you can't wait to try out the goodness, download the [updated setup here](https://openlivewriter.azureedge.net/stable/Releases/OpenLiveWriterSetup.exe).

## Release Notes

For spell checking to work you'll need to have Windows 8 or newer installed (Windows 7 does not have spell checking support) and you’ll need to install your preferred input language in Windows to enable spell checking in that language. Only one language can be spell checked in Open Live Writer at a time, but you can change the language at any time by going to **File > Options > Spelling** and choosing a new dictionary language.

Google Blogger categories will automatically populate for easy tagging of your blog posts. In addition to categories, there are several other Google Blogger bug fixes in this release. The most notable issues were time zone differences causing scheduled posts to be scheduled at the incorrect time, failing to open drafts that were posted to Blogger, and failing to download and open posts from Blogger that are older than your most recent 500 posts.

### Bug fixes

[#190](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/190) - Saving doesn't mark categories as saved  
[#103](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/103) - Errors when using invalid url to insert an image  
[#323](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/323) - ArgumentNullException when getting recent posts on empty blog  
[#301](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/301) - Can't retrieve drafts from Google Blogger  
[#247](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/247) - Can't Edit Old Blogger Posts (>500)  
[#224](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/224) - Google Blogger scheduled post is scheduled at the wrong time  

### Improvements

[#239](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/239) - Fix issue with spaces in username  
[#281](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/281) - Test Plans

### Features

[#130](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/130) - Add spell check feature back in OLW  
[#234](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/234) - Support Blogger categories

---

### Special thanks to our contributors for this release:

<img src="https://github.com/willduff.png" class="avatar" alt="willduff avatar" width="40" height="40">  [@willduff](https://github.com/willduff)

<img src="https://github.com/martinwoodward.png" class="avatar" alt="martinwoodward avatar" width="40" height="40">  [@martinwoodward](https://github.com/martinwoodward)

<img src="https://github.com/bbowyersmyth.png" class="avatar" alt="bbowyersmyth avatar" width="40" height="40">  [@bbowyersmyth](https://github.com/bbowyersmyth)

<img src="https://github.com/kathweaver.png" class="avatar" alt="kathweaver avatar" width="40" height="40">  [@kathweaver](https://github.com/kathweaver)

<img src="https://github.com/jannavarro.png" class="avatar" alt="jannavarro avatar" width="40" height="40">  [@jannavarro](https://github.com/jannavarro)

<img src="https://github.com/hashhar.png" class="avatar" alt="hashhar avatar" width="40" height="40">  [@hashhar](https://github.com/hashhar)

<img src="https://github.com/jmbucknall.png" class="avatar" alt="jmbucknall avatar" width="40" height="40">  [@jmbucknall](https://github.com/jmbucknall)
