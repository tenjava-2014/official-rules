Rules
==============


This repo contains the rules for the July 2014 ten.java contest. You can use commit/line comments to comment on rule changes or PR additions/changes for consideration. Changes here will be merged into the wiki.

Repository Rules
================

Maven skeleton
--------------

* We will be providing a Maven-based repository skeleton to all repositories.
  * There is no requirement to use our template but we think it will be helpful for those who are unfamiliar with Maven.   
  * We will be providing tutorials and other resources in due course.
* Current progress on this skeleton is available [here](https://github.com/tenjava/repository-template)
  * If you have an idea for the template, submit a pull request or create an issue ticket!

Before the contest
------------------

* Access will be removed.
* Our Maven skeleton (see above) will be pushed over all repositories.

During the contest
------------------

* Access will be restored to the repositories in time for the contest.
* Developers should push to their repository regularly during the contest time.
  * We want to observe your activity throughout the contest, not just one big commit at the end. 
  * If you're committing and pushing less than twice per hour while working then you're doing it wrong.
* Developers must use the provided repository.
* Developers may not accept pull requests during the contest time.
* Binaries should not be pushed to the repository.
* You may use the wiki functionaliy or make use of markdown files to document your plugin.

After the contest
-----------------
* Access to the repositories will be revoked until judging is complete.
* You're welcome to continue working on the project either in our repository or by making your own once the judging is over.


Development rules
=================

Code
----

* Code must use the Bukkit API. Code written that depends on APIs provided by forks of (Craft)Bukkit or by external dependencies (e.g. Vault, libraries not available in Bukkit/CraftBukkit etc) cannot be accepted.
  * Plugins may use NMS/OBC.
* Your plugin cannot depend on any other plugins.
  * Your plugin can use the libraries available to (Craft)Bukkit (see [pom.xml](https://github.com/Bukkit/CraftBukkit/blob/master/pom.xml#L54) for more info) at runtime.
* Code absolutely must compile. Unlike last year, we are making no efforts whatsoever to fix compile errors. Plugins that do not compile will result in disqualification.
* Be aware that we'll be running plugins on the latest CraftBukkit beta version. Ensure that any NMS/OBC imports use the correct package name and that you are using API available in the latest beta at the time of start of the contest.
* Submissions that are deemed malicious will not be judged and the developer will be disqualified. We may remove the repository in question. We may publicly discuss the submission.
* Plugins may not include code written outside your selected timeslot or written by another person.
  * If we suspect that code not written during the contest time or code written by another person is deliberately present in the final source of the entry and the entry would be awarded a winning place, we may request proof in the form of recorded video if we feel the VCS commit logs do not provide enough information. Failure to provide sufficient proof may result in disqualification.

Resource packs
--------------

* Resource packs can greatly enhance a player's experience. We're allowing resource packs this year, as long as your use of them meets the following:
  * Plugins should not 100% rely on the use of a resource pack. Packs should exist only to add to the experience.
  * We will judge your plugin primarily with your resource pack (but may disable it to check the above point).
  * Resource packs should be uploaded under the releases section of your repository as a ZIP file. Packs must be made solely in the timeslot.
  * Since the focus for ten.java is your idea and code, we are **allowing the use of external assets only in resource packs** as long as the creator's license enables you to use them. Block model changes are not possible in 1.7.x so assets include sounds, textures, music, fonts etc.
  * Bear in mind that we are not judging your use of a resource pack and they should solely be used to add to the experience.
  * Any externally sourced assets you use in the resource pack must have been made prior to the contest start time (Sat Jul 12 2014 00:00 UTC). You must provide sources for any external assets you choose to use.

Compilation
-----------

* You can target your code at Java 6, 7 or 8. All 3 versions will be available on our build server (we'll be using Oracle's versions, FYI).
* All submissions must use Maven. If you choose to modify our template, you must have a default goal available since we won't be supplying any on our build server.
  * While we cannot accept projects which do not use any build tool, it is up to the organizer's personal discretion as to what we do with projects using Ant, Gradle or other build tools. Maven is highly preferred but we don't want to disqualify people because they used a different tool if it's not too much trouble for us to build.

Other participants
==================

* You're welcome to watch other streams (including the official stream) during the contest time(s) and you're welcome to give advice to other participants. We have no problem with people helping others and will encourage it throughout the event.
* Please ensure you use your own ideas and own code for your submission. Copying concepts from other participants is not okay.

Teams
=====

* Per the "Code" section, we are not allowing code written by anyone other than the participant to be submitted in the contest. This means teams are not permitted for this contest, though we do want to look into a team-based contest in the future.
