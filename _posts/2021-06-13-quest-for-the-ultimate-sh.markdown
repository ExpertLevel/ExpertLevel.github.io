---
layout: post
title:  "Quest for the Ultimate Shell"
date:   2021-06-13 10:00 +0700
categories: blog
author: wesley
---

<div markdown="span" class="alert alert-info" role="alert"><i class="fa fa-info-circle"></i> <b>Note:</b> Shells are made to preference of the user on the otherside of the keyboard, this summarizes my 20-ish year Journey of the 'perfect' shell.</div>

For most of the new folks (new to Linux and/or BSD) this will be the first thing one starts today - as the shell will be your home through all those sleepless nights.

Over the years I’ve worked with an extensive set:<br>
[sh](https://en.wikipedia.org/wiki/Bourne_shell)<br>
[bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell))<br>
[csh](https://en.wikipedia.org/wiki/C_shell)<br>
[ksh](https://en.wikipedia.org/wiki/KornShell)<br>
[tcsh](https://en.wikipedia.org/wiki/Tcsh)<br>
[zsh](https://en.wikipedia.org/wiki/Z_shell)<br>

The one that seems to been missing so far is [Fish](https://en.wikipedia.org/wiki/Fish_(Unix_shell)), perhaps this changes in the future.

My personal shell preference is Zsh and has been for a few years in the beginning raw as a Fish (phun intended) but now combined and weaponized with [Oh-My-Zsh](https://ohmyz.sh) for a year.

So let’s review most of them, and give my opinion based upon where one might be in their career. 

sh/csh can in my opinion pretty much been put in a same group, functional shells working but sometimes limited for that what you need - then you need to write ‘dirty hacks’ however this in many operating systems get’s fixed by symbolic-linking csh to tcsh. 
Currently csh is actively used in NetBSD for one in its “original” shape and not the tcsh shape as the csh is to be considered the “original” BSD shape.

ksh is AT&T’s  or better said [Bell Labs](https://en.wikipedia.org/wiki/Bell_Labs) wonder child, however support on ksh is a bit weird as quoted from the Wikipedia: “KornShell, i.e. ksh2020, a "major release for several reasons" (such as removal of EBCDIC support, dropped support for binary plugins written for ksh93u+ and removal of some broken math functions), was released by AT&T, but is not maintained or supported (by AT&T; wasn't even on release date). “ So this shell isn’t really maintained it appears even through the source code is available on Github which should be considered a “modern-day” platform. One can argue if the ksh2020 is the same ksh or just a hard-fork which should’ve gotten a different name.

tcsh aka csh on steroids. Is a nice and very stable shell for users whom aren’t new to the world of shells and don’t want the ultimate ‘newbie’ experience but are still comfortable with the limitations of a C Shell - however none of these where so big that they couldn’t be overcome for me.

bash is super user friendly and for this reason comes with very newbie friendly Operating Systems like [Ubuntu](http://www.ubuntu.com)   
Mac OSX “recently” (with [Catalina](https://support.apple.com/kb/HT208050) in 2019) made the move of zsh as a default shell instead of bash and users in Big Sur (11.4) are properly warned (as it still exists):

```
goldfinger :: ~ » bash

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
bash-3.2$ exit

goldfinger :: ~ » bash --version
GNU bash, version 3.2.57(1)-release (arm64-apple-darwin20)
Copyright (C) 2007 Free Software Foundation, Inc.
goldfinger :: ~ »
```
Sorry for the small side-step about Mac OSX no longer ‘supporting’ and eventually removing bash from it’s base - Why this sidestep well, It would be my recommended shell for absolute newbies to the world of shells. However the people at Mac appears to think even zsh can meet this requirement or they’re just done with the GPLv3 license, that’s at least my expectations. The bash version included in Mac OSX is “really old” v3.2.57 v.s. v5.1. patch 008 but as said this is to be expected to be due to licensing restraints within the realm of GPL licensing. 

So my recommendation of shells is either:
1. Bash - Keeping in mind that most likely at some point it get’s removed at the Apple OSx base.
2. Zsh - Enhanced with Oh-My-Zsh will give you git integrations too and fancy themes there is one for everyone’s liking for sure.


Both of them would do a great job! Taking my [wife](http://expertlevel.blog/about/elena) as a baseline I would unleash her on Bash sooner than Zsh. 

However she needs to decide for herself what is the best tool, I can only tell her what I like and what I don’t like about various shells this comes from twenty years of ‘dirt’ through various shells. 

I’ll let her at some point in the upcoming future touch both and she can then do a writing about shells from her point of view.

The newbie shell would be Bash in my opinion and more advanced Zsh mainly due to git integrations on a more ‘favorable’ way in my opinion then Bash. People can choose their weapon of choice appropriately. This blog post just summarizes 20 years of various Shells and hopefully now ending up with one I can get even older with perhaps I migrate to Fish with [Oh-My-Fish](https://github.com/oh-my-fish/oh-my-fish) someday who knows. For now I have 0 experience with this shell I've however seen promising demo's. But once you get comfortable with your shell and you forked all your needed functionality into usable functions or extensions once doesn't move towards something new rapidly.
