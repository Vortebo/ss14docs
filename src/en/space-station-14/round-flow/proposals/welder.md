# The Welder

| Designers | Coders | Implemented | GitHub Links |
|---|---|---|---|
| Vortebo | N/A | :x: No | TBD |

## Overview

The Welder is a roundstart antagonist aimed at evoking the feel of a slasher movie villian. Its goal is to increase the size of its domain while picking off the crew one by one. To this end, it has a variety of powers that exert spooky effects on targeted players. It also has an AI-like spectral mode, facilitating appearing out of nowhere and disappearing around corners, and allowing it to corrupt the controlled part of the station to its will.

## Background

Named after the character in Yahtzee Crowshaw's _Chzo Mythos_ series, the Welder is a character that popped up in SS13 over a decade ago. According to the Goonstation wiki, it was made sometime around 2012, but I swear it must have existed prior to 2010. In any case, it's been removed, re-added, and entirely replaced over the years. This version is partly based on those others, and partly going in a different direction because I misremembered and thought the role had been deleted due to just not being fun, requiring a redesign (apparently the actual reason was spaghetti code).

## Features to be added

### The Welder

The Welder is a roundstart antagonist and a subgamemode. It starts in a random part of maints. The Welder has two major focuses: expanding its domain, and punishing those who transgress its domain. The more (unique?) Spooky Actions performed before a transgressor is killed, the higher the multiplier for the Spooky Points earned upon killing them. Points are used for purchasing additional Spooky Actions and other powers.

The Welder starts in spectral mode, essentially an AI Eye which (initially) only sees the corrupted domain. The corrupted domain is the area the Welder directly controls. Some amount of maints surrounding the Welder's spawn location should start already under its control. The corrupted domain has several important effects. First, it becomes invisible to the AI. Second, any players who enter it become transgressors. Third, neither radio nor suit coordinates work. Finally, any non-holy lightbulbs that get installed in the domain blow up; the explosion shouldn't blow a hole in a wall but should severly slow whoever tried to install the bulb. After the Welder's fourth kill, the corrupted domain looks increasingly spooky. If the entire domain is recovered by the crew, the Welder stops existing.

The Welder is capable of entering corporeal mode, appearing as a Scary Dude. This can only be performed in dark enough areas, and if the Welder is exposed to bright enough light while corporeal, it takes steady damage; at roundstart they shouldn't be able to survive for more than a few seconds, enough to realize and fix their mistake. All other damage types are affected by a damage multiplier which starts at 0x but ramps up exponentially with each hit, though it also cools down quickly after a long enough time without getting hit. The corporeal body can only be healed by returning to spectral form. The Welder has only one movement speed, somewhere between a normal walk and run. It doesn't get any movement penalties. It should create a stomping sound which is only audible for players a few tiles away. The Welder cannot speak locally and just grunts instead.

While corporeal, the Welder can slash lights to break them; doing this adds any resulting dark-enough area to the domain, and also earns Spooky Points. The Welder can only attack transgressors; its attack does a large amount of stun damage (enough to possibly escape after one hit but to be doomed after two), plus bleed. A context-menu action allows the player to harvest a transgressor's soul, a process similar to the Revenant. Doing this is the main way to earn Spooky Points. A successful harvest turns off suit coordinates and (possibly?) prevents revival. The Welder can abandon to spectral mid-harvest, but the would-be victim becomes permanently immune; does so does come with a cool disappearing effect, though. If killed while corporeal, the Welder is banished and can no longer become corporal or use most powers for rest of the round. However, it can ride the evac shuttle to CC for the post-credits stinger, as long as its domain isn't fully removed - this would be basically a glorifed spectator ghost, so maybe they also get dead chat.

In either mode, the Welder needs to be able to see well in the dark, and needs to know what areas are too bright and what are part of its domain. I do not have an interesting visual in mind at this time.

