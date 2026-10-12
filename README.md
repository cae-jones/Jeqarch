# Jeqarch

Source for some of CAE Jones's BGT (Blastbay Game Toolkit) audio games, roughly 2011-2017, plus Sengoku Tide (2024-2026).

- **JLA**: Justice League fan game. Source only, since its music and voices belong to their owners.
- **Mystery**: a short single-script game.
- **Redsword**: a short 2D platformer with audio and braille output (2016-2017). Source and sounds. `redsword.bgt` is the latest source (2017-01). It includes `sounds.dat`, which isn't stored here: run `pack.bgt` in this folder to rebuild it from the sound folders. It also expects `quickdict`, `KeyC`, `FiniteStateMachine`, `custom_voice` and `clock` from `c:\bgIncludes\` and `dynamic_menu` from `c:\winsim\`. Copies of most of these are in `include/`.
- **SengokuJidai**: source, maps, campaigns and sounds. `sj.bgt` is the playable game, `SJ2.bgt` an incomplete sequel and `sjerver.bgt` the multiplayer server.
- **SengokuTide**: source and sounds. `SengokuTide/st3.bgt` is the latest revision (2026-03); `st.bgt` and `st (2).bgt` are earlier ones from 2026. `neighborhood_game.bgt` is a separate game built on the same includes. `pgs21/` is a separate experiment (`play.bgt`, `World.bgt`).
- **Sonic**: accessible Sonic the Hedgehog fan remake (2011-2013). Source only (`sth.bgt`, changelog, walkthrough), since its music and sounds belong to their owners.
- **Sword**: a small sword-fighting game (2013). Source and sounds. Expects `FiniteStateMachine` and `custom_menu` from `c:\bgIncludes\`.
- **Temporal**: source, maps and sounds.
- **ToweringTones**: a falling-gems puzzle game where matching gems annihilate each other, with normal and flash modes (`towertone.bgt`, 2011). Source, music and sounds.

Run a game with BGT: open its main `.bgt` file in `bgt.exe`. Compiled builds aren't included because scanners false-flag BGT executables.
