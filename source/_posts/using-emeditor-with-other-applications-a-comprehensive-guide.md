---
title: "Using EmEditor with Other Applications: A Comprehensive Guide"
date: 2024-10-08T20:10:34.793Z
updated: 2024-10-10T22:03:03.895Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/de67db97111b230778d53cfacb51bb9c7a1356b2082aff96997373a5633f37e3.jpg
---

## Using EmEditor with Other Applications: A Comprehensive Guide

January 10, 2011 at 5:03 am [#9184](https://tools.techidaily.com/emeditor/products/) 

[![](https://secure.gravatar.com/avatar/d48a4b8332642b90e109a726bc885d5e?s=80&d=identicon&r=g)scrabbles](https://www.emeditor.com/forums/users/scrabbles/ "View scrabbles's profile")

Member

Hi qjunkim,

 I’m the author of that blogpost (thanks muchly for posting that link here flamerz). The rrun (emeditor macro) script allows you to run only selected lines as well, though the version available will (as you say) run rterm each time.

 I have modified the script, so that if a flag called “useSource” is set true, and you have a running instance of RGui + R Console (default when rgui is launched from shortcut), it will run the code in that instance and not reload rterm each time. I found it was more reliable to use the “source” command, rather than sending strings to the REPL;  
 eg source(“C:/test.r”,echo=TRUE,keep.source=TRUE)

 echo and keep.source args are hardcoded in the script, but of course feel free to modify that! in r, if you are not already familiar with this command, try “help(source)” for more options.

 I’ll upload the script and do a little blog post about it to explain it more.

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
<li><a href="https://youtube-lab.techidaily.com/ed-diy-guide-screen-capture-and-sound-from-youtube-for-2024/"><u>[Updated] DIY Guide Screen Capture & Sound From YouTube for 2024</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-facebook-instream-ads-how-to-setup-and-evaluate-facebook-instream-ad-for-2024/"><u>[Updated] Facebook Instream Ads | How to Setup and Evaluate Facebook Instream Ad for 2024</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/updated-in-2024-how-to-react-when-youre-your-own-reflection-in-a-video-call/"><u>[Updated] In 2024, How to React When You're Your Own Reflection in a Video Call</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/exploring-the-fallout-microsoft-365-suffers-during-a-severe-distributed-denial-of-service-incident-covered-by-zdnet/"><u>Exploring the Fallout: Microsoft 365 Suffers During a Severe Distributed Denial-of-Service Incident Covered by ZDNET</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-to-cast-oppo-f25-pro-5g-screen-to-pc-using-wifi-drfone-by-drfone-android/"><u>How to Cast Oppo F25 Pro 5G Screen to PC Using WiFi | Dr.fone</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/smart-savings-without-compromising-quality-why-i-chose-the-most-affordable-microsoft-surface-pro-model-gadgetsforgeeks/"><u>Smart Savings without Compromising Quality: Why I Chose the Most Affordable Microsoft Surface Pro Model | GadgetsForGeeks</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/upcoming-change-alert-microsoft-introduces-fees-for-future-windows-11-update-installations-cost-breakdown/"><u>Upcoming Change Alert: Microsoft Introduces Fees for Future Windows 11 Update Installations - Cost Breakdown</u></a></li>
<li><a href="https://video-ai-editor.techidaily.com/updated-2024-approved-install-vllo-on-mac-and-browse-alternative-solutions/"><u>Updated 2024 Approved Install VLLO on Mac and Browse Alternative Solutions</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/why-participate-a-step-by-step-tutorial-on-joining-microsofts-exclusive-windows-testing-program-featured-by-zdnet/"><u>Why Participate? A Step-by-Step Tutorial on Joining Microsoft's Exclusive Windows Testing Program, Featured by ZDNet</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1884021/19272" target="_top" id="1884021">
  <img src="//a.impactradius-go.com/display-ad/19272-1884021" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1884021/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

