---
title: "Using EmEditor with Other Applications: A Comprehensive Guide"
date: 2024-11-16T01:12:33.358Z
updated: 2024-11-22T23:41:01.308Z
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
<li><a href="https://facebook-video-recording.techidaily.com/new-2024-approved-social-media-strategies-for-showcasing-your-video-content/"><u>[New] 2024 Approved Social Media Strategies for Showcasing Your Video Content</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/new-compreenas-a-step-by-step-process-to-apply-luts-in-photoshop-cc/"><u>[New] Compreenas a Step-by-Step Process to Apply LUTs in Photoshop CC</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/new-youtubes-celebrated-click-it-achievements/"><u>[New] YouTube's Celebrated Click-It Achievements</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/approved-mp3-upload-process-stream-convert-and-share-on-youtube-quickly/"><u>2024 Approved MP3 Upload Process Stream, Convert & Share on YouTube Quickly</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/how-mozilla-revolutionized-screen-splitting-with-ffxp/"><u>How Mozilla Revolutionized Screen Splitting with FFXP</u></a></li>
<li><a href="https://tech-revival.techidaily.com/how-to-effortlessly-reduce-video-file-size-a-ranking-of-the-best-techniques-for-secure-email-attachments/"><u>How to Effortlessly Reduce Video File Size: A Ranking of the Best Techniques for Secure Email Attachments</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/lautstarke-und-nicht-bootende-festplatten-problemlosung-fur-interne-and-externe-laufwerke/"><u>Lautstarke Und Nicht Bootende Festplatten - Problemlösung Für Interne & Externe Laufwerke</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/logiciel-de-recuperation-de-donnees-pour-windows-10-fichiers-perdus-restaure-gratuitement/"><u>Logiciel De Récupération De Données Pour Windows 10 : Fichiers Perdus, Restauré Gratuitement</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/sicheres-datensicherungsverfahren-mit-automatischem-nas-backup-in-windows-betriebssystemen/"><u>Sicheres Datensicherungsverfahren Mit Automatischem NAS-Backup in Windows-Betriebssystemen</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/step-by-step-tutorial-on-resetting-your-asus-uefi-bios-on-windows-11-devices/"><u>Step-by-Step Tutorial on Resetting Your ASUS UEFI BIOS on Windows 11 Devices</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/ultimate-tutorial-on-effective-techniques-for-retrieving-data-from-a-damaged-hard-disk/"><u>Ultimate Tutorial on Effective Techniques for Retrieving Data From a Damaged Hard Disk</u></a></li>
<li><a href="https://win-workspace.techidaily.com/1728486919512-usb/"><u>USBメモリーから取り出されたデータの復活手段５種</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/htnQWyEOCgc?si=fy86hi8_hTtbWAnw&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

