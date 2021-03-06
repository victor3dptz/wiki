---
layout: page
title: PowerMac 6100 Graphics Card Benefits
---

![Logo](/mac/powermac6100/img/07graphics.gif) This page describes additional benefits to adding a video card to your Power Mac 6100.

### Intro

In addition to the speed bump, there are two more benefits to adding a video card: support for a second monitor, and support for additional resolutions.

Before you read any of this, I should add the caveat that I can only provide data for the monitors that I have in front of me. Some of my findings my not be replicable if you don't have a comparable or larger monitor. Mine is an Apple Multiple Scan 15.

### Adding a second monitor

It's as easy as plugging it in.

Although my main monitor is now plugged into the DB-15 port on the back of the HPV card, the original HDI-45 port is still there on the motherboard, and so is the HDI-45 to DB-15 adapter that came with my Performa. If I plug in another monitor and restart my machine, I get two desktops. If you haven't done this before, it's definitely worth seeing. I use the **Monitors Control Panel** to make the logical positions of the monitors match their physical positions on my desk:

![1](/mac/powermac6100/img/monadj.gif)

For example, my main monitor sits on top of my computer, and my second monitor sits off to the right. When I move the mouse pointer off the right side of my main monitor, it appears on the left side of my second monitor.

![2](/mac/powermac6100/img/mondiag.gif)

I can also set things up like this, so that I need to move the mouse to the corner of the screen before it switches desktops. This is useful if I need to run the mouse up and down the edge of the screen (on a scroll bar, for example), and I don't want to wander over to the other desktop accidentally.

You can rearrange the logical positions of the monitors by dragging their icons around. Note that the icons' sizes represent the resolution settings of the monitors. In this example, Monitor 2 is set to 1024 x 768, and Monitor 1 is set to 832 x 624. You can also control which monitors holds your menu bar by dragging that around. And last, having more than one monitor finally gives you a reason to click the **Identify** button. This makes a big number pop up on each monitor, in case you've forgetten which one is which.

Besides being really cool, what's this good for? I use it for putting together Web pages, such as this one. I have my Netscape running on my main monitor, and my text editor running off to the right. That way I can keep the html on one screen while I watch the effect of the changes on the other.

I occasionally have access to a few different monitors aside from my primary Apple Multiple Scan 15. I recently acquired a used SuperMatch 17-T that I'm going to give to my brother soon, and sometimes I use a **really** old, el cheapo, single resolution VGA monitor that I pulled out of the computer graveyard at my parent's company. It's worth about $50. Maybe. But it's great as a second monitor. For further information on how to hook up a VGA monitor to a Mac, read on:

### Connecting a VGA Monitor

I had to try a few adapters before I found one that would do everything I wanted. For example, to connect my cheap VGA monitor, I had to find an adapter that would set the sense pins for 640x480 @ 60 Hz. After several trips to the computer store, I finally brought the dang monitor with me and tried all the adapters until I found one that worked. With any adapters that didn't support the refresh rate I wanted (and many didn't), all I got was a rapidly scrolling image, or else no image at all.

The one that worked turned out to be the very affordable MacView adapter by Sony. It has two sets of DIP switches that allow you to trick your Mac into thinking it's hooked up to just about any monitor you can buy. I bought it for $11.99 from the Creative Computers Superstore. I suppose that the more expensive wheel-type adapters would also do the trick.

### Screen resolutions

The other nice thing adding a video card is that they all support more resolutions than DRAM video:

Desired resolution | None (640K) | 7100 HPV (1MB) | 7100 HPV (2MB) | 8100 HPV (2MB) | 8100 HPV (4MB) | AV Card (2MB) | Nubus (Various)
------------------ | ----------- | -------------- | -------------- | -------------- | -------------- | ------------- | ---------------
512x384 | 16 bit | 24/32 bit | 24/32 bit | 24/32 bit | 24/32 | 24/32 bit | Varies
640x480 | 16 bit | 16 bit | 24/32 bit | 24/32 bit | 24/32 bit | 24/32 bit | Varies
640x870 | N/A | 8 bit | 8 bit | 8 bit | 8 bit | 8 bit | Varies
800x600 | N/A | 16 bit | 24/32 bit | 24/32 bit | 24/32 bit | 24/32 bit | Varies
832x624 | 8 bit | 16 bit | 24/32 bit | 24/32 bit | 24/32 bit| 24/32 bit | Varies
1024x768 | N/A | 8 bit | 16 bit | 16 bit | 24/32 bit | 16 bit | Varies
1152x870 | N/A | 8 bit | 16 bit | 16 bit | 24/32 bit | 16 bit | Varies 

* The maximum bit depth of the Portrait monitor is 8 bits.

To get 1024x768 on my Apple Multiscan 15, I chained two adapters together. I used the MacView adapter discussed above along with a generic Mac-monitor-to-PC adapter. So the cable chain goes:

``Mac HPV card-->MacView adapter-->Mac-PC adapter-->Apple monitor``

which is ugly. Furthermore, it sticks out the back of the computer about 6 inches. But it works.

Chaining adapters is only one way to get 1024x768 on the Apple Multiscan 15. It tricks the monitor into thinking it's hooked up to a PC, and it tricks the Mac into thinking it's driving a VGA monitor. I know there are adapters out there that will do this directly. Griffin Technologies makes a model that has Mac connectors on both ends and switches to allow various settings, but I've not personally used any of their products.

One might ask why this dual chicanery is necessary, i.e. why Apple doesn't permit the user to select this option directly, since both the HPV card and the monitor support it. Here's my theory: 70 Hz is suboptimal for 1024x768, since the Mac standard is 75 Hz. Apple has a reputation for high quality video, and doesn't want to give users an option that doesn't look great. Therefore, this option is only available if you're driving a VGA monitor and can blame the flicker on that. Personally, I'd rather have the option without resorting to chaining adapters up the yin-yang. On the other hand, it seems like my monitor is really, really close to being able to support 1024x768 @ 75 Hz. Anyone know why Apple chose not to go the extra mile on this one?

