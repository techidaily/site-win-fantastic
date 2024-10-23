---
title: "Using EmEditor with Other Applications: A Comprehensive Guide"
date: 2024-10-18T04:03:50.309Z
updated: 2024-10-22T20:51:41.578Z
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
<li><a href="https://youtube-webster.techidaily.com/nlock-creative-expression-mastering-jump-cut-usage/"><u>[New] Unlock Creative Expression Mastering Jump Cut Usage</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/1-ultime-solutions-de-transfert-pour-ssd-avec-transcend-disk-manager-et-outils-dechelle-comme-easeus-todo-backup/"><u>1. Ultime Solutions De Transfert Pour SSD Avec Transcend Disk Manager Et Outils D'Échelle Comme EaseUS Todo Backup</u></a></li>
<li><a href="https://video-capture.techidaily.com/audio-ambition-realized-cutting-edge-recording-methods-for-minecraft-players-for-2024/"><u>Audio Ambition Realized Cutting-Edge Recording Methods for Minecraft Players for 2024</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/guide-complet-creer-un-disque-reparation-pour-windows-aturage-etapes-faciles-et-methodiques/"><u>Guide Complet : Créer Un Disque Réparation Pour Windows Aturage - Étapes Faciles Et Méthodiques</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/how-to-use-ispoofer-on-nokia-c300-drfone-by-drfone-virtual-android/"><u>How to use iSpoofer on Nokia C300? | Dr.fone</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-full-tutorial-to-bypass-your-oneplus-nord-n30-se-face-lock-by-drfone-android/"><u>In 2024, Full Tutorial to Bypass Your OnePlus Nord N30 SE Face Lock?</u></a></li>
<li><a href="https://facebook.techidaily.com/navigating-social-media-silence-is-fb-offline/"><u>Navigating Social Media Silence - Is FB Offline?</u></a></li>
<li><a href="https://review-topics.techidaily.com/possible-solutions-to-restore-deleted-music-from-tecno-by-fonelab-android-recover-music/"><u>Possible solutions to restore deleted music from Tecno</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/resolving-the-d-drive-disappearance-issue-in-windows-11-update/"><u>Resolving the D: Drive Disappearance Issue in Windows 11 Update</u></a></li>
<li><a href="https://fox-place.techidaily.com/step-by-step-guide-saving-your-windows-11-system-and-documents-on-a-shared-network-storage/"><u>Step-by-Step Guide: Saving Your Windows 11 System and Documents on a Shared Network Storage</u></a></li>
<li><a href="https://tech-revival.techidaily.com/unlocking-creative-solutions-top-8-applications-of-chatgpt-in-visual-fields/"><u>Unlocking Creative Solutions: Top 8 Applications of ChatGPT in Visual Fields</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/windowsusbcmd/"><u>Windows環境下でUSBメモリが再フォーマットされた場合のファイル損失に対処し、CMDを使ってデータ復元法</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2043593/7443" target="_top" id="2043593">
  <img src="//a.impactradius-go.com/display-ad/7443-2043593" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2043593/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

