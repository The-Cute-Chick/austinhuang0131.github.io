---
title: BVE Trainsim 5 Survival Guide
description: Wanna actually play a realistic train simulator FOR FREE? Try BVEts5! Includes Mac installation and recommended scenarios.
comments: true
permalink: /bve
---

Aight, so hear me out: These train simulators on Steam really cost. Like $30+. Honestly, maybe they're better in the 3D graphics, but BVE Trainsim 5 could score much better in performance than these costly alternatives.

## Install
### Windows
Read official instructions and downloads [here](http://bvets.net/en/download/).

### Mac
Yes, you can run BVEts5 on a Mac. Referenced [this blog post](https://kakurasan.blogspot.com/2015/07/bve-trainsim-on-wine.html) (Japanese).

**Known Issues:** Can't show Japanese characters at all. I tried `LANG=ja_JP.UTF-8`, `LANG=ja_JP.Shift_JIS` and `LC_ALL=ja_JP` in Runtime Arguments. If you could solve this, please please please leave a comment below.

1. [Get WineBottler.](http://winebottler.kronenberg.org/) (2.0 is fine.) Load the disk image, drag both WineBottler and Wine to the Applications folder. (Non-Sudo people: Or any folder you like - I drag to the Downloads folder. But both apps should be in the same folder. I didn't try otherwise.)
2. [Get BVE 5 WITHOUT INSTALLER.](http://bvets.net/en/download/zip.html) Unzip it.
3. Launch WineBottler.
4. Click Advanced.
5. For Program Installation, select the `BveTs.exe` in the folder.
6. For Installation mode, select "copy file (program) and all files in the folder to the App Bundle."
7. For System Version Info, select 7. (BVE 5 requires Vista or higher.)
8. You MUST tick "Include Mono". I didn't tick "Include Gecko", but I think it's okay if you leave it on.
9. For Winetricks, find the following and tick them: `dotnet35` (MS .NET 3.5), `d3dx9_43` (MS d3dx9_43.dll), and `mdx` (Managed DirectX).
10. Tick Silent Install.
11. Press Install, set file name, and go. Takes like 2 minutes to install, then you get an .app bundle. Off you go!

## [WIP] Scenarios
Yes yes, I know many English scenarios are made in BVE 4 or OpenBVE. I know [Converter](http://bvets.net/en/download/conv.html) exists. But isn't it better to play scenarios that actually support 5?
* Windows users: Place all Scenarios in `C:\users\<name>\My Documents\BveTs\Scenarios`.
* Mac users: Place all Scenarios in `/Users/<name>/Documents/BveTs/Scenarios` (which is equivalent to `~/Documents/BveTs/Scenarios`).

All scenarios should contain 1 folder and a bunch of TXT files (Which tells BVE what route to drive) outside the folder. If there's only 1 folder with nothing else, either it's a Vehicle file (I'll indicate) or you forgot to look inside when you unzip.

### Tama Toshi Monorail
Download [here](http://neclgm.blog.fc2.com/blog-entry-58.html). Both the page AND THE SCENARIO is in English!

To start the train from the terminus, you'll need to press ATS 0 (S) - ATS 13 (J) - ATS 4 (B2), BEFORE releasing the emergency brake or touching the reverser. Your train WILL NOT MOVE if you don't do so.
* On Windows, that is <kbd> SPACE </kbd> - <kbd>8</kbd> - <kbd>END</kbd>. You can also press <kbd>Delete</kbd> for a list of key assignments specific to that scenario.
* On Mac, or if your Windows computer does not have an <kbd>END</kbd> key, you'll need to reassign keys. Right click => Preferences => Input device => Key assignments... => Switches => Find "ATS 4 (B2)" => Press the On/Off box below => Press the key you want to assign (Fn combos accepted, no other combos). If you want to show the in-game key assignment list (Just this game), you'll need to reassign "ATS 2 (A2)" as well.
* Here's a walkthrough:

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/u58bNLPdQew" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Keihan Keishin Line
**Resource-Heavy! Requires good GPU!!!** Download [here](https://www.like-a-lake.com/bve-keihan-keishin/). Find "Mirror site(yahoo box)" and you'll see two columns: The left with Installer, the right without. You'll also see a OneDrive link and a Yahoo Box (Japanese) link.

* Station names are in English.
* Mac users: Ignore errors when loading the scenario, they don't affect the gameplay that much. Tested multiple times.
* To start the train from the terminus, you'll need to press <kbd>5</kbd> to enable ATS (Or you will not be able to drive - The line does not have ATO), and switch the reverser to the front. Then, **remain on Emergency Brake** until you're told to depart by the screen message (Or ATS will stop you. If you forgot this: Get back on P0 AND Emergency Brake (By pressing <kbd>/</kbd>), then release it again).
* Seriously, **abide speed limit.** This is ATS, not ATC, and Deadman's Switch gets activated extremely often, which will you give you a big delay off your schedule.
  * IF there's a red light in the bottom-left corner, you're screwed: You just triggered ATS. To release, Get back on P0 AND Emergency Brake (By pressing <kbd>/</kbd>), then <kbd>6</kbd> (Disable ATS) + <kbd>5</kbd> (Enable ATS).
* Here's a walkthrough:

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/Zcpggd-N0pM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### TRTA Hanzomon Line
Download [here](http://shtr-m.net/bve/hanzomon.html). Click the first link wrapped by `>><<` in the first heading.

For this scenario, you'll need to download vehicles.
1. Go [here](http://vertah.sakura.ne.jp/bvedata/train.html).
2. You need 8000, 08, 8590, and 30000. (For TKK 2000, download [here](http://bve.jpn.org/tokyu2000.html) instead, but it's an EXE file.)
3. Click the link at the bottom of each box.
4. For 8000: The download link is in the purple box at the bottom of the page. For others: First text link in the second-last box at the bottom.
5. Unzip them and place them in `.../Scenarios/vertah`.

* To start the train from the terminus, you'll need to press <kbd>8</kbd> to enable ATC for Metro.
* Here's a walkthrough for one of the routes:

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/XDeNjNsnG4I" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>