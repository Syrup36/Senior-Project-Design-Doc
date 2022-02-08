---
id: HWrtgiodOlHQRimHlYaMF
title: Systems
desc: ''
updated: 1644329634793
created: 1643737940449
---
*last updated {{fm.updated}}*

## Gameplay

Core gameplay would be a top-down, 3D "platformer." Movement is currently analogous to that of Animal Crossing. The player would traverse the small world to find their friends.


The flow of the game, from start to finish, is modeled below:
```mermaid
    flowchart TB;
        A>Intro Cutscene]-->B[Tutorial];
        B-->C{Player Explores};
        C-->D[Player finds a Friend];
        D-->E[Player talks to the Friend];
        E-->C;
        C-->|Once All Friends are Found|F>Final Cutscene];
        F-->G>End Credits];     
```

Exploring the world could consist of small, non-punishing platforming sections as well as a few small puzzles (potentially, I'm still thinking about this).

## Difficulty

As this game is meant to be a medium for me to display my findings, I am aiming for the game to be completely approachable for novice/casual players. There are no current plans for other difficulties.

The game is meant to be a completely relaxing experience, though ~~there may be optional challenges available~~. 
> *(Update: There will be none. Developing these "challenges" would take too much time)*

There is no way to lose the game - there are no lives, there is no punishment for falling off obstacles, and there are no penalties for taking your time.

## World/Map Design

The graph below is a hypothetical map of the play area:

```mermaid
    flowchart LR

    subgraph Campsites
        direction LR
        C[Campsite/Player Spawn]---O[Other Campsite]
    end

    subgraph Lake
        direction TB
        L[Lake]---W[Waterfall]
        L---CA[Cave]
    end

    subgraph Woods
        direction TB
        F[Forrest]
    end

    subgraph Trail
        direction TB
        H[Hiking Trail]---I[Top of Hill]
    end

    Woods---Campsites
    Lake---Campsites
    Campsites---Trail
```