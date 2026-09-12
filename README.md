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

1. Unzip. You get `project-campy-camping.app` and two launchers beside it.
2. The app is not notarized, so macOS will call it damaged or from an unidentified developer.
   Open Terminal, `cd` into the unzipped folder, and run this once:
   ```
   xattr -cr .
   ```
3. Double-click **join-campy.command** (or **host-campy.command** if you are the host). macOS
   asks for microphone access the first time you talk; say yes.

### Windows

1. Unzip anywhere.
2. Double-click **join-campy.bat** (or **host-campy.bat**). If Windows says it protected your
   PC: *More info* → *Run anyway*. The build is unsigned, that is all.

### Linux

1. Unzip. If the game will not start, `chmod +x campy.x86_64`.
2. Run **join-campy.sh** (or **host-campy.sh**).

### Hosting and joining

One player hosts, everyone else joins. Joining looks for a session called "campy" anywhere in
the world, so agree on who hosts and have only one host up at a time. There is no menu for this
yet; the launchers pass the right flags. Two groups at once? Run the game from a terminal with
`--host <name>` and `--join <name>`.

## Controls

| | |
|---|---|
| Move | **W A S D** |
| Sprint | **Shift** |
| Jump | **Space** |
| Look | mouse |
| Talk | hold **T** (push-to-talk; in open mic it forces transmit) |
| Open mic ↔ push-to-talk | **V** |
| Free or capture the mouse | **Esc** |
| Session readout, with the build label | **F1** |
| Quit | **⌘Q** on a Mac, **Alt+F4** elsewhere |

## Reporting a problem

[Open an issue](https://github.com/radical-beard/campy-beta/issues/new) with what you did, what
happened, your platform, and the **build label**: press **F1** in game and read the first line.
If the game crashed, attach the newest file from its log folder:

| | |
|---|---|
| macOS | `~/Library/Application Support/Godot/app_userdata/project-campy-camping/logs/` |
| Windows | `%APPDATA%\Godot\app_userdata\project-campy-camping\logs\` |
| Linux | `~/.local/share/godot/app_userdata/project-campy-camping/logs/` |
