# Automatia Public Releases

Automatia is a game under development. It is a progression-based RPG with NPCs, story and multiple worlds. It can also be played co-operatively with other players in randomly generated worlds, like a sandbox.

<img width="600" height="400" alt="image" src="https://github.com/user-attachments/assets/f034aa7e-e2d6-4558-bad9-ed1b1ebb6beb" />

https://github.com/user-attachments/assets/89ec4535-8b79-4edb-8a37-78e292e246ff

## Automated Release Publishing

- [Download for 64-bit Linux](https://github.com/fwsGonzo/automatia-releases/releases/latest/download/automatia-linux.zip)
- [Download for 64-bit Windows](https://github.com/fwsGonzo/automatia-releases/releases/latest/download/automatia-windows.zip)
- [Download for 64-bit macOS](https://github.com/fwsGonzo/automatia-releases/releases/latest/download/automatia-macos.zip)

Note: On macOS you will need to `brew install` jemalloc.

## Mini player-guide

1. Edit config.json to set net_user to a nickname
2. Set net_uuid to a randomly generated UUID
3. Set server_address to a public server IP (or keep localhost and run your own local server)
4. Start the client

If the client doesn't start up, run it in a terminal to get the reason. Try enabling compatiblity_mode in config.json.

## Controls

### Movement

| Key | Action |
|-----|--------|
| WASD | Move |
| Space | Jump |
| Shift | Sprint |
| Ctrl | Crouch |
| Arrow keys | Look |

### Interaction

| Key | Action |
|-----|--------|
| Left click | Mine / interact |
| Right click | Place / use |
| Middle click | Copy block |
| Scroll wheel | Cycle hotbar slot |
| 1–9 | Select hotbar slot directly |
| Q | Drop item |
| Tab | Toggle building in air |

### Interface

| Key | Action |
|-----|--------|
| **Escape** | Open settings menu (also closes menus) |
| E | Open inventory |
| Enter | Open / send chat |
| F5 | Toggle HUD |
| F6 | Toggle minimap (press again to center, again to hide) |
| F7 | Open waypoints |
| F8 | Add waypoint at current position |
| Alt+Enter | Toggle fullscreen / windowed |

## Gamepad support

Automatia has full gamepad support out of the box. Plug in any Xbox or PlayStation controller and start playing.

| Input | Action |
|-------|--------|
| Left stick | Move |
| Right stick | Look |
| A / Cross | Jump / confirm |
| B / Circle | Close menu / back |
| X / Square | Inventory secondary action |
| LB / L1 | Transfer item (in inventory) |
| RB / R1 | Sprint |
| Left trigger | Mine / interact |
| Right trigger | Place / use |
| DPad | Navigate hotbar rows |
| Start / Options | Open inventory |

The gamepad deadzone and look sensitivity can be adjusted in **Settings → Controls**.

## Accessibility

Open **Settings > Accessibility** for:
- Color blindness mode with Protanopia, Deuteranopia and Tritanopia options
- Auto-jump over small gaps (on by default)
- Auto-jump-up to climb blocks when walking into them
- Toddler gamepad mode: restricts controls to movement, looking, jumping and building only
- Toddler auto-face: camera slowly turns to follow the movement direction

## Graphics settings

With a beefy PC you can:
- Increase `raycast_shadows` to 128, or even more to get large shadow rays from the sun
- Increase `multisampling` and `anisotropy` to 16 for smooth edges
- Use `supersampling` but be careful with values above 4x. 2x is visibly smooth!
- Enable `reflect_terrain` for terrain reflections
- Enable SSAO and shadow mapping
- Increase `viewdist` for insane view distances, at increasing RAM usage

You can increase performance by:
- Lower `viewdist` until FPS stabilizes
- Disable `raycast_shadows`
- Lower `multisampling` and `anisotropy` to 1 and 4 respectively

## Server admin Web UI

The server ships with a Deno-based web dashboard for server administration. Start it with:

```
cd webservice && deno task start
```

The dashboard provides player management, allow-list control, automation rules, audit log, backups, and live server logs. Configure access via the `AUTOMATIA_API_KEY` and `AUTOMATIA_API_URL` environment variables. TLS is supported via `deno task start:tls` with `TLS_CERT` and `TLS_KEY`.

## Blog posts

[Automatia Update: All Aboard!](https://libriscv.no/blog/all-aboard)

[Automatia Update: Sleeping with the Fishes](https://libriscv.no/blog/sleeping-with-the-fishes)

[Automatia: Update 5](https://libriscv.no/blog/automatia-5)

© 2012-2026 Alf-André Walla. All rights reserved.
