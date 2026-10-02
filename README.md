<img width="1060" height="598" alt="image" src="https://github.com/user-attachments/assets/54067259-61e1-4c91-8688-c6bcadb44c41" />


# 🌽 Pay or Die

**Grow, gamble, bonk zombies... and pay the rent.**

*Pay or Die* is a pixel-art farming survival game that runs entirely in your web browser. You start with an empty field, a handful of seeds, a rusty shovel and 20 gold. Every day the landlord wants more rent, and every 30 seconds the crows, zombies and stranger things get bolder. Farm smart, take risks, protect your crops, and pay up. Or else.

---

## Table of Contents

- [Features](#features)
- [How to Play](#how-to-play)
- [Controls](#controls)
- [Crops](#crops)
- [Shovels](#shovels)
- [Enemies](#enemies)
- [Stamina](#stamina)
- [Shops](#shops)
- [Difficulty](#difficulty)
- [Tips](#tips)
- [Running the Game](#running-the-game)
- [Technical Notes](#technical-notes)
- [Credits](#credits)
- [Disclaimer](#disclaimer)
- [Copyright and Usage](#copyright-and-usage)

---

## Features

- **Pixel-art farming** on a 30×15 tile farm with tilling, planting, watering and harvesting.
- **14 crops**: 4 vegetables, 6 fruits, a risky mystery seed and 3 rare crops worth big gold.
- **Enemies that escalate**: crows, red birds, pink poison birds and slow-moving zombies, with the threat rising every 30 seconds.
- **5 shovels with special abilities**, from a rusty starter to a legendary shovel that turns zombies into crop guardians.
- **Stamina system**: every swing costs energy, and running out slows you down.
- **8-direction walk animation** with a 4-frame walk cycle.
- **Three shops**: seeds, shovels, and a style shop with clothes and daily boosts.
- **Clothes that stay unlocked** across runs.
- **Keyboard, mouse and touch controls**, with click-to-move pathfinding.
- **Settings menu** with volume, music, mute, difficulty and a controls page.
- **Chiptune music and retro sound effects**, generated live in the browser.
- **Nothing to install.** The whole game is one HTML file.

---

## How to Play

### The goal

Survive **5 days** by paying rent at the end of each day. Each day lasts **150 seconds**.

| Day | Rent (Normal) |
|-----|---------------|
| 1   | 30 gold       |
| 2   | 70 gold       |
| 3   | 130 gold      |
| 4   | 210 gold      |
| 5   | 320 gold      |

- If you can't pay the rent when the day ends, you're **evicted** and the game is over.
- If you run out of gold, seeds and growing crops all at once, you're **bankrupt** and the game is over.
- Pay all 5 rents to **save the farm** and win.

Your **score** is the total gold you earn during a run. Your best score is saved.

### The farming loop

1. **Till** a grass tile to turn it into soil.
2. **Plant** a seed in the soil.
3. **Water** a growing crop to make it grow twice as fast until its next growth stage.
4. **Harvest** a ripe crop to earn gold.
5. **Buy** better seeds, shovels and boosts, then repeat.

Ripe crops **rot after 25 seconds**. A red **!** blinks over a crop that's about to rot, so harvest quickly. Withered crops can be cleared to reuse the soil.

---

## Controls

### Keyboard

| Key | Action |
|-----|--------|
| `WASD` / Arrow keys | Move |
| `Space` / `Enter` / `Z` / `J` | Action: till, plant, water, harvest, attack, open a shop |
| `Q` / `E` | Previous / next seed (only seeds you own) |
| `1` to `5` | Pick one of the first five seeds |
| `P` / `Esc` | Open the menu (pauses the game) |
| `M` | Mute or unmute |

In shops and menus, use the arrow keys to browse, `Enter` to buy or select, and `Esc` to go back.

### Mouse

| Input | Action |
|-------|--------|
| Left click on far grass or a path | Walk there (the farmer finds a way around obstacles) |
| Left click on grass next to you | Till it |
| Left click on soil or a crop | Walk over and plant, water, harvest or clear |
| Left click on a building | Walk to the door and open the shop |
| Right click on a zombie | Walk to it and hit it (hold to keep swinging) |
| Right click anywhere else | Swing the shovel in that direction |
| Click the seed box in the top bar | Change seed |
| Mouse wheel | Scroll shop lists |

### Touch

On phones and tablets, an on-screen D-pad appears. **A** is the action button and **B** switches to the next seed. Tapping the field works like a left click.

---

## Crops

### Vegetables and fruits

| Crop | Seed Cost | Grow Time | Sells For |
|------|-----------|-----------|-----------|
| Wheat | 2g | 9s | 5g |
| Strawberry 🍓 | 4g | 12s | 9g |
| Carrot | 5g | 15s | 12g |
| Blueberry 🫐 | 8g | 18s | 19g |
| Tomato | 10g | 22s | 26g |
| Grape 🍇 | 14g | 24s | 34g |
| Corn | 18g | 30s | 45g |
| Pineapple 🍍 | 22g | 32s | 55g |
| Watermelon 🍉 | 30g | 38s | 75g |
| Pumpkin 🎃 | 40g | 45s | 105g |

Grow times are without watering. Watering doubles the speed until the next growth stage.

### The Mystery Seed (15g)

A gamble. When it ripens it becomes one of these:

- **Dud (40%)**: it withers and you get nothing.
- **Common crop (42%)**: a random vegetable or fruit.
- **Rare crop (18%)**: one of the crops below.

### Rare crops

Every normal seed also has a **4% chance** to turn into a rare crop when it ripens.

| Rare Crop | Sells For |
|-----------|-----------|
| Ruby Tomato | 90g |
| Gold Corn | 120g |
| Star Melon | 200g |

---

## Shovels

Shovels are sold at the **Tool Stand** on the left side of the farm. You start with the Rusty Shovel. Shovels you buy last for the current run, and you can switch between the ones you own.

| Shovel | Rarity | Cost | Ability |
|--------|--------|------|---------|
| Rusty | Common | Starter | 5 hits to defeat a zombie |
| Iron | Uncommon | 40g | 3 hits, knocks zombies far back |
| Frost | Rare | 90g | 3 hits, freezes zombies for 3 seconds |
| Gold | Epic | 180g | One hit defeats any zombie |
| Necro | Legendary | 260g | Defeated zombies rise as green **guardians** for 40 seconds. Guardians chase off birds and fight other zombies. |

Hit counts are for Normal difficulty.

---

## Enemies

### The threat level

Every **30 seconds** the threat level goes up. An alarm sounds, more enemies can appear at once, and new types join in. The threat level carries over between days: day 2 starts at threat 1, day 3 at threat 2, and so on.

### Birds

Birds land on growing crops and peck at them. Walk close to a bird to scare it away and earn gold.

| Bird | Arrives At | Behavior | Gold for Shooing It |
|------|------------|----------|---------------------|
| Black Crow | Start | Eats a crop in 4.5 seconds | 1g |
| Red Bird | Threat 1 | Faster, eats a crop in 3 seconds | 2g |
| Pink Bird | Threat 2 | **Poisons the soil.** The tile turns pink and can't be planted until the next day. | 3g |

### Zombies

- Zombies climb over the fence and shamble slowly toward the nearest crop, then eat it.
- If there are no crops, they come after you. A zombie touching you knocks you back and steals 3 gold.
- Defeating a zombie earns **4 gold**.
- A health bar appears over a zombie once it's been hit.

---

## Stamina

Your stamina bar has **5 levels**, shown in the top bar and as small pips above the farmer's head.

- Every shovel swing uses one level, whether it hits or misses.
- Stamina starts refilling about a second after your last swing.
- At **zero** you're exhausted: you move at **half speed** until the bar is completely full again (about 7 seconds).

With the Rusty Shovel, defeating one zombie uses all your stamina, so stronger shovels are worth saving for.

---

## Shops

| Shop | Location | Sells |
|------|----------|-------|
| **The Old Shed** | Top right | All seeds |
| **Tool Stand** | Left side | Shovels |
| **Style Shop** | Bottom right | Clothes and boosts |

### Clothes (kept forever, even after game over)

| Item | Cost |
|------|------|
| Straw Hat | 40g |
| Red Cap | 80g |
| Gold Crown | 300g |
| Red Flannel | 50g |
| Snow Tee | 70g |
| Gold Suit | 220g |

### Boosts (last until the end of the current day)

| Boost | Cost | Effect |
|-------|------|--------|
| Speed Tonic | 20g | Move 40% faster |
| Grow Juice | 35g | All crops grow 50% faster |
| Lucky Charm | 40g | Triple the chance of rare crops |
| Market Bell | 45g | Harvests sell for 25% more |

---

## Difficulty

Choose a difficulty from the menu on the title screen. It's locked once a run starts.

| Setting | Easy | Normal | Hard |
|---------|------|--------|------|
| Rent | 70% | 100% | 130% |
| Enemy spawn rate | Slower | Normal | Faster |
| Zombie health | 4 | 5 | 6 |
| Bird eating speed | Slower | Normal | Faster |
| Stamina per swing | Lower | Normal | Higher |

---

## Tips

- **Water everything.** It doubles growth speed and costs nothing but time.
- **Don't overplant early.** A field you can't protect is a buffet for crows and zombies.
- **Stay near your crops.** Birds flee when you get close.
- **Watch the timer.** The timer bar has a mark every 30 seconds, so you can see when the next threat increase is coming.
- **Save gold for rent.** Check the RENT value in the top bar. It turns green when you can afford it.
- **Mystery seeds are a gamble.** They pay off best with a Lucky Charm active.
- **Manage your stamina.** Don't waste swings, or you'll be slow when the next zombie shows up.


---

## Technical Notes

- **Rendering:** HTML5 Canvas at a 480×270 internal resolution, scaled up with crisp pixel rendering.
- **Art:** every sprite is defined in code as a pixel array. There are no external image files.
- **Audio:** music and sound effects are generated live with the Web Audio API. There are no audio files.
- **Game loop:** fixed timestep running at 60 updates per second.
- **Pathfinding:** a breadth-first search on the tile grid powers click-to-move.
- **Saving:** best score, clothes and settings are stored in your browser's `localStorage`. Nothing is sent anywhere.

---

## Credits

- **Game design and development:** J A C K A L
- **Walk-cycle animation:** based on a 16×16 walk sprite sheet, recolored as the farmer. 

---

## Disclaimer

This game is provided **"as is"**, without warranty of any kind. It's a personal project made for fun and learning. The author isn't responsible for any issues that may come from using or running it.

*Pay or Die* is a work of fiction. Any resemblance to real landlords, zombies or suspiciously pink birds is purely coincidental.

---

## Copyright and Usage

**© 2026. All rights reserved.**

This repository is public so people can **play and enjoy the game**. That doesn't make the code or assets free to take.

**Please don't:**

- ❌ Copy, reupload or redistribute this game or its code, in whole or in part.
- ❌ Claim this game or any part of it as your own work.
- ❌ Sell this game or use it in any commercial product.
- ❌ Reuse the code, sprites, music or game design in your own projects without written permission.

**You're welcome to:**

- ✅ Play the game.
- ✅ Share a link to this repository or the hosted game.
- ✅ Read the code to learn from it.
- ✅ Report bugs or suggest ideas through Issues.

If you'd like to use any part of this project, please ask first by contacting **tifir2024z@gmail.com**.

MORE ADJUSTEMENTS TO BE DONE SOON
---
