---
layout: post
title: Code and Gaming
tags: [linux, gaming]
---

Have you ever had come accross a situation where you have opened so many apps in your linux machine and you want to boot into windows, but without closing those apps.

{% highlight js %}
If (yes){
    here are the steps which can help you. 
    Don't shutdown your PC. simply hibernate it.
    
    To hibernate, run ``systemctl hibernate``
    
    Extra cheese :-)
    
        hibernate will kind of shutdown your pc and you have to press power button again to boot into windows. 
        A lazy person never wanna do that, so I have tweaked my hibernation little bit. Here's how you can do the same
        open ``/etc/systemd/sleep.conf.d/hibernatemode.conf`` file and
        
        edit *from*
        
        ``
        [Sleep]
        HibernateMode=shutdown
        ``
        
        *to*
        
        ``
        [Sleep]
        HibernateMode=reboot
        ``
}
else {
    Flew from my blog, You don't belong here. 
}
{% highlight js %}

Comment down below if you find this helpful, else shoooooooooo..
