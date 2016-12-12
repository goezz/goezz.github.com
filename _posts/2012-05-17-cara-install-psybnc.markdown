---
layout: post
title:  "Cara install Psybnc"
date:   2012-05-17 22:28:21 -0500
categories: psybnc
---
Login ke shell / vps kalian<br>
ambil src nya dengan cara<br>
<em>wget http://psybnc.at/download/beta/psyBNC-2.3.2-7.tar.gz</em></span><br>
extract dengan cara<br>
<span style="font-style:italic;">tar zxvf</span> <span style="font-family:'Trebuchet MS';"><span style="font-style:italic;">psyBNC-2.3.2-7.tar.gz</span><br>
masuk directory psybnc<br>
<span style="font-style:italic;">cd psybnc</span><br>
kompile pertama (ini penting)<br>
jika anda menginginkan user lebih dari 50 karena untuk default max usernya 50 anda bisa kompile dengan cara<br>
<span style="font-style:italic;">make menuconfig</span><br>
<strong>Catatan:</strong></span> tidak semua shell / vps sudah terinstall curses, jika anda menemukan masalah error seperti ini:<br>
<span style="font-style:italic;">This needs the ncurses library. If it is not available, menuconf wont work. If you are using curses, use make menuconfig-curses instead.<br>
make: *** [menuconfig] Error 1</span><br>
ini sebabnya pada server anda tidak terinstall <em><a href="http://eg-goez.blogspot.com/2014/05/installing-libncurses5-dev-centos-debian.html">libncurses</a>,</em> jika anda pemegang root, ada baiknya anda <a href="http://eg-goez.blogspot.com/2014/05/installing-libncurses5-dev-centos-debian.html">install <em>libncurses5-dev</em></a> dahulu, tapi meskipun anda melewati ini, proses installasi tetap bisa di jalankan, hanya anda tidak bisa enable untuk bagian misal SSL Support / Identd / Max Users, tapi jangan worry, dont khawatir, anda bisa merubah manual,,<br>
jalankan saja perintah make menuconfig seperti di atas,, lalu edit file <strong>config.h<br></strong>dengan cara:<br>
<span style="font-style:italic;">nano config.h</span><br>
cari tulisan ini<br>
#define MAXUSER 50<br>
ganti 50 dengan sembarang dehh.. 99999 juga boleh,, tapi # jangan di apus ea..<br>
setelah oke,, simpan dengan cara tekan<br>
CTRL+X (yes)<br>
jalankan kompile lagi<br>
<span style="font-style:italic;">make</span><br>
setelah itu edit file psybnc.conf<br>
<span style="font-style:italic;">nano psybnc.conf</span><br>
stell port nya,,<br>
setelah di CTRL+X (yes)<br>
jalankan dengan perintah<br>
<span style="font-style:italic;">./psybnc<br>
done
