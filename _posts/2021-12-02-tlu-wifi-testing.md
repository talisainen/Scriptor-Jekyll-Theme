---
layout: post
title: "Experimenting with unreliable network connections (draft)"
description: ""
date: 2022-12-02
feature_image: images/2022-12-02-tlu-wifi-testing/zyxel-lte-wifi-router.png
# feature_image: images/2022-12-02-tlu-wifi-testing/temi-and-double.jpg
tags: [experiment]
---

In case you missed it, in one of our [previous publications](https://candid-rabanadas-e1b0db.netlify.app/tlu-workshop) we discussed troubles with wireless network coverage in Tallinn University. Such issues lead to poor user experience and may have a dramatic effect on the perception of telepresence robots in general, therefore we decided to run a series of tests. More on that below.

<!--more-->

We decided not to include Ohmni into this experiment, as we experienced issues in far better network conditions are that that would be a waste of time.

Although this was not a quantitative experiment, and its results should be interpreted as guidelines for a more serious research at most there were some interesting findings.

The experiment was run during evening time on Friday, when Tallinn University Wi-Fi network is not overloaded and in addition to that we used three different access points:

- 5 GHz network created by 2nd generation iPhone mini with Tele2 mobile network provider
- 2.4 GHz network created by iPhone 11 Pro with Tele2 mobile network provider
- 2.4GHz and 5 GHz networks created by Zyxel LTE2566-M634 4G LTE Mobile WiFi Router (the one on the first image) with Tele2 mobile network provider


{% include image_caption.html imageurl="images/2022-12-02-tlu-wifi-testing/temi-and-double.jpg" title="" caption="Temi and Double discussing TLU Wi-Fi" %}

Not to go into details, but we found Temi to be less reliable and more prone to losing connection, however it might be partially compensated by its higher self-sustainability and using offline maps when moving.

We also found a peculiar bug that we were unable to interpret: for some reason connection to Zyxel (both 2.4 GHz and 5GHz) and iPhone 11 Pro disables network icon and menu on Double 3 robot. On the contrary, iPhone SE and local Wi-Fi do not have such effect and we never encountered it before.
