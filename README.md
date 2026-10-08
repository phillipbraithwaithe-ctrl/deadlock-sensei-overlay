# Deadlock Sensei Overlay

A small see-through panel that sits on top of Deadlock and shows the next item or skill to buy from [Deadlock Sensei](https://deadlocksensei.com), the two after it, your item slots, the game clock and the enemy team. Hotkeys handle "I bought it" and marking the enemy who's wrecking you.

**[⬇ Download the latest version](https://github.com/phillipbraithwaithe-ctrl/deadlock-sensei-overlay/releases/latest)**

## Setup
1. In Deadlock, set **Settings → Video → Window mode** to **Borderless Windowed**. In exclusive fullscreen, nothing can draw over the game.
2. Unzip, then run **Deadlock Sensei Overlay.exe**. It's a portable app with no install.
   The app isn't code-signed yet, so Windows shows *"Windows protected your PC"* the first time. Click **More info → Run anyway**.
3. It opens in the top-left and runs from the system tray. Right-click the tray icon to show or hide it, move it to a corner, turn click-through on or off, or quit.

Before a match, press **Ctrl+Alt+C** so you can click the panel, pick your hero and the enemy team, then press **Live game**. Press **Ctrl+Alt+C** again so your clicks go through to the game.

## Hotkeys
| Keys | Does |
|---|---|
| Ctrl+Alt+B | I bought it (ticks the next item) |
| Ctrl+Alt+Z | Undo |
| Ctrl+Alt+1 … 6 | F\*\*K THIS GUY on enemy 1–6 (the build adapts) |
| Ctrl+Alt+W | Walker down (+1 slot) |
| Ctrl+Alt+T | Start the game clock |
| Ctrl+Alt+← / → | Clock −10 s / +10 s |
| Ctrl+Alt+O | Show/hide the overlay |
| Ctrl+Alt+C | Click-through on/off |

Rebind them in `%APPDATA%\Deadlock Sensei Overlay\settings.json`.

## Safe by design
The overlay **never touches the game**: no injection, no reading game memory or files, no simulated input, no screen capture. It's an ordinary always-on-top window plus Windows hotkeys, like Discord or OBS. Everything it shows comes from deadlocksensei.com, so it updates without a new download.