Some possible powers and buffs for the Welder to purchase:
| Power/Buff | Effect | Usable In | Cost | Spooky Action |
|---|---|---|---|---|
| Portals | Place sets of portals within domain; portals are invisible to other players | Spectral | Mid | Yes (when a player goes through one) |
| Spooky Locker | Designate a destination locker within domain that any transgressor will now be bluespaced to when they get shut in a locker. Welder gets non-pop-up notification | Spectral | Mid | Yes (when activated) |
| Far Sight | See some amount of area around transgressors | Spectral | Mid | No |
| Emerge | Corporealize within the indicated locker | Spectral | Mid | Yes |
| Spooky Voice | Speak locally in the voice of any victims. Blood loss effect added, only appears in chat window | Spectral | Low | No |
| Possess | Briefly possess transgressor; victim gets flashbang effect for the duration | Spectral | Mid | Yes |
| Sleep | Makes a victim in a bright enough area fall asleep | Spectral | Mid | Yes |
| Trap | Briefly removes all accesses from a victim | Spectral | Mid | Yes |
| Haunt | A specific victim gets a spooky message | Spectral | Low | Yes |
| Puppet | Make an object say something | Spectral | Low | Yes |
| Manipulate | Make an un-anchored object move | Spectral | Mid | Yes |
| Shhh | Briefly mutes a victim | Spectral | Low | Yes |
| Light Resistance | Survive in the light longer, enabling short excursions to attack victims or increase territory | Corporeal | Mid | No |
| Improved Light Resistance | Enough time to chase someone down a hallway | Corporeal | High | No |
| Run | Movement speed becomes faster than normal run | Corporeal | High | No |
| Listen | Hear everything transgressors hear | Both | Mid | No |
| Boo! | Spectator Boo! action occurs for every transgressor | Both | Low | Yes |
| Mass Corruption | Lights around all transgressors explode, converting area to corrupted domain if possible | Both | High | Yes |
| Illness | All transgressors get the same effect at once. Effect is random (vomit, metallic taste, etc.) | Both | Low | Yes |
| Improved Spooky Voice | Allows speaking over radio | Both | Mid | No |

### The Chaplain

By using their bible on enough of the Welder's victims, the chaplain gains the ability to summon the Welder. Once this ritual is performed, the Welder is unable to return to spectral form for a length of time; for that duration, they also lose any buffs they may have purchased.

After the first or second victim investigated, when the chaplain summons their familiar, they get Cerberus instead of Remilia. The chaplain also gains an ability that lets them temporarily see who among the crew have transgressed, though doing so puts their health just above crit. When enough victims have been investigated to enable the summoning ritual, the bible sprite ought to change to something real evil-looking.

Holy water can be used in a crafting recipe to make holy lightbulbs that, when installed _within_ the corrupted domain, reverts control back to the station.

## Round Resolution

Call shuttle at 40% station takeover?

- Crew major: No domain remains. The happy ending, where the monster is truly defeated and the studio doesn't demand sequels.
- Crew minor: Welder banished, domain remains. The canon ending, where the final girl survives just long enough for the next movie to start.
- Neutral: Other conditions don't get met. I can't think of an analogy.
- Welder minor: no living transgressors. Every character got got, but there's more 20-somethings out there.
- Welder major: >= 50% of station in domain. End of the world, real downer of a movie.

## Game Design Rationale

The Welder is actually a territory control gamemode in disguise. Early Spooky Points are earned by expanding domain, and later abilities decrease the fog of war, increase domain size, and ease travel through enemy territory. Many other abilities are focused on getting victims into the domain and making it hard for anyone to get back out alive. The crew's first counterplays when the Welder is noticed are identifying the domain, preventing additional travel through it, and shrinking its size; directly forcing an armed confrontation with the Welder requires either investigating enough corpses to summon it or a misplay on the Welder's part. Should be sub game mode because X. Should be roundstart because Y.

A serial killer stalking maints is a natural addition to the game. It's already generally accepted that going into maints alone is risking life and limb. The Welder provides additional reason to be cautious about such activities, as well as greater incentive to bring a light source with you if you're intent on going anyway. It should not, however, be too discouraging, as the Welder should be fairly easy to outrun and enough people should be trampsing through its domain that they have plenty of time in the round between transgressing and the Welder actually coming for them.

Intro to this paragraph. The corrupted domain provides increased ambiguity about the cause of a loss of AI cameras and smashed lights. Several of the obtainable powers are also meant to give players pause about e.g. flickering lights, bluespace lockers, and alcoholism. At the same time, many of the powers encourage working together, e.g. being aware of if their coworkers have gone missing or if anyone else is experiencing illness at literally the exact same time (presumably unlikely even if/when virology returns).

The Welder is meant to pick crew members off one by one. To this end, it isn't meant to be particularly robust in combat. Instead, its powerset is meant to encourage the player to both quickly deal with folks who wander into their lair and plan efficient, aggressive actions against their list of targets. A very successful Welder becomes better able to make a lot of noise, but doesn't become any less vulnerable to a clown with a gun.

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
