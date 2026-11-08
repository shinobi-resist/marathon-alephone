# Player guide: Marathon 2 and Infinity on your Mac

For our native Apple Silicon builds of Classic Marathon 2 and Classic Marathon Infinity (Aleph One 1.11). Everything here is the engine's default; change any of it in **Preferences > Controls** from the main menu.

## Installing

1. Download the DMG for your game from https://github.com/shinobi-resist/marathon-alephone/releases (and `SHA256SUMS` if you want to check it: `shasum -a 256 -c SHA256SUMS`).
2. Open the DMG and drag **Classic Marathon 2** or **Classic Marathon Infinity** onto **Applications**. They install side by side and keep separate preferences and saves. macOS 12 or later, Apple Silicon.
3. Open the app from Applications or Launchpad.

### Gatekeeper
Release builds are signed with a Developer ID certificate and notarised by Apple, so macOS opens them with no warning. If macOS says it "cannot verify" the app is free of malware, you have a test build that was not notarised: click **Done**, open **System Settings > Privacy & Security**, scroll to the message about the app and click **Open Anyway**, then confirm. You only do this once per app.

### Where your saves live
- Saved games: `~/Library/Application Support/Marathon 2/Saved Games` (Infinity: `~/Library/Application Support/Marathon Infinity/Saved Games`). Quick saves, recordings and screenshots sit next to it in the same folder.
- Preferences: `~/Library/Preferences/Marathon 2/` (or `Marathon Infinity`).
- In Finder, **Go > Go to Folder** and paste the path. Deleting or updating the app leaves saves and preferences in place.

## Controls

| Action | Key | Mouse |
|---|---|---|
| Move forward / back | **W** / **S** | |
| Sidestep left / right | **A** / **D** | |
| Turn left / right | **← / →** | move the mouse |
| Look up / down | **↑ / ↓** | move the mouse |
| Glance left / right | **Q** / **E** | |
| Recentre view | **V** | |
| Fire | **Space** | left button |
| Second trigger (second weapon, or alt fire) | **Left Shift** | right button |
| Previous / next weapon | **F** / **R** | scroll wheel |
| **Run / swim** | **Left Control** (hold) | |
| Turn → sidestep (hold) | **Left Option** | |
| Move → look (hold) | **Left Command** | |
| **Action**: open doors, flip switches, read terminals | **Tab** | |
| Auto map | **M** | |
| Aux trigger (throw grenade with the assault rifle, etc.) | **`** | |
| Pause / menu | **Esc** | |

Double-tapping the Run key also activates doors and switches, so you can leave Tab alone once you have the habit.

### Mouse look feels too fast or too slow
The game reads the mouse itself, so your macOS tracking speed is not the whole story. Open **Preferences > Controls > Mouse** in the game:

- **Horizontal Sensitivity** and **Vertical Sensitivity** sliders. They are logarithmic, so small moves near the middle make a big difference; start by dragging both a quarter of the way down.
- **Mouse Feel**: *Classic* reproduces the 1995 acceleration curve; *Modern* is linear with no acceleration, which is what most players expect from a current FPS. If turning feels twitchy at the start of a movement and sluggish at the end, choose Modern.
- **Invert Vertical Aim** if looking up and down feels backwards.

### Moving feels slow
You are walking. **Hold Left Control to run**, or set **Preferences > Controls > Run/Swim Behavior** to **Always Run**, which makes running the default and the key a walk key. Marathon's walking pace is deliberately slow; nearly everyone plays with Always Run.

## Multiplayer in brief
Gather a LAN game from **Join Network Game / Gather Network Game**; internet games go through the lhowon.org lobby and need UDP port 4226 open on the gatherer's router.

## Saving
Marathon saves at pattern buffers in the levels. Aleph One also offers quick saves (**Preferences > Misc**), which many players switch on.
