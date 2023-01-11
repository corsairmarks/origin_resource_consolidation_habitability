# Overview

Driven Assimilators and Rogue Servitors with Origin: Resource Consolidation do not have their biological (Cyborg Species/Bio-Trophies) species's habitability preference set to machine.  This mod changes that by adding an extra event before initial empire Pops are generated to adjust habitability for these empire types with Origin: Resource Consolidation.

Because the starting Cyborg Species now prefers Machine Worlds, the guaranteed habitable worlds are instead random habitable classes. These worlds are also occupied with (very) early primitives, similar to Origin: Necrophage.

# Changes

This mod adds an extra event which is triggered after each empire's capital planet is initialized.  The event applies to Driven Assimilators (and Rogue Servitors - just in case) with the origin Resource Consolidation (aka Machine World).  The secondary, non-robotic species is altered to have ideal habitability for Machine Worlds (`pc_machine`). It also adds an extra event to set up the starting primitive worlds.

## Compatibility

Built for Stellaris version 3.6 "Orion" and backwards-compatible with versions 3.5 "Fornax," 3.4 "Cepheus," 3.3 "Libra," and 3.2 "Herbert."  Not compatible with achievements.

Should be compatible with almost anything.  If other mods add new origins which also start on a machine world, this mod will **not** affect them.

### When to Install

This mod can be safely added or removed from your save game after the game has started.  The code in this mod executes entirely during game setup - if the game was started with the mod, its effects have already been applied, otherwise no code will be executed.

### Not Included in "Subtle Polish"

This mod is intentionally not included in my modpack [Subtle Polish: A Collection of Fixes and Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2522974089) because it is a significant penalty to Origin: Resource Consolidation empires with a non-Lithoid cyborg secondary species.

### Recommended Companion Mods

[Planetary Modifier Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2496357128) patches the game setup process so any gas giants in your home system don't lose the Chthonian Planet modifiers.  The modifier is from the base game and is purely cosmetic.  It also lightly enhances Extensive Moons System and the C.A.R.E planet special modifier.

## Known Issues

Because of how species modification at game start works, you will have an "extra" species with no Pops in your species tab with the original planetary preference from empire design.  This extra parent species will not be hidden (uses the same type of modification as Origin: Shattered Ring in the base game).

## Changelog

* 1.0.0 Initial version
* 1.1.0 Mark as compatible with Stellaris version 3.2 "Herbert" - no script changes
* 1.2.0 Mark as compatible with Stellaris version 3.3 "Libra" - no script changes
* 1.3.0 Mark as compatible with Stellaris version 3.4 "Cepheus" - no script changes
* 1.4.0 Mark as compatible with Stellaris version 3.6 "Orion" - no script changes
* 1.5.0 Resource Consolidation guaranteed colonies are now primitives (like Necrophages) with random habitable planet classes
* 1.6.0 Add a compatibility trigger for other mods to check whether this one is active

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/origin_resource_consolidation_habitability)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property.  That will ensure the game can see the files, and also that CWTools will parse them.  Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.