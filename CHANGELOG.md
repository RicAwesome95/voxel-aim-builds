# Voxel Aim changelog


# v1.9.2

### Added

- Spectate: you also see the player's mouse while it's free (menus, pause), with their name under it
- Spectate: a WATCH button next to players in the global chat and the online list shows their game live (about a second behind), with their crosshair, colors, game settings and window layout; Esc leaves and puts your own settings back. Settings > Multiplayer: "Let others spectate you" (on by default)
- New setting: Countdown (Settings > General). Off = Aim Lab–style tasks start the moment you click, with no 3, 2, 1 (KovaaK's tasks already do; a 1v1 still counts down).
- New Stats tab in Settings, like Valorant's, to find the source of lag spikes: Client FPS, Total Frame Time, Worst Frame Time, CPU (Game) Time, CPU (Render) Time, Idle Time, Draw Calls, Used Memory, Network RTT, Network RTT Jitter, Packet Loss, Packets Lost (Total), Packets Receive Rate, Packets Send Rate, Uploaded Data and Out Packet Size. Each one is Hide / Text Only / Graph Only / Show Both (or set them all at once). Text goes in one line across the top (only what fits), graphs on the right (up to 14).
- New settings in Settings > General, both on by default, to see if they help your frame rate: Stats graph (turn it off to stop the KovaaK's-style stats, the Graph window and the KovaaK's results; the results screen is then the Classic card) and Replays (turn it off to stop recording your rounds).
- 7 new songs in the music playlist: Die For You (VALORANT, Grabbitz), Ticking Away (VALORANT, Grabbitz, bbno$), You're Under Arrest (ILLIT), greater than one (ericdoa, VALORANT), WATCH (Stella Mwangi, VALORANT), RENEGADE (VALORANT, 99GOD, C103) and RAJA (ARB4, Tienas, Mangal Suvarnan, VALORANT).
- The Range: a new table and skills-test screen, like Valorant's. The table is smaller and open at the front (shelves and ammo boxes inside, dark angled end blocks, a wooden top) with sandbag walls either side. The screen leans against it more upright, with lighter condensed text; shooting START or Practice lights up its box with a target icon for a moment, and START turns into EXIT while a test runs (the sensitivity boxes don't light up). You can't stand on the screen: land on it and you slide off the front.
- The Range bots got a new look, closer to Valorant's practice bots: rounded armour instead of plain boxes (shoulder pads, chest, head and limbs all curve), a tall rounded head with one glowing eye, a dark rib cage under the chest, and a yellow rim light along their outline that fades smoothly along every curve, stronger on the upper body than the legs.
- New setting: Mouse DPI (Settings > General). It's only used to show your cm/360.
- New results screen, like KovaaK's: Final Score and your high score, a graph of the round (Score, Accuracy, Dmg Eff, SPM, Kills, Kills/s, Damage; click to switch each one) and HISTORY of your earlier runs; SCORE CALCULATION (what each thing you did is worth), ACC, DMG EFF and KDR; ANALYSIS and PLAYLIST tabs; and the leaderboard with Entries, Median and your Percentile. STATS, DONE, NEXT and REPLAY at the bottom.
- New Graph window (on by default; switch it in the Windows list at the top right): your last round over time (Score, Accuracy, Dmg Eff, SPM, Kills, Kills/s, Damage) and HISTORY, right under the Replay window. Drag it anywhere.
- 17 new KovaaK's tasks, made from their .sce files. MICRO GOLD MINE is now complete: eth FP OGG Micro 60, Amare Dynamic TAF Micro, eth Didy - S, eth PP Micro, uv VBR Micro 2ts, eth Valorant Micro Reactive, eth FarSkeet, Aimerz+ 1w4ts HF Hard S1, 1w2ts Pasu Perfected Goated, HeadClick Altered and Valorant Fireworks Flick Horizontal - Far.

### Changed

