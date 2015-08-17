---
layout: post
title: Localize osx folder names
---

#Localize osx folder names

All localized folder names are located in `/System/Library/CoreServices/SystemFolderLocalizations/XX.lproj/SystemFolderLocalizations.strings` in binary format by default where `XX` stands for your locale name.

Before edit it you need to convert that in xml format with `sudo plutil --convert xml1 SystemFolderLocalizations.strings`

Finished editing the file you can convert that back to binary format with `sudo plutil --convert binary1 SystemFolderLocalizations.strings`

Now you need to restart Finder with `killall -KILL Finder`
