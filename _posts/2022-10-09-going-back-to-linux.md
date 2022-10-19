---
layout: post
title: Going Back To Linux
date: 2022-10-09 20:44
category: 
author: 
tags: [personal, setup, linux, ramble]
summary: Ramblings about coming back to Linux
---



I used to use Arch Linux as my daily driver OS many years ago (around 2010, maybe), back when I was around 15 years old, this was on a Acer laptop and I used to spend all day looking around and configuring CLI programs and tiling window managers (ratpoison was one of my favorites). At some point I replaced the laptop with a desktop computer and for some reason I never got around to install Linux on it or any other main computer I used since then, its been more than 10 years! Since then I've installed and used Linux on the Raspberry Pi and on servers, but never as a main OS.

And I want to change that now. I have a Lenoxo Thinkpad X1 Carbon that is a few years old but that I use almost daily and that I take with me when I travel, I think its the perfect candidate for this experiment. I did not replace the Windows it came with, rather, I replaced the SSD and did a clean install on it. If I ever need that Windows back I can just pop that drive back in in a few minutes.

This time I went with the Manjaro distribution, and more specifically the Sway community edition. This distro comes prepackaged with a few programs what I was going to install anyway (like FireFox), but more importantly it comes with Sway ready to go. Sway is a tiling window manager for Wayland. So far I have been enjoying it very much.

Coming back to Linux has had a mixed set of problems and issues, and also some other things that go very smoothly. Some things will always be the same: Vim, Nano, Zsh and other programs are still as popular and widely used as ever. But others seem to almost have disappeared (the Musca window manager for example), and that is fine. Getting to know and learn new software, practices and methods is always exciting, even if it sometimes gets in the way.

Speaking of getting in the way. The Manjaro Sway defaults are very sane and good. It is setup in a way that you really don't need to change anything to have a good working setup for everyday use. But it gets problematic if you want to start experimenting and change stuff. Their default config file for Sway and Waybar consist of sourcing a bunch of other files that are spread among many different directories. This can make it really hard if its your first time and you want to change stuff one thing at a time. You will need to hunt down the files for the setting that you need.  

