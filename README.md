# Tradeskill Route Planner

A route planner for **Monsters & Memories** tradeskills. Tick the professions you want to level, enter your skill now
and the skill you want to reach, choose where your materials may come from, and get one combined route: when a step
needs parts another ticked profession makes, you make them yourself and that profession levels too.

**Use it:** https://explorethefloor.github.io/mnm-tradeskill-planner/

## What it does

- **Combined route.** Each stage is the cheapest step per skill point across the ticked professions. Suppliers
  (Smelting, Tanning) level from the bars and canvases the others need instead of on their own.
- **Material sources.** Vendor only, vendor + harvest, + mob drops, or + Enchanting and Disenchanting materials.
- **Prices you know.** Your own prices win over everything (use `*` for any text, e.g. `Cracked * Mold`). Then prices
  seen at vendors, then the wiki's base price; a vendor item with no known price uses a price you set.
- **Shopping list.** Schematics to buy, and what to buy, harvest or loot for the whole route, with where.
- **Cards.** Every item and recipe name is a link: where to buy, make or find it, and what uses it.

Your choices are kept in your own browser. Nothing is sent anywhere.

## Assumptions

- The game doesn't publish skill-up or failure odds. The route assumes a number of combines per skill point (default
  2) for any recipe that isn't trivial yet, and only uses recipes up to a set number of points above your skill
  (default 30) so failures stay rare. Both are settings on the page.
- A recipe that needs a schematic or pattern is used only when its seller is known. Recipes with no schematic or
  pattern at all (components such as straps, canvases, plates and chain links) count as learned with the skill.
- Trivials marked `?` or `~` on the wikis are guesses.

## Data

Recipes, item sources and schematic sellers come from the community wikis:
[monstersandmemories.wiki](https://monstersandmemories.wiki/tradeskills) and the
[Monsters and Memories Wiki](https://monstersandmemories.miraheze.org/wiki/Tradeskills).
Vendor stock and prices are what vendors were seen selling in Night Harbor; prices change with faction standing.
