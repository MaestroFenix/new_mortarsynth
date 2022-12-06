# New Mortarsynth NPC
NPC Mortarsynth done from scratch, no leaked code used.

Features:
* Banking movement
* Slight and Heavy Flinching
* Full fly navigation and path finding
* Slight improved model and textures
* Gibs ( Gently donated by Shift and Cvoxalury, made originally for _Dark Interval_ )
* Mortar attack: Mid-range energy ball ( DMG and radius tweakable with `sk_dmg_energy_grenade` and `sk_energy_grenade_radius`. RoF tweakable with `sk_mortarsynth_mortar_rate` )
* Repulsor: Close range energy wave that pushes away anything and causes a bit of energy damage ( RoF tweakable with `sk_mortarsynth_repulse_rate` )
* Constant movement and seeking for cover behavior
* Particles
* Sound when hurt
* Blood

Included test map and alternative bumpmaps as bonus


# Credits:
* Valve Software: Original Mortarsynth model, code snippets from retail code ( mostly the Manhack and the Base Scanner )
* Alexandra "Maestra Fénix" Bravo: Programming, mesh and VMT tweaks, upscaled tail texture, sounds ( actually renamed sound files from retail NPCs ), glueblob model recreation
* Shift: Bumpmaps
* Cvoxalury: Gib models

Feel free to integrate this on your mods, as long as you credit everybody.


# Instructions of use:

1. Place the code files on your codebase. Default path is `game/server/hl2/`
2. Declare the files into your VPC script ( Default is `game/server/server_hl2.vpc` )
3. Replace the `if 1` and `if 0` codeblocks with the `ifdef` and `ifndef` from your codebase
4. Build the DLLs
5. Place the contents of `materials`, `models` and `sound` within your mod root directory
6. Integrate `cfg/skill.cfg` and `scripts/game_sounds_manifest.txt` with your mod file version. Then place `scripts/npc_sounds_mortarsynth.txt`