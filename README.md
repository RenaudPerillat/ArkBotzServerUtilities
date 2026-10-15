# ArkBotzServerUtilities

Ark mod providing tools for the roleplay, the storyline and the management of the Ark Botz Server.

## About this project

This project is intended to provide the sources of the ArkBotzServerUtilities mod used on Ark: Survival Ascended game.
The sources shall be used with ASA devkit, the version currently developped on is 92.35.286.826107.

The baked mod is available on Curse Forge, [here](https://www.curseforge.com/ark-survival-ascended/mods/ark-botz-server-utilities).

## Contents

In this project, you will find:

- Utilities: Blueprint utility functions, such as logger, ini parameter reader, custom command management, diagnostic widget.
- MaxWayPointUpdate: Allow to modify the maximum number of waypoint that can be used.
- TabletTool: Item providing quest system to players, administrative tools to game masters, lore item.

## Documentations

### Logger

It is possible to attached a logger component for diagnostics.
The logger can be configured using commands only.

#### Command

```
AdminCheat ScriptCommand ArkBotz <DedicatedSection> SetLogEnabled True
AdminCheat ScriptCommand ArkBotz <DedicatedSection> SetLogLevel Info
```

### Diagnostic widget

Widget that is attached to admin players through a primal buff that allow to diagnose state of variables when required.

### MaxWayPointUpdate

Buff attached to players.
Can be configured using commands only.
Has a logger component attached.

#### Command

```
AdminCheat ScriptCommand ArkBotz MaxWaypointUpdate ShowConfiguration
AdminCheat ScriptCommand ArkBotz MaxWaypointUpdate SetLogEnabled True
AdminCheat ScriptCommand ArkBotz MaxWaypointUpdate SetLogLevel Info
AdminCheat ScriptCommand ArkBotz MaxWaypointUpdate SetMaxWaypoints 20
```

### TabletTool

Primal Item, singleton to manage item for each player (give at spawn, remove at death).
**CAREFUL: Item can be dropped from the inventory.**

Can be configured using using commands only.
Has a logger component attached.

#### Command

```
AdminCheat ScriptCommand ArkBotz TabletTool SetLogEnabled True
AdminCheat ScriptCommand ArkBotz TabletTool SetLogLevel Info
```

