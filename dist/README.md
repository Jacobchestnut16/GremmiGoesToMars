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
    title Gremmi Goes to Mars - Sandbox Survival Development
    dateFormat  YYYY-MM-DD
    axisFormat  %b %d
    
    
    section Milestone 1 - World Foundation
    Tilemap Generation                          :crit, done, a1, 2025-08-14, 2d
    Plants                                      :a6, after a1, 3d
    Minerals/stone/walls                        :a4, after a1, 2d
    Tree Generation                             :a5, after a6, 2d
    Time Scale / Day-Night Cycle                :crit, a2, after a1, 1d
    
    section Milestone 2 - Player Core
    Gremmi Movement                 :crit, b1, after a2, 0.5d
    D&D-style Stat Generation       :b2, after b1, 0.5d
    Inventory System                :crit, b3, after b1, 2d
    Resource Interaction/Gather     :crit, b5, after b3, 1d
    Saving & Loading                :crit, milestone, b4, after b3, 2d
    
    section Refine and release
    UI system - BETA V1 OFFICIAL RELEASE     :milestone, c1, after b4, 5d
    
    section Milestone 3 - extras 1
    Inventory Dumping (Chests, Shelves) :milestone, f1, after c1, 4d
    
    section Milestone 4 - Combat & Entities
    Enemy Entities (AI + Spawning) :d1, after c1, 8d
    Friendly Entities (NPC AI)     :d2, after d1, 6d
    
    section Milestone 5 - Crafting & Building
    Base Building                  :crit, d6, after c1, 10d
    Crafting - Items/Resources     :crit, d5, after c1, 5d
    Crafting - Spells              :crit, d4, after d5, 4d
    Crafting - Potions             :crit, d3, after d4, 4d
    
    section Refine and release 2
    UI system - BETA V2 OFFICIAL RELEASE     :milestone, c2, after d6, 5d
    
    section Milestone 6 - Advanced Simulation
    Background Task System (Queued Tasks) :e1, after c2, 8d
    Task Automation Logic                 :e2, after e1, 6d
```