- Gridshot Ultimate (5×5) room rebuilt from Aim Lab: a bigger hall with a platform taller than your eyes, bigger targets at Aim Lab's distance, softer lighting on the walls, and the targets throw shadows on the sunlit floor
- Gridshot Ultimate (5×5): targets closer together and the grid raised above eye level, matched to Aim Lab
- Replay window: the volume slider on the speaker button is now vertical (it pops up above the button) and disappears the moment you stop hovering
- Bullet marks redone like Valorant: the crater (bullet stopped) is a light, chipped dent with no black; the hole (bullet went through) is the same dent with a black core
- Range / Skirmish bullet marks stay fully visible for 9 s, then fade out (opacity, no shrinking) by 10 s
- Headshots go through: a bullet that hits a head goes on to the next head behind it, up to 5 bots / players with one bullet
- Bullet hole duration (Settings > General) is for the light rings on Amare GarfMicroTS's back wall again (0 = none, up to 12 s). The Range and Skirmish bullet marks always show, for 10 seconds.
- Settings > Video > Stats: Gameplay (Shooting Error) comes after Network. The Range screen's words no longer show through the table: they're drawn with depth now.
- Exe: the GPU Resident Drawer switch is gone. Changing it while the game runs made Unity rebuild its renderer, which failed ("Blitter is already initialized") and left the screen black; it stays off (the steadiest choice on most PCs).
- Windows: the Replay window is on by default (it opens after every round) and the Graph window is off by default; switch the Graph on in the Windows list (top right).
- The Replay window starts higher (just under the round's progress bar) and a little smaller. The Graph window sits right under it, so it never covers the Final Score; if you drag the Replay window away, the Graph stays where it was. Both stay clear of the chat at the bottom.
- Bullet marks look like Valorant's: a ringed hole where the bullet can go through, a cracked starburst crater where it can't. Each new mark glows red-orange for a moment, then cools. Marks show on every surface you hit (floor, crates, walls), never on players or bots.
- Replay window: in a small window, SHOW HITS / SHOW MISSES share the width and the buttons use shorter words (HITS, MISSES, SAVE FILE, OPEN FILE, FOLDER); button text can shrink further to fit.
- Exe: the resize arrows (and the hand / text pointers) now show as soon as you hover a window's edge, not only once you hold the mouse button.
- First start: Voxel Aim asks whether it may check for updates (YES, CHECK / NO THANKS). Either answer can be changed in Settings > General > Check for updates; a required update still shows.
- Every window resizes in every direction: drag any edge or corner. The Replay picture stays 16:9 inside the window (with bars), the Music window opens its song list when you drag it taller, and the Playlist window resizes even with no playlist running.
- Settings > General: Bullet tracers comes before Bullet hole duration.
- The Range screen: the AIM SENSITIVITY line is smaller so it fits its strip, and the screen's words no longer show through the table and the walls.
- The version number (bottom right) opens the changelog from the pause menu too; closing it takes you back to the pause menu.
- Shooting Error moved into the stats: Settings > Video > Stats > Gameplay > Shooting Error (Hide / Text Only / Graph Only / Show Both, off by default). It shows your firing + movement error in the Range and Skirmish; the box at the top right of the Range is gone.
- The Mod menu window can be resized too: drag any edge or corner (its contents scroll).
- Window resizing is easier to grab, like Windows 11: the edge reaches 8 pixels outside the window (and 4 inside), and the corners reach 16 pixels along each side, the same size however big the game window is.
- Update check: when the game opens, then every 6 hours (it was every 10 minutes). New setting Check for updates (Settings > General): off = only a required update still shows. An optional update now asks first (UPDATE NOW / LATER) instead of starting by itself, and waits until you're out of the round.
- The Playlist and Music windows can be resized: drag an edge or corner (the Music list's height while it's open).
- Smoother: shaders are prepared while the game loads (and when a KovaaK's map or the Skirmish map is built), the HUD's numbers and the Range's help text are no longer rebuilt every frame (less garbage, fewer hitches), and Unity no longer steps physics the game doesn't use.
- Wall penetration damage now uses measured Valorant numbers where they exist (Classic, Frenzy, Stinger, Ghost, Bulldog, Phantom, Vandal, Sheriff); other guns use a default for their tier.
- Wall penetration, like Valorant: Low guns (Classic, Shorty, Frenzy, Stinger, Bucky) go through wood and glass, Medium (Ghost, Spectre, Judge, Bulldog, Guardian, Phantom, Vandal, Marshal) also through stone, High (Sheriff, Operator, Ares, Odin) also through metal. Each wall takes away part of the damage, and a thick wall or a shot along a corner can stop the bullet. Where it gets through you see a bullet hole on both sides; where it doesn't, a lighter crater.
- Replay window: drag any edge or corner to resize it; the picture stays 16:9.
- The exe uses your own Windows pointers now (hand, text, move and the resize arrows) instead of drawn ones.
- Countdown: the growing copy of the number stays centred on it in a small window (it used to drift sideways).
- Long sessions build up less lag: targets are reused instead of made and destroyed on every hit, KovaaK's bot bodies share one material, and a KovaaK's map frees its memory when you switch tasks.
- Changelog: each version lists its newest changes first.
- The Range: START gives you infinite ammo while the test runs; your ammo is back to normal when it ends.
- Windows menu (top right): a SETTINGS button that opens Settings.
- Graph: switching a line on makes only that line rise; the others stay where they are.
- Video > General now has Display Mode (Fullscreen / Windowed Fullscreen / Windowed), Resolution and Monitor dropdowns. Every change asks you to confirm and reverts by itself after 15 seconds.
- Exe performance: the menus skip a hidden extra layout pass every frame, and the Replay window no longer searches the whole scene every frame or redraws its picture while it's paused and nothing changed.
- Buttons: a label that's too wide for its button now gets a slightly smaller font so it fits (down to 70%), instead of being cut off.
- Windows: drag an edge of the Replay window to change its width (the picture stays 16:9), or an edge or corner of the Graph window to change its size; they stop at a minimum size and at the screen. The pointer shows resize arrows on the edges; the move arrows only appear while you hold the title bar. Reset window positions also resets sizes.
- Exe: after opening the Music window's song list near the bottom of the screen, you can still drag the window.
- KovaaK's graph: the lines rise up from the bottom in a quick animation, and Score is drawn on top, then Accuracy, then Dmg Eff and the rest. Switched-off line buttons are easier to read.
- Mod menu: Reset all settings. Temporary shows every setting at its default until you press Restore or close the game (your account isn't touched); Permanent resets this PC and your account's saved settings after you type CONFIRM. Scores, replays and your login stay.
- Exe: the Graph window keeps the same size when you move the Replay window up or down (it used to stretch).
- Exe: Settings > Video > Graphics Quality has GPU Resident Drawer (off by default). Off is steadiest on most PCs; on may help if your CPU is the bottleneck. Try both on your PC.
- F11 switches between fullscreen and windowed (in the exe it goes back to your fullscreen or borderless mode). Settings > Video follows it.
- Exe in a window (not 1080p fullscreen): the KovaaK's graph lines, the replay trail, the replay crosshair and a few animated texts no longer fly off to the wrong place.
- Gridshot 3x3 and the other tasks in the indoor room: the platform (the stage) now reaches both side walls, so there's no gap into the void at its ends.
- Gun: Bullet hole duration setting (Range and Skirmish). 0 by default, so there are no bullet holes; type up to 12 seconds (how long they lasted before). They fade over the last 2 seconds.
- Music player (Settings > Audio): previous song and next song buttons (double arrows) on each side of play / pause.
- Video: Frame rate limit is now Limit FPS Always (on / off, off by default) with Max FPS Always below it, where you type the number (20–1000). Max FPS in Menus is typed too, and greys out while its limit is off.
- Sniper Scope: the scope's centre dot can be turned on or off, with its own colour, opacity and thickness.
- Aim Down Sights: Use Base Crosshair for ADS (on by default), or give ADS its own crosshair (colour, outlines, centre dot, inner and outer lines), with a button to copy your Primary settings into it. It shows while aiming down sights with non-scope guns.
- Crosshair settings have sub-tabs like Valorant: General and Primary. General has Use Advanced Options (off by default); turning it on adds Aim Down Sights and Sniper Scope.
- Settings: windows (Replay, Graph, Playlist, Music, chat and the rest) hide while Settings is open and come back exactly where they were when you close it.
- Settings > Video now has three sub-tabs like Valorant's: General (display, frame rate, the new Limit FPS in Menus, on at 60 by default), Graphics Quality and Stats. The stats text at the top sits in light boxes, like Valorant's.
- The FPS counter in the bottom left is gone: Client FPS now shows at the top left by default (Settings > Stats, Text Only; set it to Hide to remove it). The crosshair's hit / miss colour (green / red) is off by default.
- Replays: your gun now moves with the replay's view (it used to stay hidden or stuck where the live camera was).
- Exe: fewer lag spikes. Unity's garbage collection now runs a little at a time (incremental GC) instead of freezing the game for a moment, the map, pings and stats overlay no longer make garbage every frame, and the Stats tab has GC Runs to show when one happens.
- Range bots are bigger: 1.96 m tall like an agent (they were 1.85 m). The Range has no map (pings still work there).
- The Range and Skirmish now share the same basic mechanics: pings (Z, with the ping wheel) work in the Range too, on top of the movement, jumping, heights, crouching and guns they already shared. Any new mode you move in gets them as well.
- Pings in Skirmish (Z), like Valorant: tap Z to ping where you're looking (walls, crates, the floor, even up in the air); it shows the place's name and how far it is, updating as you move. If it's 3.10 m or less above the ground straight below it, a thin line drops to the ground with the name and distance at the bottom. Hold Z for the ping wheel (after 130 ms): move the mouse like a joystick to pick Caution (up), On My Mark (left), Watching Here (right) or Need Support (down) and let go of Z to send it; right click cancels. Your teammates see your pings, on the map too, and the minimap now shows the name of the place you're in.
- Walking and crouching speeds like Valorant: walking is 60% of your running speed (4.05 m/s with the knife), crouching 35% (~2.36 m/s). Your body is 1.96 m tall for bumping into things (1.37 m crouched), so you can crouch under lower gaps.
- Your character is now 1.96 m tall like every Valorant agent (about 1.37 m crouched): your eyes sit at 1.82 m standing, like Valorant, and 1.23 m crouched, and other players' models in Skirmish are the same size.
- Skirmish E rebuilt from the real overhead map: a crate row in front of each spawn (a crate, a tall double stack and a sandstone block, with a step crate behind), a sandstone block in the corner, and on each side a ramp along the wall up to an L-shaped crate ledge with a tall wall block at its end and step crates beside it. Heights match too (a crate is 1.96 m, an agent's height; a step is half that, the sandstone 1.5 crates, the double stack 2, the tall block 3): jump onto a step from the floor and onto a crate from a step.
- Skirmish has a map now: a round minimap at the top left, and M opens the bigger map in the middle (press M again to close it). It turns with you by default; switch it to Fixed in Settings > Controls > Interface > Minimap. Teammates show on it.
- Jumping moves your hands like in Valorant: they dip a little as you take off, float up while you're in the air and drop when you land, then settle. It works with every gun and knife, even while inspecting or aiming.
- Skirmish is much less laggy: players now connect straight to each other (like the aim tasks) and send where they are about 30 times a second instead of 10, with hits arriving the moment they land. If a direct connection can't be made, that player goes through a fast relay server in Asia instead (and through the database only if that's down too). The bottom-left corner shows Direct, Relay or Via server, and the Tab board shows the real player-to-player ping (⇄) when connected directly.
- The Range is wider (34 m across instead of 24), the distance lines and their labels are gone, and the floor has Valorant-style glowing lines: one down the middle, two fanning out diagonally from the table's ends, and one running across the whole hall in front of the table. Bots can appear further out to the sides.
- View kick per gun: heavy single shots kick the screen up much harder now (Sheriff, Operator, Outlaw, Marshal, Guardian, shotguns, Bandit, Ghost), and every kick settles in the same time, so the difference is easy to feel. Rifles and SMGs (Vandal, Phantom, Spectre…) feel the same as before.
- Skirmish: when a wall or crate is behind you as you die, the camera now stops calmly in front of it instead of jumping back and forth as you look around. Ramps no longer shove you off when you walk near their side edges; like crates, you stay on until most of you is past the edge.
- The Range and Skirmish: firing kicks the screen up again. Every shot punches the view up for a moment and a long spray lifts the view by about a third of its climb (the bullets still follow the full recoil).
- Headshots are animated now instead of one picture: a white-hot flash, a starburst of spikes that shoots out and twists back in, a shockwave ring, electricity crackling round the head and the fire spark (three flame lines shooting up, flickering) with hot sparks flying off.
- The Range: bots that die blow up now, timed like Valorant and animated every frame (no more blue flash): the bot glows orange, billowing fireballs on the head, chest and hips gone in about 0.14 s, a burst of white-hot spikes from the head, electricity crawling round the legs, body and shoulders, and three flickering flame lines on the head (the middle one brightest) that fade by 0.38 s. Then just 2 dark shards and 3 gears drop to the floor and vanish after about a second.
- Bullet tracers are always on in the Range and Skirmish (the Bullet tracers setting is for aim tasks).
- Create account: the username and password rules are shown under each box, plus Passwords don't match under Repeat password. Whatever isn't met turns red when you press Create account.
- Multiplayer: your mic starts muted in every room. Press U (Mute / Unmute Microphone, Controls > Communication) to talk. Push To Talk is a keybind there too (V).
- Multiplayer: everyone's ping (ms) shows in the room lobby and on the Tab boards.
- Multiplayer: hold Tab in any room (aim tasks or Minecraft, waiting or playing) for a scoreboard with everyone's score and ping. The Skirmish Tab board has a Ping column too. Show Scoreboard (Hold) is a real keybind now (Controls > Interface).
- Skirmish: players and bots block each other now; you can't walk through anyone alive.
- Skirmish: a death animation. Bodies are knocked back away from whoever shot or knifed them and fall flat.
- Skirmish: you see everyone's bullet tracers now (enemies in red, teammates in blue), even with your own tracers off.
- The ▶ (watch replay) button only shows on players who actually have a replay of the score shown.
- Results screen: LEADERBOARD, ANALYSIS and PLAYLIST switch the right side like KovaaK's, with LEADERBOARD open when the round ends. The leaderboard there shows the whole top 50 (scroll).
- Click any player on a leaderboard (results screen or the Leaderboard screen) for their leaderboard entry: rank, score, game version, date, percentile, time to kill, accuracy, sensitivity, cm/360, FOV, resolution, average FPS, time paused and pause count. These details are saved with every new personal best from now on.
- The classic results card is back as the default. The KovaaK's-style results screen is an option: Settings > General > Results screen.
- fuglaaPressure is 120 seconds in KovaaK's; here it defaults to 90 s, the longest duration.
- Matty Routine 1 - Statics is now complete too: Pokeball 1w4ts 30%, 1wall 5targets small Raspberry, 1w2ts reload, fuglaaPressure, 1w4ts Voltaic and VT 1w3ts Rasp Advanced. Each one has its own map, targets, gun, magazine, scoring and leaderboard, like in KovaaK's.
- Credits: kya is now credited as Co-creator. Testers: Smiley Mehh and PotatoInSpace. Thank you!

### Fixed

- A bullet mark on the edge of a box is clipped to the box, so it no longer hangs off into the air
- Fixed: after Reset all settings, opening Settings > Audio spammed errors and the music player there lost its time and seek bar.
- Windows: a window under another one no longer darkens or lights up when your mouse is over the top one; it just can't be clicked through.
- Exe: Reset all settings (Mod menu) no longer leaves you with an empty sky; the game comes back with the defaults.
- Headshots no longer show the circle (shockwave ring) coming out of the head; the flash, starburst and fire spark stay.
- Multiplayer: fixed switching to Skirmish right after a round (or after a cancelled match). The finished round's 3D scene stayed behind the room, so the room creator got stuck on CLICK TO BEGIN and the other player on a countdown with no mouse or Esc. Now everyone leaves the round's scene first, and no new aim match can start while the room is moving.
- Multiplayer: fixed players showing as offline (with 3 or more players, or with the game in a background tab) while they were still in the room. (offline) is red now.
- Multiplayer: fixed the room getting stuck on aim tasks when the room creator switched to Skirmish (or Minecraft) while another player was already Ready.
- Skirmish: when you die the camera no longer sinks to the floor. It eases back and up behind you, looking 20° down, and stops there.
- Leaderboard replays are fixed: long tracking rounds (like Amare GarfMicroTS) were too big to upload, so their replays were never saved. Replays are now zipped and moving targets are recorded 125 times a second. If a replay still can't be saved, the results say why.


# v1.9.1

### Changed

- Settings makeover, like Valorant's: full screen with tabs along the top (General, Controls, Crosshair, Colors, Video, Audio), one row per setting that lights up under the mouse, grey option buttons with a cyan edge on hover, dropdowns, thin sliders with a diamond knob that turns cyan, and CLOSE SETTINGS at the bottom. Crosshair and Colors are tabs now. On / Off settings switch only with their buttons (clicking the row does nothing).
- Every button gets Valorant's hover look: a green fill with a thin bright cyan edge (it fades in). Boxes and dropdowns get a cyan border under the mouse. In the Range, spraying and running and gunning no longer move your view or the crosshair: it stays in the middle and only the bullets climb and spread, like Valorant.
- Crosshair profiles: keep up to 5 crosshairs and switch between them from the dropdown (Create New Profile, Delete, Duplicate, Rename). Import and export Valorant crosshair codes (like 0;P;c;5;h;0;0l;4;0o;2;0a;1;0f;0;1b;0): Export copies this crosshair's code, Import makes a new profile from a code.
- Controls: every action can have two keys (a second box next to the first; Backspace clears a box). A key can be on more than one action like Valorant: an orange warning shows on the action, under its tab, and the list of conflicting bindings is on the right. The Controls tabs look like Valorant's (underlined text).
- Multiplayer scores exactly like single player now (speed points on Gridshot tasks, accuracy multipliers on the KovaaK's tasks, and so on). New room setting: Accuracy penalty (On: misses cost points, or your accuracy multiplies your score; Off: misses are free). Each task starts with its own setting, and the room creator can switch it. Hold-to-fire tasks never have it.
- Amare GarfMicroTS: bullets that miss leave a faint light ring on the back wall, like KovaaK's; each one fades away over 7 seconds.
- Multiplayer: no more Aim tasks / Skirmish / Minecraft buttons before you make a room. Create a room first; inside it the room creator picks the game (Aim tasks, Minecraft or Skirmish) and can switch any time in the lobby. Everyone in the room moves along, and the room code stays the same.
- Crosshair profiles work like Valorant's: a label follows the mouse over each icon; Delete and Duplicate ask in a pop-up (a duplicate is named Copy of …); Export copies the code straight away (the label says Profile copied to clipboard); Import opens a pop-up to paste a code into; Edit makes the name in the dropdown typable. GarfMicroTS wall marks now stay for 5 seconds and fade out smoothly by 7, and a long spray no longer removes older marks early.


# v1.9

### Added

- Updates (Windows): when a new version is out, the game downloads it by itself with a progress bar, installs it and starts again (no itch.io visit).
- osu! 3D: a new task. Numbered circles pop up on the wall with an approach ring closing in; click as the ring meets the circle (300 / 100 / 50 for timing, or a miss). Sliders: hit the start, then hold left-click and keep the crosshair on the ball to the end. Combo, osu! accuracy, max combo, and its own leaderboard.

### Changed

- The download comes with a READ ME that explains how to unblock it on Windows (Properties > Security > Unblock).
- Resuming from pause picks up right where you left off (no more 3-second countdown).
- KovaaK's tasks (every playlist task) start the moment you press Play or restart: no CLICK TO BEGIN and no countdown, like KovaaK's. Multiplayer rooms still have CLICK TO BEGIN and the countdown.
- Voice chat in multiplayer rooms and Skirmish: you hear everyone in the room. Settings > Audio > Voice chat: Open mic (default), Push to talk (hold V) or Off, plus a voice volume. Bottom left shows your mic and who's talking.


# v1.8

### Added

- New bottom HUD in the Valorant style (Range and Skirmish): health with a shield icon left of the middle, ammo right of the middle, in thin angled frames. Health fills red at 40 or less, the ammo when the magazine is under 35% full.
- Leaderboard replays: when you set a new personal best on an account, its replay goes on the leaderboard too. Press ► on a player's row (leaderboard or score card) to watch their replay, music and all.
- 6 new songs in the music playlist: Band4Band (Central Cee, Lil Baby), It Ain't Me (Kygo, Selena Gomez), Grenade (Bruno Mars), Party Rock Anthem (LMFAO), Again (Fetty Wap) and GGEZ (Kaien Sugar, M.Sasuke).
- Colors: new Floor tab. Pick two checker tile colors for the floor (each can be a gradient), or a preset (Light, Dark, Sand). It colors every task's floor (with map theme colors off), the Range and Skirmish.
- 7 new songs in the music playlist: Like Him (Tyler, The Creator, Lola Young), Locked Out Of Heaven (Bruno Mars), New Person, Same Old Mistakes and Eventually (Tame Impala), Chicago (Michael Jackson), Rocketeer (Far East Movement, Ryan Tedder) and Impostor Syndrome (Sidney Gish).
- 7 more new songs in the music playlist: I Really Want to Stay At Your House (Rosa Walton, Hallie Coggins), Habang Buhay (Gawr Gura cover), E85 (Don Toliver), hate that i made you love me (Ariana Grande), Circles (Post Malone), No Other Heart (Mac DeMarco) and EVERYTHING (The Black Skirts).
- New tasks: Minecraft Button Wall (Easy) and (Medium). A flat world and a 7 x 4 white wool wall with 14 button spots (3, 4, 3, 4 from the bottom). Like Gridshot, a few buttons are up at once (5 on Easy, 3 on Medium): press one and a new one comes up on another spot. 1 point per press, each with its own leaderboard.

### Changed

- Mod menu: Door knock. Send a knock from the left or the right to the players you pick; it plays on their side with no image (Hear left / Hear right to test it on yourself).
- Removed the damage numbers that popped up over targets when you hit them.
- Air strafing redone from a frame-by-frame study of a 60 fps recording (keys, mouse turn and speed): hold A or D (W can stay held) and turn the mouse the same way to curve with your view and gain speed, about +0.3 m/s per jump for a 70-80° turn, even past run speed. Turning fast no longer slows you down.
- The mouse wheel scrolls the Songs list and the Music window's song list again (it used to scroll the page behind them).
- Headshots also send up a vertical flare: a fan of white-gold flame spikes shooting straight up from the hit, on top of the spiky burst.
- Landing: no more slide. Let go of the keys when you land and you stop like normal. Jump again right away (within 0.08 s) and you keep all your speed for bunny hops; only staying on the ground longer while holding a key slows you down for a moment.
- Headshots are much more alive: a white-hot flash and a second bloom that lifts, a big orange halo above the head, a fan of sparks shooting up and arcing back down, dark shards that tumble and fall, glowing embers drifting off and lightning crackling below, on top of the burst and the vertical flare (all bigger now).
- Range: practice bots stay plain grey whatever the difficulty (the colours are only for START). START has no countdown any more; the bots come after 1 second.
- Music: every song in the Songs list and the Music window has an on / off switch. Songs you switch off are skipped by next / previous and when a song ends (you can still play one by clicking it). Saved to your account.
- Minecraft has its own leaderboard now (1 point per button, misses cost nothing), like the other tasks.
- Knife animations redone from a recording: left click is a combo of 3 different slashes (cut across to the left, rip upward, wide backhand to the right) that goes back to the first one if you wait 1 second; right click is a heavy two-handed overhead stab; the Tactical Knife inspect shows the blade face, the edge and the side (2.8 s), and pressing inspect again restarts it.
- Armory: the Karambit is now a skin of the knife (click the knife, pick Default or Karambit on the right, like the Vandal's Ion). The details on the right follow your mouse; when you're not over anything they show the last weapon, shield or knife you clicked (or nothing). Aiming down sights keeps your crosshair at the same size (only sniper scopes hide it).
- Air strafing works in every direction: whichever key is most sideways to your motion is the strafe key (A / D when you move forward or back, W / S when you move sideways), and holding the other keys too costs nothing. Changing keys mid-air without the mouse no longer kills your speed (a key against your motion only brakes gently).
- Marshal and Operator come out of the scope after every shot (aim again for the next one); the Outlaw stays scoped.
- Sniper rifles (Marshal, Outlaw, Operator) come out of the scope instantly; going in is still animated.
- Air: pressing two keys at once where one points back against your motion swings your momentum 90° to the other key (going forward, S+D = straight right, S+A = straight left; going right, S+A = straight back), losing about 1 m/s; a single key (A or D) still only nudges you. Works from any direction.
- Leaderboard: the 1.0 (old scoring) choice only shows for task and duration boards that actually have 1.0 scores; the empty ones are gone.
- Colors > Floor on KovaaK's maps: they keep their own floor texture. Default leaves it as it is, Light / Dark gray make it lighter / darker, and a custom color tints it (like the background does to their walls).
- The Bucky pumps and the Marshal / Operator work the bolt after every shot, so you can see when you can fire again.
- Marshal / Operator: you can't scope while it's racking after a shot. Hold aim (or press it) during the rack and it scopes as soon as the gun is ready.
- Karambit: a second knife (Armory > Melee), with a hooked blade and a finger ring. It spins around the ring when you pull it out, and Inspect (Y) lifts it, turns the blade to you and spins it twice. Inspect works on the Tactical Knife too.
- Movement tuned to a frame-by-frame recording: jumps are higher and longer (1.15 m, 0.67 s), running speeds up along a curve (about 0.45 s to full speed), landing slows you down for a moment (jump again right away to keep your speed), and air strafing (hold A or D and turn the same way) adds a little speed.
- Skirmish: other players crouch properly (knees bend, hips drop, feet stay flat) instead of being squashed.
- Scoped guns (Marshal and the others): no more hitch the first time you aim; the scope picture is made in the background when you equip the gun.
- Stinger and Bulldog fire bursts while aiming down sights (Stinger 4 bullets, Bulldog 3), like Valorant.
- Knife (3): Range and Skirmish. Left click slashes (50), right click stabs (75), double damage from behind; you run faster with it out. 1 = rifles and other primary guns, 2 = sidearms, 3 = knife (Settings > Controls > Equip Melee Weapon), and the mouse wheel cycles all three.
- Lyrics: faster to find (LRCLIB's own copy first) and they try again by themselves when lrclib.net can't be reached for a moment.
- Replays play the music too: the song that was playing, from the same moment in it, and it changes when the song changed during the run. It plays with the replay sound on at x1 (your own music goes quiet meanwhile). If the player had lyrics on, they show inside the replay picture. Songs someone added themselves don't play for others.
- Song search: a search bar in the song list (Settings > Audio) and in the Music window's song list. Type part of a title or an artist.
- Lyrics: synced lyrics on the left side of the screen, also while you play. The line being sung is lit up and its words light up one by one as they're sung. They're off at first: turn them on with the lyrics button in the Music window or in Settings > Audio (saved on your account with your audio settings). Lyrics come from LRCLIB (lrclib.net) and are kept on your PC after a song's first play; songs without lyrics there (or instrumentals) show none.
- Replays have sound now: the shoot and hit sounds play along. It starts muted: the speaker button next to the time turns it on, and hovering it shows a volume bar. A saved replay file keeps the sounds it was played with, your own sound files too (up to 5 seconds each). Replay files from the web version play their sounds here too.
- Image crosshair in the downloaded game: now in Settings > Crosshair too. Pick a picture, add one by pasting its path (Shift + right-click > Copy as path) or press RELOAD FILES after putting PNG / JPG files in the Crosshairs folder; new files show up when you open the screen.
- Image crosshair: opacity, and move the picture (X / Y sliders, or drag it in the preview). The preview shows a red cross on the exact middle of the screen so you can line it up, and you can turn on a small center dot in game. JPG, WebP and GIF pictures work too.
- Minecraft replays now show the world you played in (with every block you broke or placed), the buttons where they really were, and you walking around, instead of whatever world was loaded.
- Minecraft Button Wall: you stand still and only aim, like Gridshot (no walking, jumping or sneaking).
- MICRO GOLD MINE playlist: its first 4 tasks are playable now, made from their KovaaK's files: Amare GarfMicroTS (track tiny jumping dots in a small tunnel: 50 bullets on one kills it, but it heals if you stop for 0.2 s), Pokeball 5 Sphere Hipfire Extra Small (drill 5 tiny targets on a sphere around you), eth 1w4tes Micro (4 tiny targets far down a tunnel, a 3-shot pistol) and waldoTS (track 3 strafing balls; 0.01 points per damage). Each has its own leaderboard.
- Range: the crates, the stairs and landing, the wooden posts, the desk and the skills-test screen are solid now. You bump into them and can stand on them (jump onto the crates and the desk), and bots never appear on a crate.
- Range: a bot you kill flashes blue and is gone at once (it stays standing, no falling over or waiting).
- Amare GarfMicroTS: the square frame is one connected box with cut 45° corners inside and out (like KovaaK's), and the whole map sits where KovaaK's has it (the frame is in the middle of your screen, not above it).
- Playlists: pressing play in the Playlist window while you're in the Range now leaves the Range and goes to the task (it used to load the task inside the Range).
- Knife: the hit lands when the blade does in the animation (the punch, the upright rip, the swing to the right, the heavy's slam), not the moment you click.
- Range: the distance lines and lane lines on the floor are raised strips a few centimetres high (you walk straight over them).
- KovaaK's colors matched to KovaaK's screenshots: the white bricks and tiles are a lower, softer white with faint mortar lines (every task that uses them), Amare GarfMicroTS has its big dark pipes coming off the back wall, eth 1w4tes Micro has a warm paving-brick floor, waldoTS walls and the blue sky are closer to KovaaK's.
- MICRO GOLD MINE maps in their KovaaK's colors: Amare GarfMicroTS (gray walls, dark trims, light tunnel), eth 1w4tes Micro (gray panels with dark joints, dark ceiling, gray tiles), waldoTS (gray room under a blue sky). KovaaK's white bricks and tiles are a softer white now (no glare), on every KovaaK's map.
- Amare GarfMicroTS and waldoTS: a health bar shows above a target while you're hurting it (a plain orange-and-dark bar, like KovaaK's), and goes away when it heals (like KovaaK's).
- Knife animations redone to match Valorant's: you hold the knife low on the left with the blade pointing right and your free hand open on the other side. Left click is a combo of 3: a punch forward from the left, the knife brought up upright in the middle, and a swing out to the right. Right click swings up to the right, both hands meet up high, then slam down. Inspect holds it upright, lays it flat pointing right, then raises it edge-on. Every move flows smoothly from wherever the last one left off.

### Fixed

- Jumping needs a new press of the jump key every time: holding Space no longer jumps again when you land (let go and press again). A press just before landing still counts.
- Air strafing works like Valorant instead of CS: holding W no longer weakens it. A or D steer on their own in the air, so W+A or W+D while turning curves you and gains speed right away.
- Pressing the key for the weapon you already hold (1 rifle, 2 sidearm, 3 knife) no longer draws it again.
- Landing no longer locks your direction: it only lowers your top speed for a moment, and A / D (or any key) steer you right away like on normal ground.
- Range: bots no longer flash red when you hit them.
- Replays (downloaded game): fixed extra targets in the replay picture; it never shows more targets than the task has.
- Range: the distance lines and lane lines on the floor no longer flicker or break up into dashes far away.


# v1.7

### Added

- New aim-down-sights pictures: the rifles, SMGs and machine guns show a thin yellow octagon (bigger on guns with more zoom) with the gun below it; Warden, Marshal, Outlaw and Operator each have their own scope (tube, housing and reticle).
- New Vandal skin: Ion (Armory, under the Vandal's stats). White and navy with glowing blue lines, an electric ball spinning in the receiver, a blue muzzle flash and blue tracers.
- New task: Minecraft. A blocky world with natural terrain (hills, lakes, beaches and trees). Walk, sprint, sneak and jump like Minecraft, and press the black buttons (left click, from any distance): 1 point each. Break blocks (left click, in reach) and place them (right click; 1-9 or the wheel picks the block).
- 5 new songs in the music playlist: She Bugging (Khantrast), You're Welcome (Dwayne Johnson), Just Friends (Hayden James), YELLOW (Yoh Kamiyama) and Forget (Pogo).
- New chat like Valorant's: just a see-through "Global:" bar in the corner. Hover it and the messages open above it instantly (and close the moment you move away) (scroll with the wheel); the pin keeps it open. It stays in the bottom-left corner (it can't be moved). A red dot shows new messages while it's closed.
- 6 new songs in the music playlist: BAD (ATEEZ), Panini (Lil Nas X), Earrings (Malcolm Todd), Everything I Am (Kanye West), Wake (Hillsong Young & Free) and the Pepito Manaloto Theme Song (Michael V.).
- New players start with All Dropping 8 Bit Beats as their song.
- Range: new training bot: a slim grey robot with big shoulder pads, a chest plate, a thin waist and a narrow head with a visor slit, every armour piece outlined in yellow. It stands with its elbows bent and its open hands up in front of its chest. Head, body (arms count as body) and legs still take their own damage.

### Changed

- Every shotgun pellet has its own tracer (Classic right click, Shorty, Bucky, Judge), not just one.
- Bullet tracers work like Valorant: each bullet is a short, very fast streak that flies to where it lands in a couple of frames (no line left hanging). Default skins fire yellow tracers.
- Multiplayer: Minecraft rooms. Next to Aim tasks and Skirmish: 2 to 10 players in one shared world (the same terrain for everyone, web and the downloaded game together). You see everyone walking around with their name above them, and blocks anyone breaks or places change for everybody. The room creator picks the buttons: Own buttons (the default, everyone has their own 3) or Shared buttons (the same 3 for everyone, first to press one gets the point). Timed or first-to, with the live scoreboard and a winner at the end.
- You can jump while crouching (you stay crouched in the air).
- Hit effects: a short orange flare on the body and a white-gold burst on headshots (0.25 s), with tiny lightning flickers.
- Range bots: when you eliminate one in practice another appears somewhere else straight away; bots appear at once (no rising out of the floor) with a quick blue flash when they appear or go.
- Range screen: much bigger, standing on the floor in front of the desk like Valorant's, with AIM SENSITIVITY on it: shoot the small – / + boxes for one step, the big ones for ten.
- Skirmish is in the downloaded game too: Multiplayer → SKIRMISH. Teams of 1 or 2 on the Warehouse map (E), a buy phase in your spawn room, first to 10 rounds, bots for empty places, Tab for the scoreboard. The map has the same warm warehouse lighting as the web version. Rooms work across the web and downloaded versions.
- Shorty, Bucky and Judge use a circle crosshair like Valorant: a thin ring the size of the pellet spread (it grows while you move) with a dot in the middle.
- Recoil now lifts the whole view like Valorant: spraying climbs the screen (about 3-4° on rifles, 5-6° on the Ares and Odin) and every shot punches the view up for a moment, then it settles back when you let go. The crosshair shows the rest of the spray.
- Bucky and Marshal reload one round at a time, and you can fire to stop the reload.
- Classic: right click is a shotgun blast (3 pellets, 2.22 bursts a second, 3 rounds a blast).
- Aim down sights is animated: the zoom eases in, the gun comes to the middle, and each gun has its own sight picture (iron sights on the Vandal, a holo sight on the Phantom, Spectre and Stinger, a red-dot tube on the Bulldog, a ring on the Guardian, a heavy ring on the Ares and Odin, and its own scope on the Warden, Marshal, Outlaw and Operator).
- Weapons: every gun has its own spray pattern. It climbs, then sways side to side, and the crosshair moves with your spray like in Valorant.
- In the Range the game keeps going while a menu is open: you fall back down after a jump instead of hanging in the air. In the Armory you can still move and jump (WASD, Space) while you shop; in the settings and pause menus you just can't move until you close them.
- Armory: laid out like Valorant's buy menu (same places and sizes), every weapon shown with a picture of its own model. Bot armor moved to the Range settings (F3).
- Range settings (F3): Speed (Easy / Medium / Hard), Streak (Eliminate 50 / 100: a timed run), Bots (Strafe on/off, Reset), Bot Amount (1, 5 or 10), Bot Armor and Infinite Ammo. A Shooting Range panel on the left shows the current settings. Defaults: Medium, 5 bots, bot armor on, infinite ammo off.
- Range Skills Test: shoot START on the console. 30 bots pop up one at a time and stay up for a short time (Easy, Medium or Hard; on Hard they strafe). SCORE counts your eliminations, REMAINING the bots left. Shoot EXIT to stop, Practice to go back to the normal bots.
- Range: rebuilt like Valorant's range: warm plaster walls, wooden posts and a wooden roof with trusses, windows, stairs, a desk in front of you with the Skills Test console, and a big SCORE / REMAINING screen hanging over the hall.
- In the Range (and Skirmish and any later mode where you move, once they come to the exe), Show gun and Muzzle flash are always on; their settings show ticked and locked there, and your own choice still applies everywhere else. Bullet tracers always start on there too, but you can switch them off while you're there; when you leave, your own Bullet tracers setting comes back.
- Pressing B again closes the Armory, and Esc closes the Armory or the pause menu (back to the game) instead of opening another menu.
- Music effect (Settings → Audio): Off, Dance studio or Bathroom at a party. Dance studio is tuned from a phone recording of a song played in a dance studio (thin bass, boomy low-mids, a nasal 1 kHz peak, dull highs and the room's echo). Bathroom at a party is tuned from a real "you're in a bathroom at a party" edit: the music is heavily muffled (almost nothing above 1 kHz) and swims in a long, wide echo. Switch any time, even mid-song.
- Audio now starts at All music 4, Menu music 10, In-game music 10, with Mute music when game window out of focus off. Settings you already changed stay as they are.
- Every gun now has its own model and its own reload. Each of the 20 guns is shaped differently, held in gloved hands, and sized like a real first-person view: rifles are big and reach toward the middle of the screen, pistols sit small in your hand. Reloads follow the gun: pistols tip over and swap the magazine; rifles, SMGs and the Judge swap theirs with your other hand; the Sheriff swings its cylinder out; the Shorty and Outlaw break open for new shells; the Bucky and Marshal load one round at a time; the Ares and Odin lift the lid and swap the box. All timed to each weapon's reload time. Equipping a weapon raises it into view over its equip time. The tasks use the Classic and the Vandal models.
- Range: Valorant-style movement. On the ground you speed up quickly and stop hard when you let go or counter-strafe. In the air you keep your momentum, and holding A or D while turning the mouse the same way curves your jump (air strafing); steering never adds speed. Bunny hopping: hold jump (or press it just before landing) to hop again the moment you land, with no cooldown and no speed lost. Jumps are the same height at any frame rate, and walls stop you instead of holding you against them. Landing makes you a little inaccurate for a moment (it shows on the Shooting Error graph).

### Fixed

- Range difficulty colours: Easy bots are grey, Medium red, Hard purple. Hard no longer strafes.
- Crouching in the air no longer drops your view: your legs tuck up and your head stays where it is (like Valorant), so you can crouch-jump onto higher things.
- Range: Retry (the pause menu button or `) no longer starts a task round with the 3x3 balls; in the Range it refills your guns and clears the holes.
- Shorty, Bucky and Judge: the crosshair no longer spreads out with the pellet spread (like Valorant).


# v1.6

### Added

- 20 new songs in the music playlist: Folded, The Thrill, Duvet, Aruarian Dance, Feel Good, Ghosts, Heartless, Inspiration, Chill Day, Blue Boi, Everyday Hustle, Here (Lucian Remix), Chopin's Nocturne Op. 9 No. 2, Satie's Gymnopédie No. 1, Middle, Memories, How Deep Is Your Love, Cold Heart (PNAU Remix), Summer and Where Have You Been.
- New Range (ENTER RANGE on the main menu): walk (WASD, Shift to walk, Ctrl to crouch, Space to jump), buy any Valorant gun or shield in the Armory (B) and shoot bots or the wall. Each gun has Valorant's first-shot spread, firing error that grows and recovers, movement / jump / crouch spread, aim down sights, recoil, magazine, reload and damage by distance. A Shooting Error graph shows your spread live; bullet holes stay on the wall for a few seconds.
- New Music window: play / pause, previous / next song, seek, volume, mute and a dark song list.
- New Windows button (top right, whenever your mouse is free): switch the Replay, Playlist, Music and Mod menu (mods only) windows on or off. Hold a window's title bar to move it anywhere on the screen (it stops at the edges); the game remembers where you put it. Reset window positions puts them back.

### Changed

- Settings > Keybinds is now Controls, with Actions, Equipment, Interface, Communication and Voxel Aim tabs. Controls the game doesn't use yet are listed and marked Coming soon. R (reload) in magazine tasks follows the Reload key.
- Crosshair Movement error and Firing error now follow your real spread in the Range (multiplier 0 to 3).
- The Mod menu is now a window, so it also works during a 1v1 (press Esc to free your mouse).
- 1v1: if the other player closes the game without leaving, they're taken out of your room after 15 s (closing the tab or the exe leaves right away), so the same code works again for them or someone else.
- Replay line: smoother (curved, with soft edges in the exe), a bit thicker on big screens, and red only when your aim moves slower than 5°/s.
- Fullscreen replay like Aim Lab: the enlarge button fills the whole window with the replay, with the timeline and buttons over its bottom edge (Esc goes back).
- The room creator picks the connection: Direct (players connect straight to each other with WebRTC when the networks allow it, falling back to the server) or Via server (everything goes through the database).
- Multiplayer rooms have their own Room chat: while you're in a room, the chat panel has Global and Room tabs (Room messages only go to the players in your room).
- 1v1 is now Multiplayer: 2 to 10 players in one room (the room creator picks how many, 4 by default; 9 or 10 can lag on slower PCs and connections). Everyone gets their own lane side by side, and only the players who joined get a lane. A live board shows everyone's points, and the results list everyone in order. Each player connects straight to every other player (WebRTC) when the networks allow it.


# v1.5

### Added

- Tracking tasks use a new automatic rifle (no recoil) and a big square room open to the sky.
- New task: Smooth Pill Voltaic (easy). A tracking task: a pill circles all the way around you and keeps changing direction. Hold left-click to fire; every bullet on the pill is 10 points and misses cost nothing.
- New setting: Muzzle flash (on/off), in Settings next to Show gun.
- New setting: First person handedness (left hand or right hand).
- New Audio tab (like Valorant's): Main volume, Sound effects, All music, Menu music and In-game music sliders, each with a mute button.
- New task browser: the Task box opens a scrolling list of every task (with search), and a Playlists tab. Open a playlist to see its tasks in order and pick one.
- New task: 1wall 6targets small (from KovaaK's, built from its scenario file). Six tiny targets on the wall of a grey grid room; 10 points per kill times your accuracy. First playable task in the Matty Routine 1 - Statics playlist; works in 1v1 too.
- New Field of view setting: Valorant (always 103), CS:GO (always 90), or None to pick your own from 60 to 140. Switching to None keeps the view you had.
- Voxel Aim has its own new hit sound.
- Colors: new "Use map theme colors" setting (on by default, saved to your account). Each task shows its own colors: the usual blue targets on the Aim Lab-style tasks, and red targets in a white brick room for 1wall 6targets small (like KovaaK's). Turn it off to use your own colors everywhere.
- New Keybinds tab in Settings: Shoot, Restart round, Next task and Previous task in the playlist (defaults: left click, `, ] and [). Saved with your account.
- New Video tab in Settings (like KovaaK's): Display and Render scale moved here, plus V-Sync, Frame rate limit, Anti-aliasing, Anisotropic filter, One frame thread lag and Pause on loss of focus. Saved on this PC.

### Changed

- Task names that don't fit their button slide sideways when you hover them.
- 1v1: Smooth Pill Voltaic works in 1v1 rooms. You both stand in the same spot and track the same pill; each bullet on it is 1 point.
- Music playlist: All Dropping 8 Bit Beats and Sleeping City by EZ TUNZ. Pick a song, play/pause, skip, loop one song or the whole playlist, and mute music when the game window isn't focused.
- Settings has General and Audio tabs, and a search box that finds any setting on either tab.
- Muzzle flash and Bullet tracers now start off (turn them on in Settings > General).
- 1v1 rooms, the leaderboard and single player all use the same task list, so every new task works in 1v1 too.
- First playlist: Matty Routine 1 - Statics (10 KovaaK's tasks, coming soon one by one).
- Settings > Audio: click the current song for a scrolling list of every song.
- Logged-in players keep their audio settings and their song on every PC (saved to the account).
- Audio starts at Main 100, Sound effects 20, All music 10, Menu music 10, In-game music 20.
- Music now loops the whole playlist by default.
- Song list: click the current song in Settings > Audio. Sort by Date added, Title or Artist, ascending or descending (default: Date added, oldest first). Next and the whole playlist play in that order.
- 15 more songs (17 in all), each listed with its title, artists and Slowed / Remix / Instrumental where it applies.
- A short clip can play as one long track (Metal Pipe Falling loops for 10 hours).
- Songs can stream from the internet: the song list comes from a songs.json file next to the songs, so new songs show up without a game update.
- Music player in Settings > Audio: play/pause, the time, a seek bar you can drag, and a mute button.
- 3 more songs: Metal Pipe Falling (10 Hours) by kya, Aria Math by C418, and Montagem Alquimia (Slowed) by h6itam, n7san7os, MC Menor Do Alvorada.
- Leaderboard: the Version choice (old scoring) only shows for the tasks that existed in v1.0: Gridshot Medium, Spidershot and Motionshot.
- Sensitivity: pick Valorant, CS:GO or Roblox next to it to see and type your sensitivity in that game's numbers (Valorant 0.204 = CS:GO 0.64872 = Roblox 0.01412). Your turn speed stays the same. Click the number to type it.
- Settings > Audio: pick the Shoot sound and Hit sound: Voxel Aim, Aim Labs or KovaaK's. Every shot now makes a sound, and hits add the hit sound on top.
- Your own background now also colors the platform top and the two blocks on Gridshot 3x3 (Easy), Gridshot Ultimate and Sixshot (no more dark line along the platform), and the front wall of 1wall 6targets small.
- Two more playlists (coming soon): MICRO GOLD MINE (15 KovaaK's tasks) and 2023 (9 KovaaK's tasks).
- Playlist tasks now stay in their playlist: the All tasks list only shows the regular tasks.
- Your own files (downloaded game): put songs, a shoot / hit sound or PNG crosshairs in the Custom folder (Settings > Audio > OPEN FOLDER) and press RELOAD FILES. They show up in the music playlist, as the YOURS sound and as Image crosshair.
- KovaaK's maps keep their textures when you use your own background: Default shows the map as it is, Light gray / Dark gray make it lighter or darker, and a custom color tints it.
- Playlists play like KovaaK's: pick a playlist task (or PLAY PLAYLIST) and a Playlist panel shows its tasks on the menus between rounds, with DONE marks and PREV / STOP / NEXT. The results card has NEXT TASK.
- Credits: special thanks to kya (shown on the What's new screen). Metal Pipe Falling is now credited to kya.
- The countdown and CLICK TO BEGIN stay in the middle of your screen wherever you look, with a shadow and an Aim Lab-style growing echo on each new second.
- Each task now starts with its usual round length when you pick it: 30 s for Gridshot 3x3 (Easy / Medium), Motionshot and Pokeball Frenzy Auto Small; 60 s for the others (you can still change it).
- Settings: shorter Sensitivity and FOV labels.
- Logged-in players now keep their game settings on every PC too: sensitivity game, FOV, handedness, show gun, muzzle flash, bullet tracers, show opponent, mouse polling rate and aim smoothing (render scale and the display mode stay per PC).
- Magazine tasks show your rounds as a bar that fills back up while you reload.
- 3 more KovaaK's tasks in the Matty Routine 1 - Statics playlist, built from their scenario files with their own maps and colors: Pokeball Frenzy Auto Small (hold to drill: 5 bullets in a row kill a target, or it heals), voxTS Static Click rAim (big open-top brick room, 3-shot magazine, every kill refills it) and VT Multiclick 180 Advanced (small concrete room, every kill gives 2 rounds back; kills x 10 x the square root of your accuracy).
- 1v1 connects you straight to the other player (WebRTC) when your networks allow it: aim and targets update ~30 times a second instead of ~12, with less delay. Bottom left shows Direct and your ping, or Via server when it falls back to the old way.
- The Replay and Playlist panels can be minimized with their - button.
- Replays: after every round (and every 1v1) a Replay panel on the left plays your run back like Aim Lab, with your aim as one thin line whose color follows your speed: red when slow or still, yellow while adjusting, green on flicks. SHOW HITS / SHOW MISSES add a dot or x for each shot (off by default). Pause, drag the timeline, x0.25 to x2 speed, or make it BIG. It opens after every finished round, even if you minimized it before. Replays aren't uploaded: SAVE REPLAY FILE keeps one in Custom/Replays, and OPEN REPLAY FILE plays one back (web replays work too).

### Fixed

- Fixed (exe): logged-in players whose account had saved game settings could not play (Play and 1v1 Ready did nothing).


# v1.4

### Changed

- Render scale now starts at 100%.
- "Show opponent" only appears in the 1v1 settings.
- Every screen has an X in the top-right corner, and Esc goes back.
- The pause menu is simpler: Resume, Retry, Settings, Change task.
- Settings is now its own screen: open it from the main menu, the pause menu, or Esc in a 1v1. Sensitivity, render scale, sound, gun, tracers, polling rate, aim smoothing, display, Crosshair and Colors all live there.

### Fixed

- Fixed: the version number no longer shows color code text when you hover it.
- Fixed: turning "Show opponent" off and back on during a 1v1 shows them again.
- Fixed: in 1v1 Motionshot the other player's targets now move.
- Fixed: in 1v1 the room creator saw the other player as "player" with no name color.


# v1.3

### Added

- 1v1: new 60-second win condition. First to 30 is now the default.
- New Colors screen: color your targets with a solid color or a gradient (linear, radial or diamond). Press on the preview for the Start point and drag to the End point; both points stay draggable, so any direction and angle works.

### Changed

- This changelog. Click the version number in the corner to open it.
- Desktop app: the pointer turns into a hand over buttons and a text cursor over text boxes.
- Global chat: players online count. Hover it to see who's on.
- Global chat: day dividers, AM/PM times, and dates on older messages (Philippine time).
- 1v1: lanes spread out to fit the bigger tasks; outdoor tasks give your opponent their own board.
- 1v1: Settings in the room and during a match (press Esc). The match keeps going while you're in there.
- 1v1: Copy code button in the room.
- 1v1: you stay ready if you press Esc, alt-tab or minimize while waiting; Not ready is a button in the settings.
- 1v1: Cancel match in the settings (Esc) sends both players back to the room lobby to change the task or win condition.
- 1v1: play any task from single player (Gridshot Easy, Medium, Ultimate, Sixshot, Spidershot, Motionshot). Every ball is 1 point and misses cost nothing.
- Desktop app: a full color picker (color square, hue bar, R G B and hex) for every color setting. Click any color square to open it.
- Your colors are saved to your account and show up in 1v1: your opponent sees your targets and background in your lane.
- Background colors: pick both checker tile colors, each one solid or its own gradient, with presets Default, Light gray and Dark gray. The gradient can run across the whole background or inside each tile. Turn on "Color all walls" to color the whole indoor range.
- Animated targets: any target gradient can flow (presets and custom colors).


# v1.2

### Added

- Update notice when a new version is out.

### Changed

- The gun now points at the crosshair.
- Global chat in the menus.
- Timed 1v1 matches count for your Gridshot Easy personal best.
- "Show opponent" setting to hide the other lane and save performance.
- Bullet tracers for you and your opponent (can be turned off).
- See your opponent: voxel or low-poly character with a gun, their name tag, their orange targets and their shots, in a lane beside yours.
- 1v1 duels with room codes: first to 30, 50 or 100, or highest score in 10 or 30 seconds.


# v1.1

### Added

- New app icon and a version number in the corner.
- New 1.1 leaderboards for every task. 1.0 scores are still there under Version.
- New tasks: Gridshot 3x3 (Easy) with 1 point per ball and free misses, Gridshot Ultimate (5x5) and Sixshot. The old 3x3 is now Gridshot 3x3 (Medium).

### Changed

- Desktop app: Fullscreen, Borderless and Windowed display modes.
- Crosshair editor (Valorant-style), saved to your account.
- Retry from the pause menu and the score card, or press ` any time.
- Misses now cost 3 points; faster kills earn 4 to 10 points.


# v1.0

### Changed

- Raw mouse input, sensitivity and render scale, polling-rate detection and aim smoothing.
- Online leaderboards, accounts with name colors, and numbered guests.
- First release: Gridshot, Spidershot and Motionshot in 10, 30, 60 or 90 seconds.

