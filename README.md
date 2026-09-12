# Campy Camping — beta

A camping game for a few friends, played as dinosaurs, with voice that carries through the world:
closer is louder, walls muffle, tunnels echo. This is an early test build. Expect rough edges, and
tell us about them.

## Download

| Platform | Newest build |
|---|---|
| **macOS** (Apple silicon and Intel) | [campy-macos.zip](https://github.com/radical-beard/campy-beta/releases/latest/download/campy-macos.zip) |
| **Windows** (64-bit) | [campy-windows.zip](https://github.com/radical-beard/campy-beta/releases/latest/download/campy-windows.zip) |
| **Linux** (64-bit) | [campy-linux.zip](https://github.com/radical-beard/campy-beta/releases/latest/download/campy-linux.zip) |

Those links always point at the newest build. Older builds, and what changed in each, are on the
[Releases](https://github.com/radical-beard/campy-beta/releases) page.

## Before you play

- **Steam must be running and signed in.** Any account works. The game uses Steam to find the
  other players and to carry the connection; it does not need to be in your library.
- **A microphone**, if you want to talk. Voice is open-mic by default; press **V** in game to
  switch to push-to-talk (hold **T**).

## Running it

### macOS

1. Unzip. You get `project-campy-camping.app`.
2. The app is not notarized, so macOS will call it damaged or from an unidentified developer.
   Open Terminal, `cd` into the unzipped folder, and run this once:
   ```
   xattr -cr .
   ```
3. Open the app. macOS asks for microphone access the first time you talk; say yes.

### Windows

1. Unzip anywhere.
2. Run **campy.exe**. If Windows says it protected your PC: *More info* → *Run anyway*. The
   build is unsigned, that is all.

### Linux

1. Unzip. If the game will not start, `chmod +x campy.x86_64`.
2. Run **campy.x86_64**.

### Picking a session

The first screen lists every session that is up right now, with who is hosting and how many are
in. Click **Join** on one, or type a name and press **Host** to open your own; **Play alone** is
just you. If the host leaves, the game picks a new one and everyone reconnects in a few seconds;
nothing ends.

## Controls

| | |
|---|---|
| Move | **W A S D** |
| Sprint | **Shift** |
| Jump | **Space** |
| Look | mouse |
| Grab an item, or another player, into your hands | **right click** on it |
| Put down what you are holding | **right click** |
| Put the item you are holding on someone's back | **right click** while looking at them |
| Throw what you are holding | **left click** |
| Grab an item in your mouth, and let it go | **Tab** |
| Talk | hold **T** (push-to-talk; in open mic it forces transmit) |
| Open mic ↔ push-to-talk | **V** |
| Free or capture the mouse | **Esc** |
| Session readout, with the build label | **F1** |
| Quit | **⌘Q** on a Mac, **Alt+F4** elsewhere |

Things to know: whatever you are looking at within reach glows white; that is what a click takes.
A tower on someone's back can only be unloaded by *other* players, one item at a time from
anywhere in the stack — you cannot reach your own. Past seven items it starts to sway and pull the
carrier about. If you get picked up, jam **A** and **D** back and forth for a couple of seconds to
get free. Talking with something in your mouth sounds like it.

**Your things are yours.** When you quit, whatever you were carrying — in hand, in mouth, on your
back — leaves the world with you, and the next time you play on the same computer you come back
where you were, carrying it. (Same computer: the beta cannot yet follow you between machines.)

## Reporting a problem

[Open an issue](https://github.com/radical-beard/campy-beta/issues/new) with what you did, what
happened, your platform, and the **build label**: press **F1** in game and read the first line.
If the game crashed, attach the newest file from its log folder:

| | |
|---|---|
| macOS | `~/Library/Application Support/Godot/app_userdata/project-campy-camping/logs/` |
| Windows | `%APPDATA%\Godot\app_userdata\project-campy-camping\logs\` |
| Linux | `~/.local/share/godot/app_userdata/project-campy-camping/logs/` |
