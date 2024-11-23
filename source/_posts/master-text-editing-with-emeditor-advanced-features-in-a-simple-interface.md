---
title: Master Text Editing with EmEditor - Advanced Features in a Simple Interface
date: 2024-11-18T17:17:15.141Z
updated: 2024-11-22T21:19:16.079Z
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
<li><a href="https://eaxpv-info.techidaily.com/updated-from-fan-to-earner-understanding-view-requirements-for-2024/"><u>[Updated] From Fan to Earner Understanding View Requirements for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-ideas-on-improving-gopros-energy-management/"><u>[Updated] Ideas on Improving GoPro's Energy Management</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-in-2024-how-to-make-picture-in-picture-videos-on-mac-os-sierra/"><u>[Updated] In 2024, How to Make Picture in Picture Videos on Mac OS Sierra</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-mediacutmaster-review-in-depth-evaluation/"><u>2024 Approved MediaCutMaster Review – In-Depth Evaluation</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/1728489583994-windows/"><u>如何在 Windows 计算机上完成系统重置与回归操作：详细教程</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/additional-tips-about-sinnoh-stone-for-honor-magic-5-drfone-by-drfone-virtual-android/"><u>Additional Tips About Sinnoh Stone For Honor Magic 5 | Dr.fone</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/comparatif-des-logiciels-dexploration-et-de-sauvegarde-de-disque-ssd-choix-entre-transcend-disk-aomei-backupper-and-plus/"><u>Comparatif Des Logiciels D'Exploration Et De Sauvegarde De Disque SSD : Choix Entre Transcend Disk, AOMEI Backupper & Plus</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/easy-and-complete-guide-for-rebooting-your-windows-server-2012-r2-system-expert-strategies/"><u>Easy and Complete Guide for Rebooting Your Windows Server 2012 (R2) System: Expert Strategies</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/how-to-remove-screen-lock-pin-on-nubia-red-magic-8s-proplus-like-a-pro-5-easy-ways-by-drfone-android/"><u>How To Remove Screen Lock PIN On Nubia Red Magic 8S Pro+ Like A Pro 5 Easy Ways</u></a></li>
<li><a href="https://sound-tweaking.techidaily.com/in-2024-title-the-enigmatic-world-of-fibonacci-sequences-and-their-mathematical-implications-in-modern-science/"><u>In 2024, Title The Enigmatic World of Fibonacci Sequences and Their Mathematical Implications in Modern Science</u></a></li>
<li><a href="https://android-unlock.techidaily.com/lock-your-motorola-moto-g84-5g-phone-in-style-the-top-5-gesture-lock-screen-apps-by-drfone-android/"><u>Lock Your Motorola Moto G84 5G Phone in Style The Top 5 Gesture Lock Screen Apps</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/recobra-el-pase-del-tiempo-con-wechat-recuperacion-efectiva-de-conversaciones-antiguas-y-eliminadas/"><u>Recobra El Pase Del Tiempo Con WeChat: Recuperación Efectiva De Conversaciones Antiguas Y Eliminadas</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/top-performant-data-recovery-software-pour-seagate-backup-plus-5-to-guide-comparatif/"><u>Top Performant Data Recovery Software Pour Seagate Backup Plus 5 To: Guide Comparatif</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/verlorene-eintrage-wiederfinden-effiziente-wiederherstellung-in-google-keep/"><u>Verlorene Einträge Wiederfinden - Effiziente Wiederherstellung in Google Keep</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/wechsel-von-spieldaten-zwischen-apple-ids-zwei-effiziente-methoden-erklart/"><u>Wechsel Von Spieldaten Zwischen Apple IDs - Zwei Effiziente Methoden Erklärt</u></a></li>
<li><a href="https://discover-docs.techidaily.com/1728486135401-windows-1011ssd/"><u>Windows 10/11上でSSDへの起動ドライブ容易移行ガイド</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/NC0rdKEQ98o?si=HYgqC8CxF_WTO5if&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

