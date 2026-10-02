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

- **Auto-Attack** - hits nearby mobs at full charge with the weapon you hold.
  Trigger mode (only what you look at), optional aim assist, Crit Timing
  and Auto Crit (which jumps for you, with Sprint Crits works while you
  sprint too, and with Prefer Sweep stands aside when a sword's sweep would
  be worth more). No-Jump Crits skips the jump in singleplayer and LAN
  worlds only - it fakes the jump in packets, which servers can ban for.
  On a server with anti-cheat, turn on **Anti-Cheat Safe** in General >
  Menu: Auto-Attack then only hits the mob under your crosshair (Aim
  turns you onto it first), everything the mod does reaches the server in
  the order a vanilla client sends it, Sprint Crits, Fall Safe and Lava
  Guard do only what you could do yourself, in view, moving items from
  the bag stands you still for a tick, and No-Jump Crits is off.
  Never hits players, or any player's tamed animal, and leaves name-tagged
  animals and villagers alone. Priority picks between mobs - nearest, by
  health, or the one closest to your crosshair. Falling onto a mob with a
  mace, it hits just before you land, for the full smash.
- **Bow Assist** - aims bows and crossbows at mobs, allowing for arrow
  drop and movement, and shoots once the shot is clear. Auto Draw draws by
  itself, and Look To Switch hands the aim to whatever you put your
  crosshair on. Never shoots with a player or pet in the way.
- **Auto Block** - raises your shield when mobs are close, turns to face
  flanking mobs and mob archers, and blocks arrows, fireballs and other
  mob projectiles. Stands down while an axe has your shield disabled.
  Swing Timing holds your swing until a mob's hit has landed on the
  shield, then hits straight after, so no hit finds the shield down.
- **Reflect Fireballs** - hits a ghast's fireball or a breeze's wind charge
  back at the mob that fired it.
- **Auto Eat / Auto Pot** - eats or drinks from the hotbar when hunger or
  health runs low, skipping harmful food and potions. Auto Pot also drinks
  Fire Resistance in lava and milk against Wither. Ordinary food waits for
  a fight to end - including a skeleton shooting from further off, but not
  a mob behind a wall - and for you to be on your feet, not mid-jump or
  swimming.
- **Stop To Heal** - stops Auto-Attack's swing while you're hurt and carrying
  something that would put it right, so Auto Eat and Auto Pot get a moment
  to work. Your own clicks still attack.
- **Auto Totem** - a Totem of Undying into your offhand at low health, in
  a fall that would kill you, next to a lit creeper or while flying with
  an elytra.
- **Auto Armor** - puts on the best armor you carry, by how much damage
  each piece lets through (armor, toughness and Protection). Never takes
  off an elytra, a pumpkin or a head. Swap Before Breaking takes a piece
  off before it breaks when you carry a spare.
- **Auto Mend** - keeps your Mending gear repaired: the damaged Mending
  items in your inventory take turns in the offhand, where experience
  reaches them, and when something you wear or hold wears down you throw
  Bottles o' Enchanting at your feet until it's back up.
- **Auto Elytra** - press jump in mid-air and the elytra in your inventory
  goes on and opens; your chestplate goes back on when you land. It waits
  for a real drop (5 blocks from the top of the jump), and with a rocket in
  hand it takes off from anywhere and fires the rocket for you.
  Soft Landing lifts the nose when a glide would end in a crash that
  hurts, into a wall or the ground, and lets go once it's safe.
- **Fall Safe** - catches a fall that would hurt: opens your elytra, drinks
  a Slow Falling potion, or puts water below you at the last moment and
  picks it up again.
- **Lava Guard** - stops you walking into lava: it holds sneak as you walk up
  to a drop with lava under it, and holds your own movement back at the edge
  of lava that's already at your feet.
- **Skip Neutral Mobs** - leaves zombified piglins, piglins and endermen
  alone until they're angry.
- **Auto Tool** - takes the best hotbar tool as you start breaking a
  block, and hands back what you held once you stop. Fortune for ores (or
  Silk Touch, your pick), Silk Touch for ender chests, and it won't wear
  an enchanted tool down to breaking or your sword down on dirt.
- **Farmer** - right-click ripe crops, sugar cane and cactus to
  harvest them. Any ripe crop you break - right-click, or left-click as
  with cocoa - is replanted, and Auto Sapling plants a sapling where you
  chopped a tree's bottom log. Plant Empty Farmland plants bare farmland
  around you while you hold seeds. Holding FTB Ultimine's key hands the click
  to Ultimine, which does the whole patch.
- **Fisherman** - reels in when a fish bites and casts again, and stops
  before your rod breaks.
- **Rancher** - one right-click with a breeding food feeds every
  animal in reach, no aiming needed.
- **Lamplighter** - places a torch wherever it's dark enough for mobs to
  spawn, from your hotbar or inventory: on the wall beside you at eye
  height, or at your feet when there's no wall. Never on the block you're
  looking at, so digging a tunnel doesn't knock it off again.
