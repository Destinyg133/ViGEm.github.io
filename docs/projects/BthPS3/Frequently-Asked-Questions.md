# Frequently Asked Questions about BthPS3

Got questions? Who can blame you 😅 we can provide some answers, though! Read on, traveler!

## What Bluetooth hosts are supported?

In short: all of them manufactured within the last decade and running proper stock drivers (means no ScpServer/ScpToolkit, no AirBender, stock as the manufacturer intended). [For details see this article](../Compatible-Bluetooth-Devices).

## What controllers are supported?

This is unfortunately impossible to answer a 100% correctly. These drivers have been designed with compromises in mind. They aim to support the **original genuine Sony SIXAXIS/DualShock 3** (and Navigation, Move) controllers while operating within the realms of possibilities the Microsoft Bluetooth stack offers and allows. The DualShock 3 (or DS3 in short) has been a fairly popular piece of hardware and many clones have arisen over time, some coming close to the quality of the original, some... well, not quite as much. Aftermarket devices spoof (forge) the Hardware Identification Information that Windows sees and the labels and manufacturer notes on the housing itself. There simply is no rock-solid way to properly identify these devices to separate the good from the ugly. That's the inconvenient truth, any other statement would be a wild guess and not facts. [For details see this article](../About-Controller-Compatibility).

**TL;DR:** the genuine Sony hardware, anything else is a nice-to-have that may or may not work.

## Can I use my wireless Keyboard/Mouse/Headphones with this?

Yes, that's the whole purpose of this design 😉 BthPS3 *extends* the existing vanilla Bluetooth stack, it doesn't *replace* it (like ScpToolkit and alike did). This means it can never be as close to the original PlayStation Bluetooth stack (we need to play by Microsoft's design rules, remember?) as other solutions but the trade-off of keeping your stock wireless functionality should be worth it.

## How many devices can I connect at the same time?

There is no definitive answer to that one, as it depends heavily on the Bluetooth host hardware (quality, antenna design, size and position) and the amount of "noise" in your environment (Bluetooth is a fairly "weak" protocol compared to all the other radio chatter that's constantly happening in a common household). Users have reported all sorts of working constellations; like up to 6 controllers connected and working concurrently without any human-noticeable delay. So it's up to you to figure this one out! 😁

## Can it emulate another common controller, like Xbox One?

Controller emulation is *not* the job of these drivers, they provide the plumbing required to get them connected to Windows (and stay connected and keep talk), nothing more, nothing less. Other drivers (which you can find on this site) handle the controller-specific work required.

## Is there any noticeable input lag over Bluetooth?

Another stellar question! With no definite answer 😅 The truthful answer would be: don't know, don't care since it hasn't been measured with scientific equipment. The more down-to-earth answer comes from simple experience and interaction, human to machine: no. You might feel it working better or worse compared to USB, real or placebo. Those who ask this question usually just wanna hear "nope, it's all fine" so that they can move on. Well, there you have it, you can move on now 😘
