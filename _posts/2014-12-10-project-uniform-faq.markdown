---
title: "Project UniREform: ESEA Season 17 LAN Team Skins FAQ"
date: 2014-12-10 12:00:00
author: thesupremecommander
categories:
- project-info
tags:
- ESEA
- FAQ
- UniREform
img: unireform.png       #place image (850x450) with this name in /assets/img/blog/
thumb: unireform.png    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/
---
Due to the overwhelming response we've had for these skins, we have decided to create an FAQ to answer the most common questions that people have about them.

<!--more-->

#### Where did the idea for team skins come from?

Surprisingly, it wasn't our idea originally! This concept was used a long time ago in [eXtelevision's cast of the ESEA Season 7 LAN finals](http://youtu.be/KpDIfoyiMTk).

The idea was revived with uberchain's famous video *NEVER 4GET*:

<iframe width="560" height="315" src="//www.youtube.com/embed/WPVJtgdgQIM?rel=0" frameborder="0" allowfullscreen></iframe>

This video was created in the aftermath of froyotech's defeat at the hands of Exertus eSports (now Team eLevate), which broke the roster's flawless streak of victories spanning over 5 seasons. The video garnered lots of attention and praise, particularly for its use of custom team skins for both froyotech and Exertus in the video's dramatic final scene. I privately contacted uberchain about the possibility of creating a set of skins for use during major events, and the project went on from there.

#### When was this project done?

Talks about the project occurred since *NEVER 4GET* was released, but no concrete work was done except for investigating the technical potential behind such an idea. Work to actually implement the technical framework required occurred in the last half of September and released as a StatusSpec module in October shortly before the GXL LAN. The actual skins were pitched by concepts released Monday during the week of ESEA LAN. Once approval was obtained, the player skins were finished within a span of 4 days for 80 skins with the help of other concept artists and reskin artists.

#### How did the skins work?

The skins were actually all client-side. This means that they were only visible for the official broadcast on the ESEA Orange stream, and not visible on the game server for the players or the SourceTV broadcast server for other spectators.

The technical framework supporting the skins was the [player models module of StatusSpec](https://github.com/fwdcp/StatusSpec#player-models), which would override the model for a player with another specified model based on the plugin's configuration. The replacement team skin models are simply the regular TF2 player models rehexed to use different materials, whose textures are then edited to create the altered appearance.

#### What was the rationale behind how the skins were generally designed (for each in-game team and for each competing team)?

At the beginning of the project, I communicated to uberchain that the skins not only needed to be visually distinct for each competing team, but also needed to fit in with the in-game team colors of Team Fortress 2 for the purposes of familiarity.

uberchain then delivered the following concepts to me (which were shared with both the TeamFortress.TV staff and the teams for their approval):

<div id="concepts" class="carousel slide">
    <!-- Indicators -->
    <ol class="carousel-indicators">
        <li data-target="#concepts" data-slide-to="0" class="active"></li>
        <li data-target="#concepts" data-slide-to="1"></li>
        <li data-target="#concepts" data-slide-to="2"></li>
        <li data-target="#concepts" data-slide-to="3"></li>
        <li data-target="#concepts" data-slide-to="4"></li>
        <li data-target="#concepts" data-slide-to="5"></li>
        <li data-target="#concepts" data-slide-to="6"></li>
        <li data-target="#concepts" data-slide-to="7"></li>
        <li data-target="#concepts" data-slide-to="8"></li>
        <li data-target="#concepts" data-slide-to="9"></li>
        <li data-target="#concepts" data-slide-to="10"></li>
        <li data-target="#concepts" data-slide-to="11"></li>
        <li data-target="#concepts" data-slide-to="12"></li>
        <li data-target="#concepts" data-slide-to="13"></li>
        <li data-target="#concepts" data-slide-to="14"></li>
        <li data-target="#concepts" data-slide-to="15"></li>
    </ol>

    <!-- Wrapper for slides -->
    <div class="carousel-inner" role="listbox">
        <div class="item active">
            <img src="/assets/img/other/unireform/concepts/001.jpg" alt="The Rules [Team Colour]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/002.jpg" alt="The Rules [Team Colour]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/003.jpg" alt="The Rules [Team Colour]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/004.jpg" alt="The Rules [Team Colour]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/005.jpg" alt="froyotech [RED]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/006.jpg" alt="froyotech [BLU]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/007.jpg" alt="Team eLevate [RED]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/008.jpg" alt="Team eLevate [BLU]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/009.jpg" alt="Classic Mixup [RED]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/010.jpg" alt="Classic Mixup [BLU]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/011.jpg" alt="Street Hoops [RED]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/012.jpg" alt="Street Hoops [BLU]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/013.jpg" alt="What's Left? [Final Checks]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/014.jpg" alt="What's Left? [Final Checks]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/015.jpg" alt="What's Left? [Final Checks]">
        </div>
        <div class="item">
            <img src="/assets/img/other/unireform/concepts/016.jpg" alt="Thank You [Very Much]">
        </div>
    </div>

    <!-- Controls -->
    <a class="left carousel-control" href="#concepts" role="button" data-slide="prev">
        <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="right carousel-control" href="#concepts" role="button" data-slide="next">
        <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
</div>

*Team eLevate is incorrectly referred to as eLevate eSports in these concepts.*

Hopefully these concepts give you a little more insight into the general design of the skins. For more information, you'd have to contact uberchain.

#### Are there posters for these skins?

Yes, there are! uberchain designed some sweet posters for each of the teams in both RED and BLU variants, which you can get in both 4K and 1080p below:

![froyotech](/assets/img/other/unireform/posters/1920x1080/froyotech_RED.jpg)
*download froyotech team poster: [RED 3820x2148](/assets/img/other/unireform/posters/3820x2148/froyotech_RED.jpg), [RED 1920x1080](/assets/img/other/unireform/posters/1920x1080/froyotech_RED.jpg), [BLU 3820x2148](/assets/img/other/unireform/posters/3820x2148/froyotech_BLU.jpg), [BLU 1920x1080](/assets/img/other/unireform/posters/1920x1080/froyotech_BLU.jpg)*

![Team eLevate](/assets/img/other/unireform/posters/1920x1080/elevate_RED.jpg)
*download Team eLevate team poster: [RED 3820x2148](/assets/img/other/unireform/posters/3820x2148/elevate_RED.jpg), [RED 1920x1080](/assets/img/other/unireform/posters/1920x1080/elevate_RED.jpg), [BLU 3820x2148](/assets/img/other/unireform/posters/3820x2148/elevate_BLU.jpg), [BLU 1920x1080](/assets/img/other/unireform/posters/1920x1080/elevate_BLU.jpg)*

![Classic Mixup](/assets/img/other/unireform/posters/1920x1080/classicmixup_RED.jpg)
*download Classic Mixup team poster: [RED 3820x2148](/assets/img/other/unireform/posters/3820x2148/classicmixup_RED.jpg), [RED 1920x1080](/assets/img/other/unireform/posters/1920x1080/classicmixup_RED.jpg), [BLU 3820x2148](/assets/img/other/unireform/posters/3820x2148/classicmixup_BLU.jpg), [BLU 1920x1080](/assets/img/other/unireform/posters/1920x1080/classicmixup_BLU.jpg)*

![Street Hoops eSports](/assets/img/other/unireform/posters/1920x1080/streethoops_RED.jpg)
*download Street Hoops eSports team poster: [RED 3820x2148](/assets/img/other/unireform/posters/3820x2148/streethoops_RED.jpg), [RED 1920x1080](/assets/img/other/unireform/posters/1920x1080/streethoops_RED.jpg), [BLU 3820x2148](/assets/img/other/unireform/posters/3820x2148/streethoops_BLU.jpg), [BLU 1920x1080](/assets/img/other/unireform/posters/1920x1080/streethoops_BLU.jpg)*

There is an additional ESEA LAN poster available:
![ESEA LAN](/assets/img/other/unireform/posters/1920x1080/esealan_wallpaper.jpg)
*download ESEA LAN poster: [1920x1080](/assets/img/other/unireform/posters/1920x1080/esealan_wallpaper.jpg)*

#### Can I get these skins?

Yes! All skins will be posted on the [Project UniREform GitHub](http://github.com/fwdcp/UniREform). For skins from this LAN, you will be able to download them from the [LAN release page](https://github.com/fwdcp/UniREform/releases/tag/esea-lan-s17).

#### How will I be able to use these skins?

If you just want to play with these skins in normal gameplay, you should be able to install them as a client-side mod. Theoretically, these models might not work like that because they're rehexed to use different model paths and texture paths, but you can always copy over the modified textures if that is the case.

If you want to install these for use on your server, please be advised that the brands used in these skins are owned by the respective teams (who have graciously given us the ability to create, use, and release them), so you should seek permission before using them publicly (i.e. on a server). Assuming you've cleared that, you can use a plugin like [TF2 Model Manager](https://forums.alliedmods.net/showthread.php?t=164630) on your server to replace models. Due to how the StatusSpec player models module mimics the functionality of TF2 Model Manager client-side, the models included in the VPKs should be fully compatible and ready-to-go for such use.

If you want to use them to create art, feel free to just use the released models! The models should be fully compatible with [Source Filmmaker](http://www.sourcefilmmaker.com/). We request that you be appropriate and respectful in your artwork.

If you want to replace the models the same way we did in the cast (for the purposes of creating videos of the teams in action, for example), you can use StatusSpec to replace the models for the team. We will release the `custommodels.res` file that was used in the cast to replace each player with their appropriate team model.

#### Will this project be continued for future competitive events?

We intend to do so, though hopefully under much less of a time constraint than we had here. Stay tuned.

#### Will these skins ever be released as items for the game?

In a perfect world, yes, that would be cool. Unfortunately, there are several large hurdles in the way:

* As they currently stand, the skins are simply reskinned versions of the TF2 characters and not separate models attached to the players, so some conversion would be required to submit them as items.
* We would need to work on an agreement with the teams to release these as items since they own the brand and should be receiving the revenue generated from any sales of such items.
* Realistically, while it is possible for such skins to be released through the normal Steam Workshop process, it's not likely to happen as simply as that, and most likely it would only happen through a comprehensive agreement on competitive affairs with Valve.

However, we are keenly interested in this and would love to see it happen someday.

#### Where can I submit my feedback?

We have created [a Google Forms survey](http://goo.gl/forms/T6RpJH4jyJ) which you can fill out to address the specific feedback that we have. In addition, you can talk to either me or uberchain via Steam, Twitter, or TeamFortress.TV.

#### Who should I direct my appreciation to?

uberchain is really the one person who you should thank - without her, none of this would have ever happened.

Here's the general credits for the project:

* *Concept Artists:* uberchain, kichizone, Fudge
* *Reskin Artists:* uberchain, The Scurvy Orange, Fudge, DillyDong, Colteh
* *Special Thanks:* Mikahvi, ZeroAE, Liz, SedimentarySocks, [TeamFortress.TV](http://teamfortress.tv/), [TF2 Texture Improvement Project](http://tf2tip.maxofs2d.net/), [Team eLevate](http://elevate.gg/), [froyotech](http://www.froyotech.tv/), [Classic Mixup](http://play.esea.net/teams/51672), [Street Hoops eSports](http://play.esea.net/teams/74241)

#### How do I ask other questions?

You can contact me via Steam, Twitter, or TeamFortress.TV - I'll be happy to answer questions to the best of my ability.
