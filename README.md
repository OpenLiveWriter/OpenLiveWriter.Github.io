# OpenLiveWriter.com Amazing Website
The website for http://openlivewriter.com is hosted on GitHub pages using the source in this repository.
Note that issues should only be logged against the website itself - for Open Live Writer application issues or enhancements see
the [OpenLiveWriter repo](https://github.com/OpenLiveWriter/OpenLiveWriter/issues/).

### License
Open Live Writer proudly uses the [MIT License](license.txt).

### Roadmap
You can find the roadmap for the Open Live Writer product [here](https://github.com/OpenLiveWriter/OpenLiveWriter/blob/master/roadmap.md).

For the website, we are initially focussed on getting a fast, lightweight product homepage set up. Then we want to increase the end
user help content to assist people using Open Live Writer. [Developer documentation should live alongside the code](https://github.com/OpenLiveWriter/OpenLiveWriter/).

### Contributing
Open Live Writer is an open source project and wouldn't exist without the passionate community of volunteers
and the same is true of the [website contributors](https://github.com/OpenLiveWriter/OpenLiveWriter.github.io/graphs/contributors).

To contribute to the website simply:
  1. Fork the repo and clone locally
  2. Create a specific topic branch, add a nice feature or fix your bug
  3. Send a Pull Request to spread the fun!

If you haven't already, please sign the [.NET Foundation CLA](http://cla2.dotnetfoundation.org) to give us 
permission to include your code in the next release of Open Live Writer.

This project has adopted the code of conduct defined by the [Contributor Covenant](http://contributor-covenant.org/) to clarify expected behavior in our community.
For more information see the [.NET Foundation Code of Conduct](http://www.dotnetfoundation.org/code-of-conduct).

For developer chatter, head on over to the [OpenLiveWriter Gitter room]((https://gitter.im/OpenLiveWriter/OpenLiveWriter?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)):
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/OpenLiveWriter/OpenLiveWriter?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

### For the people writing posts and news items:

All the files within **`_posts`** should have this section at the top of the file.

```
---
layout: default
title: 'Initial public release'
version: 0.5.0.0
categories: [release, news]
date: 2015-12-09 00:00:00 -0800
author: martinwoodward
download: true
---
```
Do not change the `layout`.  
`title`: The text that you want to see on the page.  
`version`: The version number of OLW about which the post is concerned.  
`categories`: Comma separated categories within braces. If this contains `blog` it goes to `/blog`, if it contains `news` it goes to `/news`. If both, then it will be present in both places.  
`date`: yyyy-mm-dd hh:mm:ss timezone (timezone is of the form +0530 or -0800, ie. +/-hhmm).  
`author` is the GitHub username of the author. Used to link to their profile and show a small gravatar.  
`download`: I'm not sure what this does but let it be.

### .NET Foundation
The Open Live Writer project is supported by the [.NET Foundation](http://www.dotnetfoundation.org).

