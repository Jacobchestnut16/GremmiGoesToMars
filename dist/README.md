# Gremmi Goes To Mars

A goblin Banished to Mars by a petty kingdom
Gremmi, his name is, has only a few days to prepare for survival or ... be met with certain doom ... on Mars ...
His goals are
Befriend the witch, Unlock portals around Earth, Gather strange supplies, and Cast weird spells

All in this 2D survival fantasy where exile is just the beginning.

Craft. Farm. Fight. And maybe… get even.

## Game Development process:

```mermaid
---
    title: Game commit process
    config:
        theme: dark
---
gitGraph
    commit id: "Store Page"
    branch development
    commit id: "TileMap v1.0"
    commit id: "TileMap v1.1"
    commit id: "TimeCycle v1.0"
    commit id: "TimeCycle v1.1"
    commit id: "TilePallet-Walls v1.0"
    commit id: "TilePallet-Mountain v1.0"
    commit id: "TileMap-Mountain v1.0"
    commit id: "PlantI.F. v1.0"
    commit id: "TileMap-Plant v1.0"
    commit id: "TileMap-Plant v1.1"
    commit id: "TileMap-Plant v1.2"
     
```


main = Steam releases or updates

development = releases or changes to the game. These releases can be found for download in beta downloads (eg. [download](DownloadGame.md), Steam pre-release)


### Time line:

Green = complete

Red = critical path

```mermaid
%%{
    init: {
        'gantt': {
            'leftPadding': 200,
            'barHeight': 25,
            'barGap': 15,
            'topPadding': 60
        },
        'themeVariables': {
            'doneTaskBkgColor': '#2B522EFF'
        }
    }
}%%
gantt
    title Gremmi Goes to Mars - Sandbox Survival Development Beta 1 Timeline
    dateFormat  YYYY-MM-DD
    axisFormat  %b %d
    
    
    section World Foundation
    Tilemap Generation                          :crit, done, a1, 2025-08-14, 1d
    Time Scale / Day-Night Cycle                :crit, done, a2, after a1, 1d
    
    section Minerals/Agriculture
    Stone Mountains                             :crit, done, a4, after a2, 1d
    
    section Plants
    Plants Classes/Maps/Generation              :crit, done, a5, after a4, 0.5d
    Plants Images/Lookup/Grow-animation         :crit, done, a6, after a4, 0.5d
   
    
    section Player Core
    Gremmi Movement                 :crit, b1, after a5, 0.5d
    D&D-style Stat Generation       :b2, after a5, 0.5d
    
    section Game Mechanics
    Boundaries                      :crit, c4, after b2, 0.5d
    Chunking                        :crit, c2, after b2, 0.5d
    
    section Player Interaction
    Inventory System                :crit, b3, after c2, 0.5d
    Resource Interaction/Gather     :b5, after c2, 0.5d
    
    section Refine and release
    Saving & Loading                         :crit, milestone, b4, after b5, 1d
    UI system - BETA V1 OFFICIAL RELEASE     :milestone, release1, after b5, 1d
```

<pre>

Rlease description:

Gremmi Goes To Mars; Stranded on a desolate Red Planet, Fighting to survive.
Learn to grow food.
Collect materials.

</pre>

```mermaid
%%{
    init: {
        'gantt': {
            'leftPadding': 200,
            'barHeight': 25,
            'barGap': 15,
            'topPadding': 60
        },
        'themeVariables': {
            'doneTaskBkgColor': '#2B522EFF'
        }
    }
}%%
gantt
    title Gremmi Goes to Mars - Sandbox Survival Development Beta 2 Timeline
    dateFormat  YYYY-MM-DD
    axisFormat  %b %d
    
        
    section Milestone - extras 1
    Minerals/stone/walls                    :crit, a2 , 2025-08-21, 3d
    Inventory Dumping (Chests, Shelves)     :a1, after a2, 2d
    
    
    section Combat & Entities
    Enemy Entities (AI + Spawning) :d1, after a1, 2d
    Friendly Entities (NPC AI)     :d2, after d1, 2d
    
    section Crafting & Building
    Base Building                  :crit, d6, after d2, 10d
    Crafting - Items/Resources     :crit, d5, after d2, 5d
    Crafting - Spells              :crit, d4, after d5, 4d
    Crafting - Potions             :crit, d3, after d4, 4d
    
    section Refine and release 2
    UI system - BETA V2 OFFICIAL RELEASE     :milestone, release2, after d6, 5d
    
    section Advanced Simulation
    Background Task System (Queued Tasks)   :e1, after release2, 8d
    Task Automation Logic                   :e2, after e1, 6d
```
<pre>

Rlease description:

Gremmi Goes To Mars; Stranded on a desolate Red Planet, Fighting to survive.
Build your base.
Fend off enemies.
Make friends with Martian life.


Advanced Simulation //planned for BETA V2
Includes task automation like auto mining, auto farming, etc.

</pre>