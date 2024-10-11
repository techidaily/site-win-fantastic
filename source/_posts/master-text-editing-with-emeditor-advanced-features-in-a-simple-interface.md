---
title: Master Text Editing with EmEditor - Advanced Features in a Simple Interface
date: 2024-10-09T17:20:57.071Z
updated: 2024-10-11T09:45:04.415Z
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
<li><a href="https://screen-mirroring-recording.techidaily.com/new-voice-storage-test-report-for-2024/"><u>[New] Voice Storage Test Report for 2024</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-follow-the-leaders-on-igtv-for-inspiration/"><u>[Updated] Follow the Leaders on IGTV for Inspiration</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-home-visionarys-review-best-devices-for-clips/"><u>[Updated] Home Visionary's Review Best Devices for Clips</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/8-unexpected-ways-language-expands-your-horizons/"><u>8 Unexpected Ways Language Expands Your Horizons</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/activate-your-apowerrec-vip-account-with-simple-steps-for-both-pc-and-mac-users/"><u>Activate Your ApowerREC VIP Account with Simple Steps for Both PC & Mac Users</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/advanced-nuxt-pro-dashboard-with-argon-theme-enhanced-laravel-integration-by-creative-tim/"><u>Advanced Nuxt Pro Dashboard with Argon Theme - Enhanced Laravel Integration by Creative Tim</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/channel-boosting-strategies-effortless-sponsorship-securing-tips/"><u>Channel Boosting Strategies Effortless Sponsorship Securing Tips</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/comprehensive-walkthrough-for-beginners-getting-started-with-pc-auto-chess-gameplay/"><u>Comprehensive Walkthrough for Beginners: Getting Started with PC Auto Chess Gameplay</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/easy-webcam-video-capture-using-vlc/"><u>Easy Webcam Video Capture Using VLC</u></a></li>
<li><a href="https://sound-issues.techidaily.com/fix-your-windows-1110-bluetooth-stuttering-a-step-by-step-guide-to-smooth-sound/"><u>Fix Your Window's 11/10 Bluetooth Stuttering: A Step-by-Step Guide to Smooth Sound</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/free-solutions-capturing-your-macs-display-using-top-rated-screenshot-tools/"><u>Free Solutions: Capturing Your Mac's Display Using Top-Rated Screenshot Tools</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/incredible-techniques-turning-static-pictures-into-engaging-videos/"><u>Incredible Techniques: Turning Static Pictures Into Engaging Videos</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/mastering-text-overlays-on-video-content-a-comprehensive-tutorial/"><u>Mastering Text Overlays on Video Content: A Comprehensive Tutorial</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/new-in-2024-crack-the-code-4-easy-ways-to-get-filmora-discounts-and-promotions/"><u>New In 2024, Crack the Code 4 Easy Ways to Get Filmora Discounts and Promotions</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/step-by-step-tutorial-to-correct-the-development-error-6034-in-call-of-duty-modern-warfare-for-pc-gamers-and-console-players/"><u>Step-by-Step Tutorial to Correct the Development Error 6034 in Call of Duty Modern Warfare - For PC Gamers & Console Players</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/ultimate-guide-top-substitutes-for-bandicam-on-computers-and-apple-devices/"><u>Ultimate Guide: Top Substitutes for Bandicam on Computers and Apple Devices</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/uncover-and-rescue-gone-footage-the-ultimate-guide-to-samsung-phone-video-recovery/"><u>Uncover and Rescue Gone Footage: The Ultimate Guide to Samsung Phone Video Recovery</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2118314/7443" target="_top" id="2118314">
  <img src="//a.impactradius-go.com/display-ad/7443-2118314" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2118314/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

