---
layout: post
title:  "Cara mudah instal bot eggdrop"
date:   2012-05-18 22:27:21 -0500
categories: eggdrop
---
Login ke vps / shell kalian..<br>
<br>
ambil filenya dengan cara:<br>
<span>wget ftp://ftp.eggheads.org/pub/eggdrop/source/1.6/eggdrop1.6.21.tar.gz<br>
<br></span>setelah selesai... extract file nya dengan cara<br>
<span>tar zxvf</span></span> <span style="font-family:'Trebuchet MS';"><em>eggdrop1.6.21.tar.gz<br>
<br></em></span>setelah itu masuk folder eggdrop dengan perintah<br>
<span style="font-style:italic;">cd</span> <span style="font-family:'Trebuchet MS';"><span style="font-style:italic;">eggdrop1.6.21</span><br>
setelah berada pada folder eggdrop1.6.21 saatnya mulai kompile dengan perintah² berikut:<br>
<span style="font-style:italic;">./configure</span><br>
<span style="font-style:italic;">make<br>
make install<br>
<br></span>setelah semua done,, silahkan anda masuk folder eggdrop dengan perintah<br>
<span style="font-style:italic;">cd ~/eggdrop<br>
<br></span>di sini anda harus menyiapkan:<br>
<br>
<strong>1 file konfig *<br>
tcl² wajib (seperti walls)*</strong></span><br>
anda bisa melihat contoh config saya.. <a href="http://egg.url.ph/egg.conf">di sini</a>..<br>
setelah semua siap.. jalankan dengan perintah<br>
<span style="font-style:italic;">./eggdrop -m namaconfig<br></span>mudah kan?? sebenarnya saya sudah membuat bash untuk install otomatis, silahkan di coba pada <a href="http://egg.url.ph">http://egg.url.ph</a><br>
jika kurang jelas silahkan menuju blog saya yang membahas eggdrop di <span style="font-style:italic;"><a href="http://eg-goez.blogspot.com">eg-goez.blogspot.com</a>
