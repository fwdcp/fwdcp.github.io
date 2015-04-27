---
layout: post          #important: don't change this
title: "Behind the Scenes: TF2 Production"
date: 2015-04-27 12:00:00
author: thesupremecommander
categories:
- blog                #important: leave this here
- behind the scenes
tags:
- AdvSpec
- NodeCG
- production
- StatusSpec
- TeamFortress.TV
- UniREform
img: btsproduction.png       #place image (850x450) with this name in /assets/img/blog/
thumb: btsproduction.png    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/
---
One of the most critical parts of a competitive scene's existence is its production - the process of taking a game and creating an immersive experience for viewers that allows them to share in its excitement. Game productions are the main way that currently interested people enjoy the game and newly interested people are encouraged to follow, and TF2 is no exception.

<!--more-->

### The Basics

At its core, a production is composed of the game itself and then the many additions made to the game in order to suitably display it to viewers. In most productions (especially for online events), the team accomplishing this includes a cameraman and one or more casters. Smaller teams may have both of these functions performed by one person, while larger productions usually have a play-by-play commentator who describes the action, a color commentator who provides valuable insights into the game, and a separate cameraman who focuses on picking the best players and areas to display. Getawhale, one of the more prevalent play-by-play commentators of the scene, described his role as follows:

> My experience doing a cast typically involves preparation, which involves looking at the teams and players that will be playing and taking down notes for while I cast. I show up, I talk to whoever my co-caster is (sometimes do a specific plan, sometimes more casual), and then we [commentate]. I stay in contact with my camera person or production person throughout the cast and keep chat open so I'm able to take in information while I talk.

In addition to these people directly involved with the game, major organizations like TeamFortress.TV employ a vast support staff behind-the-scenes. This support staff includes producers, who incorporate various graphics and other elements into a production; schedulers, who organize casts based on the availability of cameramen and casters; graphics designers, who create a streamlined and consistent interface to the stream; developers, who create and maintain programs used in production; and promotion staff, who raise awareness of the various events being covered by social media, articles, videos, and other similar efforts. In a typical online production, as many as 20 people may be directly involved with making it happen in the different stages of the process.

### Hacking the Game (Literally)

![StatusSpec](/assets/img/other/bts/production/statusspec.jpg)

One of the main problems with producing TF2 content is the limitations of the game itself, which include "a bad HUD, SourceTV bugs, and none of the features that are in CS:GO or Dota," as put by developer Matt "bluee" McNamara. The natural solution for this problem has been the use of extensive modification of the game via client plugins.

