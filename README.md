# Automatia Public Releases

Public release packages for the Automatia game.

<img width="600" height="400" alt="Screenshot from 2026-02-05 10-57-07" src="https://github.com/user-attachments/assets/d772bf97-8fa6-4410-a64f-c9a417d6c406" />

## Automated Release Publishing

- [Download for 64-bit Linux](https://github.com/fwsGonzo/automatia-releases/releases/latest/download/automatia-linux.zip)
- [Download for 64-bit Windows](https://github.com/fwsGonzo/automatia-releases/releases/latest/download/automatia-windows.zip)
- [Download for 64-bit macOS](https://github.com/fwsGonzo/automatia-releases/releases/latest/download/automatia-macos.zip) (NOTE: Needs tweaking)

## Mini player-guide

1. Edit config.json to set net_user to a nickname
2. Set net_uuid to a randomly generated UUID (remove dashes for now)
3. Set server_address to a public server IP (or keep localhost and run your own local server)
4. Start the client

If the client doesn't start up, run it in a terminal to get the reason. Try enabling compatiblity_mode in config.json.

Here are some commands you need to know:
1. Ctrl+F to toggle flying (R=down, T=up)
2. /w [world] to enter another world
    - `/w std`
    - `/w farms`
    - `/w winter`
    - `/w water`
    - `/w desert`
    - `/w limbo`
3. Shift+F1-F4 to control the sun
4. Shift+F5 to toggle debug lighting
5. Shift+F11 to toggle entity pivots and sector boundries

## Graphics settings

With a beefy PC you can:
- Increase `raycast_shadows` to 128, or even more to get large shadow rays from the sun
- Increase `multisampling` and `anisotropy` to 16 for smooth edges
- Enable `reflect_terrain` for terrain reflections
- Increase `viewdist` for instane view distances, at increasing RAM usage

You can increase performance by:
- Lower `viewdist` until FPS stabilizes
- Disable `raycast_shadows`
- Lower `multisampling` and `anisotropy` to 1 and 4 respectively

© 2012-2026 Alf-André Walla. All rights reserved.
