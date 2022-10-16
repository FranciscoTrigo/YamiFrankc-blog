---
layout: post
title: Make a Discord bot for Home Assistant with Node-Red
date: 2022-09-24 03:46
category: 
tags: []
summary: 
---

<style type="text/css">
    .image-wrapper {
    text-align: center;
    /* background-color: brown; */
    color: gray;

    .image-caption {
        margin-top: $spacing-unit / 3;
    }
}
</style>

I have a Home Assistant server running in my house with many different integrations and its working mostly greatly. Home Assistant has a Discord integration that you can use to send notifications with the integrated automation system, but I still fell like that system is a bit cumbersome for anything but the most simple integrations. That is why I decided to manage my Discord Home Assistant bot with Node-Red.  
In this post I will show the steps to create a basic Discord bot that you can build upon depending on your needs.

## Prerequisites

For you to be able to follow this tutorial you will need the following:

- An existing Home Assistant instance.
- Node-Red installed somewhere and already integrated with your Home Assistant.
- A Discord server or channel where your bot can live without unauthorized access.

## Prepare the bot

First we are going to create a Discord bot. You need to go to the [Discord's developer portal](https://discord.com/developers/applications/) and login with your Discord account.
Click on the button on the top right side to create a new app. Give it a name and continue.

{% include image.html
    img="assets/hassio-discord/make-bot.png"
    title="Cool screenshot"
    caption="You can also see a list of all your created apps here!" %}

Click on your bot's icon and then click on "Bot" on the left. Here you will be able to assign a name to it and also a profile picture. 
After you set that up click on "Click to reveal token". It will give you your unique token to control the bot. Copy it and save it, we will need it.  

DO NOT SHARE THIS WITH ANYBODY.  
If for some reason you need to change your token in the future, you can do it here.

{% include image.html
    img="assets/hassio-discord/2bot.png"
    title="Bots"
    caption="Look at the directions" %}

## Set up in Node-Red

We are going to use the [node-red-contrib-discord-advanced](https://github.com/Markoudstaal/node-red-contrib-discord-advanced) package for Node-Red, to install it go to the "Manage Palette" option and look for the package to install it.

{% include image.html
    img="/assets/hassio-discord/nodered.png"
    title="Node-Red"
    caption="This is where you need to click" %}