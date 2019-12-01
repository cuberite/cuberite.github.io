---
layout: post
title: 'Cuberite Newsletter 2019'
discussion-id:
---
Happy holidays everyone! We're approaching the end of 2019 (oh, where did the time go), which means it's time for a long-overdue status update for Cuberite.

General News
------------

 - Cuberite has an official Discord server! Feel free to drop by and say hello. https://discord.gg/76w5J6M
 - Cuberite's [Android app](https://github.com/cuberite/android/releases/download/1.4/cuberite-android.apk) has received a redesign, as well as multiple bug fixes and code cleanups. Devices running Android 4.0 and above are supported.
 - The build process of official Windows downloads, which used to reside on [xoft](https://github.com/madmaxoft)'s home server, is currently being moved to [AppVeyor](https://www.appveyor.com/).
 - Minecraft 1.13 support is partially done, and 1.14 support is planned.
 - Cuberite's website has been restructured slightly, to make it easier to find relevant information. A new "Discuss" page houses information about official communication channels.
 - A few issues related to the forum, such as outdated templates and registrations not working, have been resolved.
 - Analytics are no longer collected from website visitors. Cuberite's Piwik analytics server has been removed.

Cuberite Development
-----------------

In addition to smaller bug fixes and cleanups, these are a few notable changes to Cuberite since the end of 2017:

 - [#4017](https://github.com/cuberite/cuberite/pull/4017): Improve rain simulation
 - [#4041](https://github.com/cuberite/cuberite/pull/4041): Add support for Minecraft 1.12.2
 - [#3959](https://github.com/cuberite/cuberite/pull/3959) [#4038](https://github.com/cuberite/cuberite/pull/4038) [#4050](https://github.com/cuberite/cuberite/pull/4050): Vector parameters
 - [#4053](https://github.com/cuberite/cuberite/pull/4053): Implement horse inventory
 - [#4178](https://github.com/cuberite/cuberite/pull/4178): Make offline UUIDs consistent with vanilla
 - [#4185](https://github.com/cuberite/cuberite/pull/4185): cLightingThread: Faster chunk reading
 - [#4220](https://github.com/cuberite/cuberite/pull/4220): Add unbreaking for armor
 - [#4251](https://github.com/cuberite/cuberite/pull/4251): Rewrite explosion knock back
 - [#4260](https://github.com/cuberite/cuberite/pull/4260): Optimise chunk set
 - [#4272](https://github.com/cuberite/cuberite/pull/4272): Ocelots no longer multiply exponentially
 - [#4341](https://github.com/cuberite/cuberite/pull/4341): Fix directory traversal bug ([CVE-2019-15516](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-15516))
 - [#4390](https://github.com/cuberite/cuberite/pull/4390): Initial support for 1.13 clients (unplayable early state)
 - [#4412](https://github.com/cuberite/cuberite/pull/4412): Fixed crash in hopper while pulling items from blockentity above itself
 - [#4417](https://github.com/cuberite/cuberite/pull/4417): Refactored block-to-pickup conversion

As always, the latest Cuberite updates are available to download on the [homepage](/).

Contribute
-------------

 - If you are interested in developing Cuberite core or plugins, please do not hesitate to join the [forum](https://forum.cuberite.org) or [Discord server](https://discord.gg/76w5J6M). Cuberite development has slowed down a bit due to lack of free time among regular contributors, as well as larger changes in Minecraft 1.13 and 1.14, so any new contributions are greatly appreciated.
 - Feel free to donate to Cuberite through [Liberapay](https://liberapay.com/Cuberite) or [Bountysource](https://www.bountysource.com/teams/cuberite). Donations are used to cover server hosting expenses.