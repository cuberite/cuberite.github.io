---
layout: post
title: 'August/September 2017 Newsletter'
discussion-id: 3020
---
This is the Cuberite newsletter for August/September 2017. It's been a while since the last update, but the project has still been busy, with many new features, bugfixes and community developments.

Project News
------------

 - Development reaches the 2000 milestone. The main Cuberite repository has reached both 2000 stars and 2000 merged Pull Requests on [GitHub](https://github.com/cuberite/cuberite/stargazers)
 - Cuberite was the subject of a [popular post on Hacker News](https://news.ycombinator.com/item?id=15070192) where a lively discussion brought many new interested users to the project
 - Cuberite now has a [Liberapay team](https://liberapay.com/Cuberite) as an alternative to Bountysource. Liberapay is a free and open source recurrent donations platform based in France. It has lower fees than Bountysource, so more of your money will be put to good use, and as an open platform shares the mission of Cuberite
 - Upcoming developments planned for the near future include a fully rebuilt build system, for faster and more expansive builds, as well as greater reliability. A new email system for team members and a matrix homeserver are also planned

Development Focus
-----------------

As well as regular feature development, bugfixes and code cleanup, there have been several major improvements to Cuberite recently:

 - [#3908](https://github.com/cuberite/cuberite/pull/3908): 1.12.1 Support by @Bond-009 was merged, and 1.12.2 support is planned 
 - [3864](https://github.com/cuberite/cuberite/pull/3864): Protocol level chunk sparsing for faster load times was implemented by @peterbell10
 - [3869](https://github.com/cuberite/cuberite/pull/3869): The Forge handshake was implemented by @satoshinm, opening the possibility for plugins to behave as server-side mods compatible with Forge
 - [3871](https://github.com/cuberite/cuberite/pull/3871): UUIDs are now represented as a native class inside the code, allowing for improved validation and better interfaces in the Lua API
 - Other code cleanup projects are ongoing, including replacing integer coordinate arguments with Vectors throughout the project \([3874](https://github.com/cuberite/cuberite/pull/3874)\)
 - Compilation was also fixed on newer compilers, as well as debug mode on ARM and BSD
 - Upcoming pull requests include [scoreboards](https://github.com/cuberite/cuberite/pull/3953), and [books](https://github.com/cuberite/cuberite/pull/3877)

Anything Else
-------------

 - Please donate to Cuberite through [Liberapay](https://liberapay.com/Cuberite) or [bountysource](https://www.bountysource.com/teams/cuberite). Server costs are currently covered by generous community contributions, however additional funds for team members would be very much appreciated
 - If you are interested in developing cuberite core or plugins, please do not hesitate to join in on the [Forum](https://forum.cuberite.org) or IRC \(#cuberite on freenode\) , where we would be glad to help you out
