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

The corrupted domain is the area the Welder directly controls. Some amount of maints surrounding the Welder's spawn location should start already under its control. The Corrupted Domain has several important effects. First, it becomes invisible to the AI. Second, any players who enter it become transgressors. Third, it is the focus of spectral mode powers. Finally, it is the primary area where the Welder will become corporeal. As the Welder's kill count increases, the corrupted domain looks increasingly spooky (starting after the fourth kill).

The Welder starts in spectral mode, which is basically an AI Eye which initially can only see the corrupted domain. There are several powers and buffs available for purchase which can only be used in spectral mode:
- Portals: Invisible to other players, these portals are used to disorient any soul unfortunate enough to enter the corrupted domain.
- Spooky Locker: The destination locker that a transgressor can be teleported to through the use of the Spooky Locker Grab 'Em and Pull 'Em Into the Bad Place ability.
- Far sight: See some amount of area around transgressors
- Teleport to a non-spooky locker, making it spooky: you teleport to the indicated locker near to a transgressor. Become corporeal within of the locker. Like. You right click on the locker. Y'know?
- Spooky voice: speak locally (originating from Eye) in the voice of any victims. Blood loss effect is added to victim's voice.
- Possession: victim gets the flashbang effect for the duration
- ?

As for corporeal mode. Can only exist where it's dark enough; takes damage from being in the light. Also turns visible/vulnerable to everyone when exposed to light. Damage multiplier starts at 0x but that ramps up exponentially with each hit, though it also cools down quickly after a long enough time without getting hit. Can only heal by switching back into spectral mode. Slashing lights adds any resulting dark-enough area to the domain, and also gets you some Spooky Points. Can only attack transgressors. Attack does like 75% stun damage per hit plus bleed. Specific action to harvest a transgressor's soul, ala Spooky Ghost Antag. Gets you hella Spooky Points. Can abandon to spectral mid-harvest but would-be victim becomes permantently immune; does come with a cool disappearing effect though. Become visible and vulnerable during kill time. If killed in corporeal, you lose. RIP you. You do respawn at CC for the post-credits stinger, though! Only one movement speed, somewhere between normal walk and run; doesn't get any movement penalties. Cannot speak locally, just grunts.

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

Grind up a Bible to get a new thing called Holyase. Used to make lightbulbs that, when installed within the corrupted domain, reverts control back to the station. Normal lightbulbs, like, immediately blow up. Or something.




## Game Design Rationale

The Welder is actually a territory control gamemode in disguise.

Should be sub game mode because X. Should be roundstart because Y.

## Roundflow & Player interaction

welder

Part of text in "You are The Welder" says "Punish those who have transgressed your realm" or whatever and that's part of communicating not to bother trying to kill anyone else.

## Administrative & Server Rule Impact (if applicable)

welder

## Further developments

welder

# Technical Considerations

welder
