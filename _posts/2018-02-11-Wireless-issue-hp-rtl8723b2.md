---
layout: post
title: Wireless issue hp rtl8723b2
tags: [Linux, Wifi]
---

# Wireless issue solved in Linux Hewlett-Packard Company RTL8723BE PCIe Wireless Network Adapter [103c:81c1]

 First of all remove the settings you made. by following command <br>
 <h4>sudo rm /etc/modprobe.d/rtl8723be.conf</h4><br>
 If you do not have this file, nothing is wrong <br>
 Then install a good driver <br>
 <h4>sudo add-apt-repository ppa:hanipouspilot/rtlwifi </h4> <br>
 <h4>sudo apt-get update </h4> <br>
 <h4>sudo apt-get install rtlwifi-new-dkms </h4> <br>
 reboot and enjoy
 <br>
 if you still have problems, you may need to add an option :<br>
 <br>
 <h4>    echo "options rtl8723be ant_sel=2"  | sudo tee /etc/modprobe.d/rtl8723be.conf</h4><br>
 <br>
 then reboot again .
 <br>
 <br>
 <h1> Oh ! i love linux </h1>