- **Bridger** - walk off an edge and a throwaway block (cobblestone, dirt,
  planks...) goes down under your next step, so you walk across gaps, lava
  and water. Min Drop sets how deep a drop must be, so steps down a hill are
  walked as normal. Sprint-jump along a wall and a stepping stone goes
  where each jump lands; a walking jump off an edge goes down it. Tower: hold jump
  standing still to pillar straight up. With Anti-Cheat Safe on it sneaks
  and looks at each block it places, so bridge backwards there.
- **Librarian** - rerolls a librarian's book until it offers one you
  ticked: look at its lectern and press the key. It breaks and replaces the
  lectern for you and stops when the book turns up. Tip: wall the lectern
  in, so the broken one drops at your feet instead of flying off - or carry
  a spare.
- **Quick Stack** - buttons on chests, barrels and shulker boxes: Insert
  moves in the items the chest already has, Extract takes out the items
  you already carry. Sort buttons tidy the chest, or your inventory from
  its own screen.
- **Brewmaster** - a panel beside the brewing stand lists every potion the
  game can brew, the ones you can make first and the rest greyed (hover
  one to see what's missing). Click one (right-click for splash, longer or stronger,
  shift-click to queue it) and the stand is loaded step by step - fuel,
  bottles, each ingredient as the last one finishes - until it's brewed, and the
  potions come out into your inventory. Walk away and a label over each
  stand counts down its step and says when it needs you again, so several
  stands can brew at once - and with Tend Stands on, a stand in reach is
  loaded and emptied for you without opening its screen.
- **Blacksmith** - a list beside the anvil names your damaged things
  you carry the material for, with the cost in levels. Click one (or
  Repair All) and it's repaired and back in its slot. Works in
  Sophisticated Backpacks' anvil upgrade too, with what's in the backpack.
- **Auto Replenish** - when a hotbar slot runs out, the same item comes
  in from your inventory: the next stack of torches, the next golden
  apple, a spare pickaxe when one breaks, and in the offhand the next
  totem or shield. Only exact matches, and never after you drop or move
  something yourself.
- **Sticky Mine / Sticky Use** - tap a key to keep mining or using an item
  without holding the button.
- **Radar** - markers around the crosshair pointing at nearby mobs and
  teammates (chevrons, or faces) and at chests, spawners and
  exposed ores, with distances, height arrows and a range ring. Look at
  something marked and its marker leaves the ring for the thing itself: a
  chevron over the mob's head pointing down at it, a block's icon in the
  middle of the block. The General window's Map (HUD tab) shows the same as a minimap -
  round, or the half in front of you - moved in Edit HUD and zoomed with
  = and -.
- **Target Highlight** - outlines the mob Auto-Attack or Bow Assist is
  going for, in a colour you choose.
- **Arc Preview** - dots along a drawn bow's or loaded crossbow's flight
  and a ring showing where it can land, as wide as the game's own spread.
- **Health Bars** - a WoW-style nameplate over the head of the mob you're
  fighting, or of every mob nearby: name, health and golden hearts. With
  Damage Numbers, the health you knock off floats up off the mob, MMO-style;
  with Cast Bars, a bar under it fills while the mob winds up an attack (a
  creeper's fuse, an evoker's spell, a skeleton's draw).
- **Cooldown Numbers** - the seconds left on an ender pearl, wind charge or
  other item cooldown, over its hotbar slot.
- **Hit direction** - shows which way damage came from.
- **Party frame** - your team's health (bar or hearts), armor, distance and
  danger (fire, freezing, drowning). Vanilla `/team` and FTB Teams parties,
  or your own list of names in the General window's Party tab when the server has neither.
- **Presets** with a Next Preset key, a toggle key and a hold key for the
  combat features, and a status HUD. A preset saved for This Server Only
  loads as you join that server and nowhere else, and a server you've
  never joined starts with everything off.
- **Settings menu** - search any setting from the bar at the bottom (it
  forgives typos), hover a row for what it does, and right-click a target
  category to switch single mobs off. Ten themes (including Fantasy, Clear
  Blue, High Contrast and Colour-blind), an accent colour and adjustable
  see-through windows.
- **Auto Update** - checks for a new release as the game starts and
  installs it on the next restart.
- Works alongside **Better Combat** and **Punchy**.

Open the settings with the **Delete** key (or from the mod list), and zoom
the Map with **=** and **-**. The other keys are unbound until you set them
in Options -> Controls.

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

ModMenu is optional on Fabric. On 1.20.1 some features have nothing to work
with: there are no spears, maces or trial spawners, Auto-Attack's reach is
the fixed vanilla 3 blocks (6 in creative), and Fall Safe doesn't place
water into waterloggable blocks such as slabs, since the 1.20.1 bucket
fills the block instead.

See the [changelog](../../releases) on each release for what's new.
