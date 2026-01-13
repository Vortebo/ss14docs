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
| Emerge | Corporealize within a locker, regardless of light level | Spectral | Mid | Yes |
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
| Open Door | Can open any door | Both | Low | Yes (when spectral and seen by a transgressor) |

In general, powers ought to have cooldowns.

### The Chaplain

By using their bible on enough of the Welder's victims, the chaplain gains the ability to summon the Welder. Once this ritual is performed, the Welder is unable to return to spectral form for a length of time; for that duration, they also lose any buffs they may have purchased.

After the first or second victim investigated, when the chaplain summons their familiar, they get Cerberus instead of Remilia. The chaplain also gains an ability that lets them temporarily see who among the crew have transgressed, though doing so puts their health just above crit. When enough victims have been investigated to enable the summoning ritual, the bible sprite ought to change to something real evil-looking.

Holy water can be used in a crafting recipe to make holy lightbulbs that, when installed _within_ the corrupted domain, reverts control back to the station.

## Game Design Rationale

The Welder is actually a territory control gamemode in disguise. Early Spooky Points are earned by expanding domain, and later abilities decrease the fog of war, increase domain size, and ease travel through enemy territory. Many other abilities are focused on getting victims into the domain and making it hard for anyone to get back out alive. The crew's first counterplays when the Welder is noticed are identifying the domain, preventing additional travel through it, and shrinking its size; directly forcing an armed confrontation with the Welder requires either investigating enough corpses to summon it or a misplay on the Welder's part.

A serial killer stalking maints is a natural addition to the game. It's already generally accepted that going into maints alone is risking life and limb. The Welder provides additional reason to be cautious about such activities, as well as greater incentive to bring a light source with you if you're intent on going anyway. It should not, however, be too discouraging, as the Welder should be fairly easy to outrun and enough people should be trampsing through its domain that they have plenty of time in the round between transgressing and the Welder actually coming for them.

In order to be properly spooky, it should be difficult to metagame the Welder's existence in a round. It should provide cover for other antagonists, and other antags and in-game occurences should provide cover for it. The corrupted domain provides increased ambiguity about the cause of a loss of AI cameras and smashed lights. Several of the obtainable powers are also meant to give players pause about e.g. flickering lights, bluespace lockers, and alcoholism.

Many of the Welder's powers should encourage working together, e.g. being aware of if their coworkers have gone missing or if anyone else is experiencing illness at literally the exact same time (presumably unlikely even if/when virology returns).

The Welder is meant to pick crew members off one by one. To this end, it isn't meant to be particularly robust in combat. Instead, its powerset is meant to encourage the player to both quickly deal with folks who wander into their lair and plan efficient, aggressive actions against their list of targets. A very successful Welder becomes better able to make a lot of noise, but doesn't become any less vulnerable to a clown with a gun.

I have tried to write the powers in a way that prevents them from being spammed sequentially in the Welder's domain without anyone seeing them to artificially bump up the point multiplier. They are generally inherently noticeable, require or are highly likely to be seen by at the very least a transgressor, or naturally lend themselves to being used for going after a transgressor anyway and hence would be saved for the actual kill attempt. Passive powers, or powers like speaking that are only useful if they can be used at will, don't count towards the bonus.

## Roundflow & Player interaction

The Welder is a subgamemode because if it's the only thing happening, the slow ramp-up could lead to the round feeling like a green shift to most players. It's also liable to be very noticeably the Welder if no one else is generating chaos; while many powers should decrease metagameability, their pattern of escalation would be easily picked out. The slow ramp-up is also why Welder should be roundstart; beginning in the middle of an already chaotic station, with an armed crew, is a good way for the Welder to get shot to death by the first would-be victim.

It should be very difficult for a Welder to be friendly, as it can't talk (in its own voice), looks mean, and has powers that should push it towards violence. That said, a player could opt to de-prioritize killing in favor of just kinda messing with people. This is not necessarily a bad thing, as it should still disrupt the round, other antagonists will be active, and in order to be able to get powers in the first place the Welder _does_ need to kill someone at some point.

The departments most likely to have frequent or direct interactions with the Welder are engineering, security, and service. Engineers walking through maints to set up solars are probably going to be the most frequent first victims of a Welder. Due to the Welder's ability to just not let itself be in a fight, security is not likely to be actively engaging it for the bulk of a round, but will be important when the crew actively attempts to defeat it. Service will also be prominent, via the chaplain investigating and summoning the Welder.

## Administrative & Server Rule Impact (if applicable)

The Welder is disincentivized from causing excessive damage, as it only benefits from player death via its soul-harvesting power, and lesss existing station means less space to grow the domain into. Early evac would reduce the amount of time it has to grow its powers.

A player deciding to help the Welder would potentially make it much easier for it to get powerful more quickly than the station can react to. This would, I think, be as likely as for a crew-aligned player to try to help any other antag, and resolvable via the same in- and out-of-game methods.

## Technical Considerations

Unsure
