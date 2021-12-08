# Core Protect

## Overview
---
CoreProtect is a spigot plugin designed for anti-griefing servers. It logs nearly *all* world interactions -- players opening doors, looting chests, breaking and placing blocks; TNT blowing up blocks, water and lava flow, etc. Logs include time, the acting player or entity, and give the ability for staff to [roll back](#rollback) any logged event. Per CoreProtect's [Spigot page](https://www.spigotmc.org/resources/coreprotect.8631/):

> CoreProtect is a fast, efficient, data logging and anti-griefing tool. Rollback and restore any amount of damage. Designed with large servers in mind, CoreProtect will record and manage data without impacting your server performance.

If you are going to take any action based on information you gained from core protect, you should screenshot relevant information with `F2`. 

!!! info
	Try to minimize the duplication of items through rolling back chests. Do not roll back stolen items, but instead try to retrieve them (if possible). 

## Contents
---
1. [Commands](#Commands)
	- [inspect](#Inspect)
	- [lookup](#Lookup)
	- [rollback](#Rollback)
	- [restore](#Restore)
	- [undo](#Undo)
1. [Parameters](#Parameters)
1. [Further Reading](#FR)

## Commands
---
### `inspect`
Usage: `/coreprotect inspect` or `/co i`

**Inspect** allows you to see what and when a player or entity committed an action. Left-clicking a block allows you to see actions done directly on that block while right-clicking allows you to see actions done on adjacent blocks.

### `lookup`

Usage: `/coreprotect lookup` or `/co l`

- [Parameters](#Parameters)

Lookup displays the logs of player an entity actions according to paramenters entered in the command. All parameters are optional, but if you are able to be specific, do so -- it will reduce the otherwise large amount of logs you must look through.

### `rollback`
Usage: `/coreprotect rollback` or `/co rb`
 
- [Parameters](#Parameters)

Rollback is used to bring an area back to a previous state. It undoes actions done during time `t:[time]` in radius `r:[radius]` on blocks, animals, chests, item frames, maps, and more. If someone's house is blown up, this is how you will bring it back.

!!! info
	You must ***always*** specify a radius while writing a rollback command, it should never be `r:#global`.

!!! info
	If you are rolling back a grief, roll back while specifying a user. If a rollback is only partially completed, i.e. part of someone's roof is still missing, you may be able to discover another griefer with [inspect](#Inspect)

### `restore`

Usage: `/coreprotect restore` or `/co rs`

- [Parameters](#Parameters)

This command is used to undo a [rollback](#Rollback).

### `undo`
Usage: `/co undo`

This command undoes your latest [rollback](#Rollback) or [restore](#Restore).

---
## Parameters

Usage: `/co l u:[user] t:[time] r:[radius] a:[action] b:[blocks]`

This usage uses [lookup](#Lookup) as an example. The formatting is the same for `/co rb` and `/co rs`.

- user: username of user whose logs will be isolated in results -- u:`rchristopherc`
- time: How far back in time to look back. Specify time length with s (seconds), m (minutes), h (hours), w (weeks), y (years) -- t:`10m`, t:`2h`, t:`1w`, t:`1d,5h`
- radius: radius from user to check logs for, use `#global` to check the whole world -- r:`5`, r:`#global`
- action: action user or entity took, or can be used to check chat logs (actions list from [Mine Realm](https://www.minerealm.com/community/viewtopic.php?f=32&t=6781))
	- a:block (blocks placed/broken)
	- a:+block (blocks placed)
	- a:-block (blocks broken)
	- a:chat (messages sent in chat)
	- a:click (player interactions)
	- a:command (commands used)
	- a:container (items taken from or put in chests)
	- a:+container (items put in chests)
	- a:-container (items taken from chests)
	- a:inventory (items dropped or picked up by players)
	- a:+inventory (items picked up by players)
	- a:-inventory (items dropped by players)
	- a:item (items dropped, picked up, taken from, or put in chests)
	- a:+item (items picked up or put in chests)
	- a:-item (items dropped or taken from chests)
	- a:kill (mobs/animals killed)
	- a:session (player logins/logouts)
	- a:+session (player logins)
	- a:-session (player logouts)
	- a:sign (messages written on signs)
	- a:username (username changes)
- blocks: actions done on a specific block, such as b:`56` (diamond_ore). Must use block ID's, which you can get [here](https://minecraftitemids.com/).
---
## Further Reading

This page only covers the basics of coreprotect. For more information, use of commands, watch [this video](https://www.youtube.com/watch?v=JwijCiueZ3Y) by YourMCAdmin and read the sources.

!!! quote "Sources"
	- [GameDB](https://gamedb.gg/games/minecraft/coreprotect-commands/)
	- [MineRealm/Intelli](https://www.minerealm.com/community/viewtopic.php?f=32&t=6781)
	- [Core Protect](https://www.spigotmc.org/resources/coreprotect.8631/)
	- [Mine Realm](https://www.minerealm.com/community/viewtopic.php?f=32&t=6781)
