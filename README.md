Rules
==============


This repo contains the rules for the July 2014 ten.java contest. You can use commit/line comments to comment on rule changes or PR additions/changes for consideration.

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
