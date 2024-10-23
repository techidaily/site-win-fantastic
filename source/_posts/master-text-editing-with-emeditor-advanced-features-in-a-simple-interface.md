---
title: Master Text Editing with EmEditor - Advanced Features in a Simple Interface
date: 2024-10-16T17:12:25.990Z
updated: 2024-10-22T16:59:56.406Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/e24c6a589d856da0a108fb73ed8aea987528294a85122e6caa68a425ef40bc26.jpg
---

## Master Text Editing with EmEditor - Advanced Features in a Simple Interface

June 23, 2014 at 1:57 pm [#18589](https://tools.techidaily.com/emeditor/products/) 

[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")

Participant

Interesting.  
 The above shown ways should do it. Well, at least with smaller files size.

Unfortunately I can’t really test on my 32-bit system,… I have to many things running and not enough free memory for testing.

  
 For an test I created a 581 MB text file with 130.000 x 4689 signs.  
 Open that in 32-bit EmEditor 14.4.0b2 shows this dialog:

```
---------------------------
EmEditor
---------------------------
This file contains a very long line. 
Very long lines will be split into several lines while the document is open, 
but will be recombined when saved. Highlighting very long lines is disabled, 
and some other features such as find and replace text containing CR or LF 
might not work correctly for very long lines.

c:\temp\jsout.txt
---------------------------
OK   Abbrechen   
---------------------------

```

and I ended up with 5 lines:  
 4x 134217729 chars  
 1x 072699089 chars

“Wrap by Char” was disabled.  
  
 RegEx s&r allocated 1,2 GB and I canceled after 3 minutes.

So I just quickly split the lines with SED.exe  
 c:\\temp>sed -e “s/.\\{4689\\}/&\\n/g” jsout.txt > jsoutSplitted.txt

Unfortunately here I also run out of memory, but with a smaller file this works well.  
 So on a 64-bit system that should be no problem,…I will try tomorrow just out of curiosity.

Code to create a test file (due to little memory I had to do a additional step as workaround)

```
Line="";
for(B=1, Bs=4689; B<=Bs; B++){
  Line += "X";

File="";
for(L=1, Ls=13000; L<=Ls; L++){
  File += Line ;

fso     = new ActiveXObject("Scripting.FileSystemObject");
oFile   = fso.OpenTextFile("C:\\temp\\jsout.txt", 2, true)
for(F=1; F<=10; F++)
  oFile.Write(File);
oFile.Close();

```

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://facebook-video-share.techidaily.com/new-2024-approved-essential-rules-of-engagement-on-youtube/"><u>[New] 2024 Approved Essential Rules of Engagement on YouTube</u></a></li>
<li><a href="https://extra-skills.techidaily.com/new-mastering-video-directorship-with-powerdirector-24/"><u>[New] Mastering Video Directorship with PowerDirector '24</u></a></li>
<li><a href="https://some-guidance.techidaily.com/new-the-zen-of-zoom-perfecting-your-video-experience/"><u>[New] The Zen of Zoom Perfecting Your Video Experience</u></a></li>
<li><a href="https://location-social.techidaily.com/4-feasible-ways-to-fake-location-on-facebook-for-your-lava-storm-5g-drfone-by-drfone-virtual-android/"><u>4 Feasible Ways to Fake Location on Facebook For your Lava Storm 5G | Dr.fone</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/effacement-complet-dun-ssd-avec-windows-11-explique-procedures-permanentes-and-simples/"><u>Effacement Complet D'un SSD Avec Windows 11 Expliqué: Procédures Permanentes & Simples</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/expert-insights-on-the-netgear-orbi-rbs5n-model-the-perfect-wifi-booster-for-backyards/"><u>Expert Insights on the Netgear Orbi RBS5n Model: The Perfect WiFi Booster for Backyards</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/five-simple-fixes-to-recover-your-lost-outlook-folders-effective-tips/"><u>Five Simple Fixes to Recover Your Lost Outlook Folders - Effective Tips</u></a></li>
<li><a href="https://media-tips.techidaily.com/how-to-access-and-open-an-opus-file-a-comprehensive-guide/"><u>How to Access and Open an OPUS File: A Comprehensive Guide</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/how-to-change-your-sim-pin-code-on-your-poco-x5-pro-phone-by-drfone-android/"><u>How To Change Your SIM PIN Code on Your Poco X5 Pro Phone</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/1728502490886-robocopy/"><u>Robocopy遵照计划进行扩展式备份的详解</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/seamless-integration-how-to-use-your-favorite-android-apps-directly-on-a-windows-10-desktop/"><u>Seamless Integration: How to Use Your Favorite Android Apps Directly on a Windows 10 Desktop</u></a></li>
<li><a href="https://sound-issues.techidaily.com/solution-steps-for-defective-steelseries-arctis-pro-headset-mic/"><u>Solution Steps for Defective SteelSeries Arctis Pro Headset Mic</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/ultimate-tutorial-on-starting-your-pc-with-an-hp-usb-drive-in-windows-11/"><u>Ultimate Tutorial on Starting Your PC with an HP USB Drive in Windows 11</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2134501/19576" target="_top" id="2134501">
  <img src="//a.impactradius-go.com/display-ad/19576-2134501" border="0" alt="https://techidaily.com" width="640" height="90"/>
</a>
<img height="0" width="0" src="https://aidotcom.pxf.io/i/5597632/2134501/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