While plugins have been present throughout TF2's existence, such as the omnipresent [P-REC](https://bitbucket.org/olegko/p-rec) by Orange, the controversial [OpenPlugin](https://github.com/CasualX/OpenPlugin) by Casual, and even the production-oriented [Spectate Helper](https://github.com/miek/spectate_helper_plugin) by Miek, bluee's [AdvSpec](https://github.com/MattMcNam/advspec) was the first major spectator-oriented plugin, augmenting the game HUD significantly with features like player outlines (allowing every player in the game to be seen via a team-colored glow through walls) and a medigun info panel (showing the status of each team's medigun and ubercharge). His work was later incorporated into and extended via projects like [Spec Tools](https://teamfortress.tv/thread/17283/spec-tools) (developed by Gentleman Jon) and [StatusSpec](https://github.com/fwdcp/StatusSpec) (developed by Forward Command Post). In addition, specially configured servers (most commonly found in European games) can provide a live feed of major game events (via plugins developed by Arie).

These extensions have allowed the game to be stretched far beyond its limits for the purposes of spectating. In more recent productions, many different features from minor fixes for problems like HUD freezes due to the game's buggy pause system to major additions like in-game mods have all been incorporated. Even more major changes are currently being tested in production, such as smooth camera transitions between players and remote camera control. The latter feature is in itself a major advancement for production, according to producer Alex "dashner" Pylyshyn:

> There is a trend that is starting to pick up pace in terms of separating camera men and producers. We had a lot of good technology that simply never got used because most of our camera men were only capable of camming; anything else kind of overwhelmed them and distracted them from their job… now that we’ve found out how to separate camera and producer, our productions have improved substantially.

### A Revolution in Live Graphics

![NodeCG](/assets/img/other/bts/production/nodecg.jpg)

Another huge leap for TF2 production came in the form of live graphics. Traditionally, broadcasts have relied on major systems such as CasparCG or more on-the-fly solutions like manually editing graphics via Photoshop during the production itself. In an attempt to create a simpler system for usage in productions by VanillaTV, one of the major broadcasting organizations at the time, atmo created the VTV overlay system, which utilized Web technologies to display and manipulate graphics controlled by a separate dashboard. This system would be later adapted for usage by TeamFortress.TV and by Tip of the Hats (an annual fundraising livestream event).

bluee (who had worked on some of the graphics for TeamFortress.TV) approached Alex "Lange" Van Camp (who worked on the Tip of the Hats system) with the idea of creating a generalized framework out of the separate overlay systems, which would allow for live graphics to be easily created by Web technologies as compared to Flash (required for CasparCG). Thus, the project [NodeCG](https://github.com/nodecg/nodecg) was born, and has grown in usage not only in TF2 productions but in many other contexts, like the major Twitch stream Dan's Gaming.

NodeCG has become a crucial component in productions for many reasons, most significantly simple integration with [Open Broadcaster Software](https://obsproject.com/), the streaming application used by the vast majority of TF2 streamers. In addition, the relative ease of creating graphics has allowed live graphics to be easily adapted to the changing requirements of production.

### Creating a Storyline

![ESEA Season 18 LAN final intro](/assets/img/other/bts/production/eseaintro.jpg)

A good production cannot only focus on the game itself, but also must show the background behind the game which makes the game important. Such is the role of promotional materials like trailers and posters for major events. As explained by Ness "uberchain" Delacroix, the designer leading such efforts:

> With a "feel" or a flavour, people get a good taste about what's to come - and you gotta be sure that what they see, what they taste in that instance is what's going to get them to stop by and see what it is they just tasted. When you're generating hype for an event, you always want to make sure it leaves people wanting to see more, mostly for who you're making it for but also enough that people wonder what's going down so they check it out.

The most significant graphic additions have been [Project UniREform](https://github.com/fwdcp/UniREform), which created in-game uniforms to denote top teams for major events, and event marker videos, such as [the outro to theGXL Universe 2014](https://www.youtube.com/watch?v=A3c2b6KRyHE) and [the intro to the ESEA Season 18 LAN finals](https://www.youtube.com/watch?v=zk6DBEGZfHI). These additional components to productions have earned general acclaim by the community, helping to enrich the connection between the games and the scene as a whole.

In addition to promotional materials, recent coverage of major LAN events has aimed to expand on-site coverage in order to help viewers connect with the environment and participants of a LAN. TeamFortress.TV admin Jay "mana" Kim, who helped organize on-site coverage for the recent ESEA Season 18 LAN, shared his thoughts on the importance of such coverage:

> In terms of quality, a presence from the LAN is incredibly important; it adds an enormous background and foreground to how attractive the stream is, as well as building hype of the event (in my opinion, i52, and the CSGO ESL majors prove the strength of presenting the LAN in person on stream).

### The Future

It is clear that TF2 productions have grown significantly since their inception. However, there is still significant room to grow, with productions still lacking in several areas.

One of the biggest issues is in the nature of TF2 productions as volunteer efforts. For most people involved, TF2 production is at best a hobby requiring significant time investment. Describing the situation, dashner noted:

> ESEA LAN was me, [sound producer] airon, and uberchain all sacrificing a lot of time for free to make [the stream] happen. I was paid [by ESEA] but only for the active streaming work I did on the weekend... I'm not sure where we'll be in a year. It's scary to think about - at some point everyone who volunteers their time will move on. I was fortunately there to fill the void that Lange's departure left, but once I go I have no clue who will take over.

Such a problem is of major importance, but production organizations like TeamFortress.TV have been able to recover from major figures stepping down, with others (both old and new) filling the roles that they vacate. As part of this cycle, TeamFortress.TV recently began an aggressive effort to recruit staff to continue the evolution of its live graphics and spectator plugins, and also to find new and better ways to enhance the promotion of the game.

In any case, it's clear: with the top level of the scene becoming even more competitive, it's an exciting time to be a producer and a viewer.

mana summarizes the situation best:

> There's a lot to a streamed cast than it may seem on the surface. Streams have come an incredibly long way thanks to huge efforts of everyone involved in streaming technologies. The right pickups on TeamFortressTV have created a formidable potency of backend code and assets that literally has done things we would've never imagined before. Experience has culminated to handle what we've made into enhancing the stream. [The recent ESEA Season 18 LAN] has been, by far, the best production we've done, integrating not only an improved stream, but also on site video and photos, which is unprecedented. I'm very proud of the production team and its accomplishments; to hear that we rival some major streams in quality is a testament to the incredible collaborative power that the team has.
