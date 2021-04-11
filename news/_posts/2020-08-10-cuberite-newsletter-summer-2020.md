---
layout: post
title: 'Cuberite Newsletter Summer 2020'
discussion-id: 3306
---
Hello all Cuberite fans - it's been about 6 months since the last 
update, so it's about time to let you know the current status of the 
project as well as what's gone on since the last update!

General News
------------

 - In general, the Cuberite infrastructure has had a bit of an overhaul. 
   A new dedicated server has been commissioned and most services 
   rebuilt to run as docker containers on this new server. Hopefully 
   this should lead to more uptime and a lower operating cost.
 - As part of the infrastructure upgrade, the build server has been 
   replaced. Production builds now use a version-controlled container 
   for consistency and to make upgrades easier. As a result, old updater 
   scripts or versions of the Cuberite app that did not use Cuberite's 
   [canonical download URIs](https://cuberite.org/download-links/) will 
   no longer work.
 - Binary builds for Mac are now once again being produced and are 
   available for download fom the website. FreeBSD builds remain 
   unavailable due to a lack of build slaves.
 - Before the new server could be activated, the old email system for 
   the forum failed. If you didn't get notifications for this period, 
   don't worry as the problem has now been resolved.
 - As part of the upgrade to the new system, emails from the forum are 
   now sent from noreply@forum.cuberite.org rather than 
   forum@cuberite.org as before.
 - Public demo servers are now available and you can connect on 
   eu.demo.cuberite.org or us.demo.cuberite.org depending on your 
   preferred location. Server contents are regularly reset and uptime is 
   not guaranteed. Please see the 
   [website](https://cuberite.org/demoservers/) for more information.
 - Progress for protocol versions greater than 1.12 is encouraging, and 
   Cuberite now accepts connections from 1.13 clients, although the 
   fundamental changes required for implementing all the new features 
   are still incomplete, as yet.

Development News
----------------

 - Cuberite has updated to C++17, allowing use of the new language and 
   standard library features in the project. As a result, the minimum 
   compiler versions are now clang 6 and GCC 7. 
 - The CMake system has also been reworked, so a newer version of CMake 
   is required. CMake 3.13 is required, but 3.17+ is advised to take 
   advantage of LTO and unity builds.
 - Since the last update, development effort has been coming on slowly 
   but surely, with 174 PRs merged since the last update. The changes 
   include:
   - [#4080](https://github.com/cuberite/cuberite/pull/4080): 
     Use unique_ptr to manage Block Entity Lifetime
   - [#4347](https://github.com/cuberite/cuberite/pull/4347): 
     Lock hopper when powered by redstone
   - [#4476](https://github.com/cuberite/cuberite/pull/4476): 
     Prevent container item duplication
   - [#4485](https://github.com/cuberite/cuberite/pull/4485): 
     Silk touch pickaxe drops grass block
   - [#4490](https://github.com/cuberite/cuberite/pull/4490): 
     Use LastSentPos for mob spawn packet in 1.11+
   - [#4493](https://github.com/cuberite/cuberite/pull/4493): 
     Introduce recipe book functionality
   - [#4502](https://github.com/cuberite/cuberite/pull/4502): 
     Remove leading slash from command block commands
   - [#4505](https://github.com/cuberite/cuberite/pull/4505): 
     Fix armor protection
   - [#4508](https://github.com/cuberite/cuberite/pull/4508): 
     Fix unloading of chunks that contain player entities
   - [#4509](https://github.com/cuberite/cuberite/pull/4509): 
     Prevent arrows from sinking into the ground
   - [#4518](https://github.com/cuberite/cuberite/pull/4518): 
     Lua API for spectating entities
   - [#4525](https://github.com/cuberite/cuberite/pull/4525): 
     Pickup spawn improvements
   - [#4538](https://github.com/cuberite/cuberite/pull/4538): 
     Add protocol mob ID remapping
   - [#4546](https://github.com/cuberite/cuberite/pull/4546): 
     Fix nether mob spawning
   - [#4563](https://github.com/cuberite/cuberite/pull/4563): 
     Implement wither skeletons
   - [#4580](https://github.com/cuberite/cuberite/pull/4580): 
     Replace buckets to the selected hotbar slot
   - [#4586](https://github.com/cuberite/cuberite/pull/4586): 
     Sent experience on respawn
   - [#4610](https://github.com/cuberite/cuberite/pull/4610): 
     Remove switch statements from cItemFoodHandler
   - [#4620](https://github.com/cuberite/cuberite/pull/4620): 
     Falling blocks can now be spawned at any position
   - [#4626](https://github.com/cuberite/cuberite/pull/4626): 
     Add Block Handlers for new blocks
   - [#4627](https://github.com/cuberite/cuberite/pull/4627): 
     Wolves and mooshrooms are passive mobs
   - [#4646](https://github.com/cuberite/cuberite/pull/4646): 
     Bindings: Allow coercion between Vector3 subtypes
   - [#4650](https://github.com/cuberite/cuberite/pull/4650): 
     Using super
   - [#4660](https://github.com/cuberite/cuberite/pull/4660): 
     Observers
   - [#4661](https://github.com/cuberite/cuberite/pull/4661): 
     Implement glowing redstone ore
   - [#4665](https://github.com/cuberite/cuberite/pull/4665): 
     Fix washing away of redstone mechanisms
   - [#4684](https://github.com/cuberite/cuberite/pull/4684): 
     Unify 1.8 and 1.9
   - [#4715](https://github.com/cuberite/cuberite/pull/4715): 
     Use Vector3 for cLineBlockTracer and cBlockTracer
   - [#4740](https://github.com/cuberite/cuberite/pull/4740): 
     Minimise string copying in logging code
   - [#4817](https://github.com/cuberite/cuberite/pull/4817): 
     Add emeralds to generation
 - Thanks to all the new contributors this period, as we now have 9 new 
   entries in the CONTRIBUTORS file:
   - GefaketHD
   - ion232 (Arran Ireland)
   - maxluchterhand1
   - MaxwellScroggs
   - mBornand
   - MeMuXin
   - morsmordere (Anzhelika Iugai)
   - TooAngel
   - Xenoxis

Contribute
----------

 - If you are interested in developing Cuberite's core or plugins, 
   please do not hesitate to join the [forum](https://forum.cuberite.org) 
   or [Discord server](https://discord.gg/76w5J6M).
 - Cuberite no longer accepts donations through the Bountysource 
   platform due to unethical behaviour by the present owners of the 
   service.
 - If you wish to contribute monetarily, please do use
   [Liberapay](https://liberapay.com/Cuberite). Any contribution is very
   much welcomed.

Cuberite Team
