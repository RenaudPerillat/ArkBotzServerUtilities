# ArkBotzServerUtilities

Ark mod providing tools for the roleplay, the storyline and the management of the Ark Botz Server.

## About this project

This project is intended to provide the sources of the ArkBotzServerUtilities mod used on Ark: Survival Ascended game.
The sources shall be used with ASA devkit, the version currently developped on is 92.35.286.826107.

The baked mod is available on Curse Forge, [here](https://www.curseforge.com/ark-survival-ascended/mods/ark-botz-server-utilities).

## Contents

In this project, you will find:

- ArkBotzUtilities: Blueprint utility functions, such as logger, ini parameter reader, custom command management.
- ArkBotzPlayerTracker: Record players position on the map and send it using http post request to a server.

## Documentations

### ArkBotzPlayerTracker

Inherits from SaveGameActorTickable.
Added as Server Extra World Singleton Actor Class.

Configuration
```ini
[ArkBotzPlayerTracker]
EnableLogs=True
LogsLevel="Info"
PositionRecordIntervalSeconds=1.0
SendToServerIntervalSeconds=10.0
ServerURI="https://example.com"
```
