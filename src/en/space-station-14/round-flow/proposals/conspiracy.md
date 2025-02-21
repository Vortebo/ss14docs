# Conspiracy gamemode

| Designers | Implemented | GitHub Links |
|---|---|---|
| Vortebo | :x: No | TBD |

## Overview

<!-- A very short, maybe three sentence summary of what this proposal is about. A high level "overview" or "what this adds". -->
A new team antagonist that encourages non-violent, stealth-y, social gameplay in order to suceed. Conspiracy designates several players as conspirators who must work together to accomplish a series of increasingly difficult tasks. Conspirators and crew alike are made to operate in an initially low-information environment and must use social deduction to work out who they can trust.

## Background

<!-- Summarize any information that is needed to contextualize the proposed changes, e.g. the current state of the game.

Also link any relevant discussions on Discord, GitHub, or HackMD that are relevant to the proposal. -->

So, we've got solo antags, we've got group antags, we've got conversion antags. But like, our group and conversion antags are all kinda shooty shooty bang bang? I think? Like they don't _have_ to be but. So, yeah.

## Features to be added

<!-- Give a description of what game mechanics you would like to add or change. This should be a general overview, with enough details on critical design points that someone can directly implement the feature from this design document. Exact numbers for game balance however are not necessary, as these can be adjusted later either during development or after it has been implemented, but mention *what* will have to be balanced and what needs to be considered when doing so. -->

Reiterate the overview. Will probably work best without other antags running at the same time.

### Conspirators

Some number of conspirators are selected; same selection pool as for traitor/thief (may need to make sure they're not all in one department or too evenly spread out) (though honestly it might be kinda funny if it's all one department). One person is the head conspirator. They get all the goals and have to tell the rest of the group what those goals are. Every conspirator gets told how many total of them there are, and also gets either a clue to one other conspirator (just department, department and like first initial) or just gets told who one other person is.

The conspirators must complete a series of tasks and then escape to centcomm alive and unrestrained. Major victory when that happens. Minor victories when at least one level two task is completed and/or some number of conspirators make it to centcomm. Crew victory when every conspirator is dead or detained. Tasks come in (three?) difficulties. Complete (three?) level one tasks to move to level two. Two levels twos to level three. X level three to finish the series. Level 1 explicitly requires every conspirator to participate, to make sure people come together; they should be things that are reasonably innocuous in isolation / could be done by anyone. Level 2 should escalate: things that _maybe_ normally would happen but would raise eyebrows in the best of circumstances. Level 3 is crimes.

**Conspirator Goals**

Level 1  

- Everybody hugs the captain (3x times?)
- Graffitti [word] outside [department]. Everyone must contribute one letter
- Everybody must possess X number of [item]
  - Items could include medkits,
- Hang out in/near [department] together and scream
- Everyone flushes themselves in a disposals thing
- Everyone plays a song in the same band
- ?

Level 2
- 50% of hallways must be covered in liquid
- Everyone has all access
- Switch/rename beacons
- Move [object] from [department A] to [department B]
- Stockpile X number of [item]
  - Different from level 1 goal bcuz
- ?

Level 3
- Weld crewmembers [person 1] - [person ?3?] in the same closet, alive
  - Maybe not specific crew members cuz I can see RNG / round circumstances having the potential to make that arbitrarily difficult
  - Space the closet? Though given how easily trapped crew members could bring down entire conspiracy if let go, followup probably doesn't need to be specified
- Everybody eats one of the captain's organs
- Place four hamburgers in the vault
- Team EVA outing!
- ?

### Crew

The goal of the crew is to arrest (not kill) the conspirators. X minutes into the round (15 - 30 minutes after conspirators are selected and given their goals), centcomm sends an announcement:

> Based on our sophisticated probabilistic models, we have determined that certain individuals are working together to subvert ...something. Please identify them and bring them in for questioning.

Also, a fax gets printed out on the bridge saying exactly how many conspirators there are and giving a clue about one of them.

## Game Design Rationale

<!-- 
Consider addressing:
- How does the feature align with our [Core Design Principles](../space-station-14/core-design/design-principles.md) and game philosphy?
- What makes this feature enjoyable or rewarding for players?
- Does it introduce meaningful choices, risk vs. reward, or new strategies?
- How does it enhance player cooperation, competition, or emergent gameplay?
- If the feature is a new antagonist, how does it fit into the corresponding [design pillars](../space-station-14/round-flow/antagonists.md)?
-->

Part of the goal is to have a slower-burn antagonist, one that has less potential for sudden large jumps in chaos (versus a traitor setting off a bomb). This way crew as a whole can like do their jobs n stuff? Detective? Idk. Words are hard. Like, it should eventually get chaotic, but in a more controlled way. Also, going for paranoia.
Want to incentivize antagonists to do as little damage as possible so they can complete every task. Should be hard to actually get escape shuttle called while still maintaining cover.

Kinda want to encourage the detective as an important element of a crew victory.

## Roundflow & Player interaction

<!--
Consider addressing:
- At what point in the round does the feature come into play? Does it happen every round? How does it affect the round pace?
- How do you wish for players to interact with your feature and how should they not interact with it? How is this mechanically enforced?
- Which department will interact with the feature? How does the feature fit into the [design document](../space-station-14/departments.md) for that department?
-->

## Administrative & Server Rule Impact (if applicable)

<!--
- Does this feature introduce any new rule enforcement challenges or additional workload for admins?
- Could this feature increase the likelihood of griefing, rule-breaking, or player disputes?
- How are the rules enforced mechanically by way the feature will be implemented?
-->

# Technical Considerations

<!--
- Are there any anticipated performance impacts?
- Does the feature require new systems, UI elements, or refactors of existing ones?
- For required UI elements, give a short description or a mockup of how they should look like (for example a radial menu, actions & alerts, navmaps, or other window types)
-->
