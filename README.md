# Jeqarch

Source for some of CAE Jones's BGT (Blastbay Game Toolkit) audio games, roughly 2011-2017, plus Sengoku Tide (2024-2026).

- **2DSwamp**: a side-scrolling platformer take on Aprone's Swamp, with a map editor (ctrl+U), 2013-2015. Source only, plus the grenade sounds. Everything else plays from Swamp's `sounds/` folder, so put `2DSwamp.bgt` and its includes in a Swamp folder to run it. The current Swamp has dropped some of the sounds it uses: the Flayer and Hulk zombies, Vulcan, the M40 crouch, several item and player sounds, and `Player/hurt1`-`3`. A Swamp from around 2013 has them all. `sounds/platforms/` (platform ambiences) and `music.mp3` were never part of Swamp.
- **JLA**: Justice League fan game. Source only, since its music and voices belong to their owners.
- **LePetitPlanet**: a small top-down adventure (2015) in a house, yard and beach, with enemies to fight and rings to find. Source and sounds. Its original sound pack is lost, so `paths.bgt` loads the sounds from `sounds/` instead. Large sounds were re-encoded as OGG, and `paths.bgt` falls back from `.wav` to `.ogg`. `lpp2.bgt`, a planned sequel, was an empty file.
- **Mario**: an accessible Super Mario Bros. with an audio camera and platform cues (2011-2012). Source only (`Mario.bgt`, 2012-08), since the sounds and music come from the NES game.
- **Mystery**: a short single-script game.
- **Redsword**: a short 2D platformer with audio and braille output (2016-2017). Source and sounds. `redsword.bgt` is the latest source (2017-01). It includes `sounds.dat`, which isn't stored here: run `pack.bgt` in this folder to rebuild it from the sound folders. It also expects `quickdict`, `KeyC`, `FiniteStateMachine`, `custom_voice` and `clock` from `c:\bgIncludes\` and `dynamic_menu` from `c:\winsim\`. Copies of most of these are in `include/`.
- **SengokuJidai**: source, maps, campaigns and sounds. `sj.bgt` is the playable game, `SJ2.bgt` an incomplete sequel and `sjerver.bgt` the multiplayer server.
- **SengokuTide**: source and sounds. `SengokuTide/st3.bgt` is the latest revision (2026-03); `st.bgt` and `st (2).bgt` are earlier ones from 2026. `neighborhood_game.bgt` is a separate game built on the same includes. `pgs21/` is a separate experiment (`play.bgt`, `World.bgt`).
- **Sonic**: accessible Sonic the Hedgehog fan remake (2011-2013). Source only (`sth.bgt`, changelog, walkthrough), since its music and sounds belong to their owners.
- **Sword**: a small sword-fighting game (2013). Source and sounds. Expects `FiniteStateMachine` and `custom_menu` from `c:\bgIncludes\`.
- **Temporal**: source, maps and sounds.
- **Triastra**: a third-person 3D audio adventure (2015) with flight, a sword and a fixed camera. Source and sounds. The sounds were gathered from the game's 2016 sound pack and the folders it came from, with large WAVs re-encoded as OGG. `paths.bgt` maps the original paths onto `sounds/` and falls back from `.wav` to `.ogg`. See `readme.txt` for controls.
- **ToweringTones**: a falling-gems puzzle game where matching gems annihilate each other, with normal and flash modes (`towertone.bgt`, 2011). Source, music and sounds.

Run a game with BGT: open its main `.bgt` file in `bgt.exe`. Compiled builds aren't included because scanners false-flag BGT executables.
