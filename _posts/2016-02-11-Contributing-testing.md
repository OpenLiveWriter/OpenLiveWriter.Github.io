---  
layout: default  
title: 'Contributing to Documentation'  
categories: [blog]  
date: 2016-02-11 00:00:00 -0800  
author: kathweaver  
download: true  
---

One of the best ways to contribute is testing.  There are test plans and some 
information in the source, under the directory test plans.  Also feel free to 
check those and update them if you find an issue.

They are basically check lists that go through every function of the software and tell 
what should happen when you do them, including images.  We came up with this on my last
programming gig, and they helped everyone.  

The programmers then knew what we were expecting and so did QA.  I often had QA help me with
them so that they would have some ownership.

So what do you test and how?

Each time a developer makes a pull request, you should go through the new functionality 
and make sure it behaves as expected.  Then you should go through the rest of the software
making sure that something wasn't accidently broke.  

At least two different people should go through the process, but the more the better.  It also
helps if someone goes through it that has a fresh eye on the software.

So where do you find the executeable?  To do the last build in the pull request,
scroll down to the point where you see "All checks have passed", and click on "Show All Checks".
Click on "Details", then "Artifacts", and will see OpenLiveWriteSetup.exe -- download 
that and run it even if you get messages from Windows saying it isn't safe.

If you do find an error, give the developer as much information as you can.  Screenshots, error messages,
log files, you name it.  The more complete you are, the less time the developer has to spend tracking
the error down.

-----

You can also test the nightly build.  It will contain everything that has been merged.

You can setup OpenLiveWriter to always run the nightly build:
Go to regedit, find the registery key: HKEY_CURRENT_USER\SOFTWARE\OpenLiveWriter\Updates
Then you need to create a dword key for CheckForBetaUpdates 1 = beta, 0 = regular.

You can also pull the nightly build manually by going to this link:
https://ci.appveyor.com/project/dotnetfoundation/openlivewriter/build/artifacts

Or click on the build button from the readme and then click on latest build, artifacts

Again, if you find a problem you'll need to raise an issue and give as much information as you can.
