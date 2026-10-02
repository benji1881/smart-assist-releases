# Smart Assist

A client-side Minecraft mod that helps with **PvE combat** and everyday
chores for players who find fast clicking or precise aiming hard. Every
feature is optional and configurable in game.

**Smart Assist never targets players on its own.** Auto-Attack and Bow
Assist skip players, Bow Assist won't shoot with a player in the way, and
the only players it ever shows are your own teammates (party frame and
teammate chevrons).

This repository holds the release jars. The mod checks it when the game
starts and updates itself from the latest release.

## Features

### Combat
- **Auto-Attack** - hits nearby mobs at full charge with the weapon you hold, with optional aim assist and automatic critical hits.
- **Bow Assist** - aims bows and crossbows at mobs, allowing for arrow drop and movement, and shoots once the shot is clear.
- **Auto Block** - raises your shield against mobs close by and incoming arrows, fireballs and other projectiles.
- **Reflect Fireballs** - hits a ghast's fireball or a breeze's wind charge back at the mob that fired it.
- **Skip Neutral Mobs** - leaves zombified piglins, piglins and endermen alone until they're angry.
- **Anti-Cheat Safe** - keeps everything the mod does to what a player could do by hand, for servers with anti-cheat.

### Survival
- **Auto Eat / Auto Pot** - eats or drinks from the hotbar when hunger or health runs low.
- **Stop To Heal** - pauses Auto-Attack while you're hurt so you can eat or drink.
- **Auto Totem** - moves a Totem of Undying into your offhand when you're about to die.
- **Auto Armor** - wears the best armor you carry, and swaps a piece out before it breaks.
- **Auto Mend** - repairs your Mending gear with experience and Bottles o' Enchanting.
- **Auto Elytra** - puts your elytra on when you jump in mid-air and your chestplate back on when you land.
- **Fall Safe** - breaks a fall that would hurt with an elytra, a Slow Falling potion or a water bucket.
- **Lava Guard** - stops you walking into lava.

### Tools and utilities
- **Auto Tool** - switches to the best tool in your hotbar for the block you're breaking.
- **Auto Replenish** - refills an empty hotbar slot with the same item from your inventory.
- **Farmer** - harvests and replants ripe crops, plants saplings and seeds bare farmland.
- **Fisherman** - reels in when a fish bites and casts again.
- **Rancher** - feeds every animal in reach with one right-click.
- **Lamplighter** - places torches wherever it's dark enough for mobs to spawn.
- **Bridger** - places blocks under you as you walk off an edge, and pillars straight up.
- **Librarian** - rerolls a librarian's trade until it offers the book you want.
- **Quick Stack** - buttons on chests to move matching items in or out, and to sort.
- **Brewmaster** - pick a potion and the brewing stand is loaded step by step until it's done.
- **Blacksmith** - repairs your damaged items at the anvil with one click.
- **Sticky Mine / Sticky Use** - keeps mining or using an item without holding the button.

### Display
- **Radar** - markers around the crosshair pointing at nearby mobs, teammates, chests, spawners and ores, plus a minimap.
- **Target Highlight** - outlines the mob you're attacking.
- **Arc Preview** - shows where an arrow or crossbow bolt will land.
- **Health Bars** - health over mobs' heads, with damage numbers and a bar while a mob winds up an attack.
- **Cooldown Numbers** - seconds left on item cooldowns, such as ender pearls, over the hotbar.
- **Hit Direction** - shows which way damage came from.
- **Party Frame** - your teammates' health, armor, distance and danger.

### Settings
- **Presets** - save sets of settings, switch between them with a key, or tie one to a server.
- **Settings menu** - search for any setting, hover a row for help, and choose from ten themes.
- **Auto Update** - downloads new releases and installs them on the next restart.
- Works alongside **Better Combat** and **Punchy**.

Open the settings with the **Delete** key or from the mod list. Other keys
are unbound until you set them in Options -> Controls.

## Download

Get the jar for your Minecraft version and loader from
[Releases](../../releases), and put it in your `mods` folder.

### Versions

| Build | Loader | Needs |
|---|---|---|
| Minecraft 26.3 | Fabric | Fabric API, Cloth Config |
| Minecraft 26.2 | Fabric | Fabric API, Cloth Config |
| Minecraft 26.1.2 | NeoForge | Cloth Config |
| Minecraft 1.20.1 | Fabric (Loader 0.18.4+) | Fabric API, Cloth Config |

ModMenu is optional on Fabric. On 1.20.1, features for things that version
doesn't have (spears, maces, trial spawners) do nothing.

See the [changelog](../../releases) on each release for what's new.
