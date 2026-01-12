# The Welder

| Designers | Coders | Implemented | GitHub Links |
|---|---|---|---|
| Vortebo | N/A | :x: No | TBD |

## Overview

The Welder is a roundstart antagonist aimed at evoking the feel of a slasher movie villian. Its goal is to increase the size of its domain while picking off the crew one by one. To this end, it has a variety of powers that exert spooky effects on targeted players. It also has an AI-like spectral mode, facilitating appearing out of nowhere and disappearing around corners, and allowing it to corrupt the controlled part of the station to its will.

## Background

A brief history of the Welder in various SS13 servers. This design is going in a slightly different direction because I misremembered some of this history and figured I had to reinvent the wheel, oops.

## Features to be added

### The Welder

The Welder is a roundstart antagonist and a subgamemode. It starts in a random part of maints. The Welder has two major focuses: expanding its domain, and punishing those who transgress its domain. The more Spooky Actions performed before a transgressor is killed, the higher the multiplier for the Spooky Points earned upon killing them. Points are used for purchasing additional Spooky Actions and other powers. Welder needs to be able to see in dark - and differentiate b/w light and dark - in either mode.

The corrupted domain is the area the Welder directly controls. Some amount of maints surrounding the Welder's spawn location should start already under its control. The Corrupted Domain has several important effects. First, it becomes invisible to the AI. Second, any players who enter it become transgressors. Third, radio doesn't work (neither do coords?). Any non-holy lightbulbs that get installed in the domain blow up - should not blow a hole in a wall but should severly slow whoever tried to install the bulb. As the Welder's kill count increases, the corrupted domain looks increasingly spooky (starting after the fourth kill). If entire domain is gotten rid of by crew, that fully kills the Welder.

The Welder starts in spectral mode, which is basically an AI Eye which initially can only see the corrupted domain. There are several powers and buffs available for purchase which can only be used in spectral mode:
- Portals: Invisible to other players, these portals are used to disorient any soul unfortunate enough to enter the corrupted domain.
- Spooky Locker: The destination locker that a transgressor can be teleported to through the use of the Spooky Locker Grab 'Em and Pull 'Em Into the Bad Place ability.
- Far sight: See some amount of area around transgressors
- Teleport to a non-spooky locker, making it spooky: you teleport to the indicated locker near to a transgressor. Become corporeal within of the locker. Like. You right click on the locker. Y'know?
- Spooky voice: speak locally (originating from Eye) in the voice of any victims. Blood loss effect is added to victim's voice.
- Possession: victim gets the flashbang effect for the duration
- ?

As for corporeal mode. Can only enter where it's dark enough; takes damage from being in the light. Damage multiplier (for damage other than light) starts at 0x but that ramps up exponentially with each hit, though it also cools down quickly after a long enough time without getting hit. Can only heal by switching back into spectral mode. Slashing lights adds any resulting dark-enough area to the domain, and also gets you some Spooky Points. Can only attack transgressors. Attack does like 75% stun damage per hit plus bleed. Specific action to harvest a transgressor's soul, ala Spooky Ghost Antag. Gets you hella Spooky Points. Turns off coords. Prevents revival (seems rude but like)? Can abandon to spectral mid-harvest but would-be victim becomes permantently immune; does come with a cool disappearing effect though. If killed in corporeal, Welder is banished and can no longer be corporal or use most powers for rest of the round, but can ride the evac shuttle to CC for the post-credits stinger (if domain isn't fully removed) (basically a glorifed spectator ghost, so maybe they also get dead chat). Only one movement speed, somewhere between normal walk and run; doesn't get any movement penalties. Stompy boi (probably falls off very quickly with distance though). Cannot speak locally, just grunts.

Powers/buffs specific to corporeal mode:
- Improved Light Resistance: survive in the light longer so you can bust out of a locker and drag your sleeping victim into the darkness. Passive ability but you get the idea.

Also, powers/buffs usable from both modes:
- YOu're Beaing --watched-- heard: Hear everything transgressors hear
- Spooky Locker Time: When (any transgressor or specific victim?) gets in a locker, they get bluespaced to your designated spooky locker. Gives Welder a notification when it happens.
- Make Lights Flicker: Makes lights around (everyone or specific victim?) flicker.
- Pew Pew Lights: Makes lights around everyone explode, converting area to corrupted domain if possible. Costs a lot.
- Illness: all transgressors get the same effect at once. Effect is random (vomit, metallic taste, etc.)
- Make 'em be asleepy times: ya
- Begins the spooky messages: specific victim will now start getting spooky messages every so often
- Locked doors: specific victim loses all access for a period of time
- Improved spooky voice: can also speak over radio

### The Chaplain

Chaplain gets something to do! Summon welder can happen after examining five victim's bodies? Means they get called to crime site like detective, which would be neat. Summoning ritual forces welder to be corporeal at location, and can't spectralify for a bit, so, y'know. Shoot them.

Transgressors can be seen be chaplain if chaplain does something or other that probably puts them at or near crit. And probably only the ones actually in view at the time. 

Grind up a Bible to get a new thing called Holyase. Used to make lightbulbs that, when installed within the corrupted domain, reverts control back to the station.

## Round Resolution

Call shuttle at 40% station takeover?

- Crew major: No domain remains. The happy ending, where the monster is truly defeated and the studio doesn't demand sequels.
- Crew minor: Welder banished, domain remains. The canon ending, where the final girl survives just long enough for the next movie to start.
- Neutral: Other conditions don't get met. I can't think of an analogy.
- Welder minor: no living transgressors. Every character got got, but there's more 20-somethings out there.
- Welder major: >= 50% of station in domain. End of the world, real downer of a movie.

## Game Design Rationale

The Welder is actually a territory control gamemode in disguise. Early Spooky Points are earned by expanding domain, and late-round abilities decrease the fog of war, increase domain size, and ease travel through enemy territory. Many other abilities are focused on getting victims into the domain and making it hard for anyone to get back out alive. The crew's first counterplays when the Welder is noticed are identifying the domain, preventing additional travel through it, and shrinking its size; directly forcing an armed confrontation with the Welder requires either investigating enough corpses to summon it or a misplay on the Welder's part. Should be sub game mode because X. Should be roundstart because Y.

A serial killer stalking maints is a natural addition to the game. It's already generally accepted that going into maints alone is risking life and limb. The Welder provides additional reason to be cautious about such activities, as well as greater incentive to bring a light source with you if you're intent on going anyway. It should not, however, be too discouraging, as the Welder should be fairly easy to outrun and enough people should be trampsing through its domain that they have plenty of time in the round between transgressing and the Welder actually coming for them.

Intro to this paragraph. The corrupted domain provides increased ambiguity about the cause of a loss of AI cameras and smashed lights. Several of the obtainable powers are also meant to give players pause about e.g. flickering lights, bluespace lockers, and alcoholism. At the same time, many of the powers encourage working together, e.g. being aware of if their coworkers have gone missing or if anyone else is experiencing illness at literally the exact same time (presumably unlikely even if/when virology returns).

## Roundflow & Player interaction

welder

Part of text in "You are The Welder" says "Punish those who have transgressed your realm" or whatever and that's part of communicating not to bother trying to kill anyone else.

## Administrative & Server Rule Impact (if applicable)

welder

## Technical Considerations

### UI

fs

### Other

hbh
