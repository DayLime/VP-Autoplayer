# VP Autoplayer 🎹 (Roblox)

**This tool has been specifically developed for use on Roblox.**

**VP Autoplayer** is a desktop tool that plays song sheets automatically in sync with [virtualpiano.net](https://virtualpiano.net/), simulating human performance. It's ideal for casual music lovers, performers, or anyone looking to bring Virtual Piano sheets to life with realism and rhythm.

**Get the latest version:** https://github.com/DayLime/VP-Autoplayer/releases/tag/v1.0.0

---

## ⚠ Warning

I am aware of the fact that this project is being flagged as a trojan by various Anti-Virus services. This is due to the way it uses the Windows API to execute the key presses required to play tracks. This is the official version of the project and has no malicious files attached to it. I welcome anyone who can and wants to fix this false flag to create a pull request with the updated code, but I am not actively maintaining this resource and thus will not look into solving it. 

To all the people that tried to use it or are using it I really appreicate the fact that you enjoyed this little coding project of mine :)

## ✨ Features

- 🎵 Autoplays `.txt` song sheets from your PC
- ⚙️ Real-time playback adjustment (tempo, subdivision, humanize, hold)
- 🧠 Humaniser: Adds realistic timing jitter, drops, slips, and drift
- 🎯 Target window detection (auto-pauses when not focused)
- 🔁 Per-sheet `#META` headers for tempo & notes
- 🌙 Light / Dark theme toggle
- ⏱️ Global hotkey to start/stop playback (`F4` by default)
- 📁 Automatically saves your settings

---

## 🚀 How to Use

1. **Run the App**  
   Download and open `VPAutoplayer.exe`.

2. **Select a Folder with Song Sheets**  
   Use the **Browse** button to set your sheet folder. Files must be `.txt`.

3. **Choose a Sheet**  
   Select a song from the dropdown list.

4. **Set the Target Window**  
   Choose the window where notes should be sent (e.g. Roblox).

5. **Start Playback**  
   Press ▶ or hit `F4` to toggle play/pause.

---

## 🎼 Get Song Sheets from Virtual Piano

You can find thousands of high-quality sheets at:

👉 https://virtualpiano.net

Look under the **Music Sheets** tab and copy the content into a `.txt` file.

---

## 🧠 Sheet Format & Metadata

Humanizer is designed to work like this:
- 0% ⇒ Disabled. It will play the song with 100% accuracy.
- 0–49 %  ⇒ Near-Perfect timing, but is obviously Autoplay.
- 50–74 % ⇒ Realistic but still skilled player.
- 75–100 % ⇒ Moves slower and is very sloppy. Mimmicks the average humans physical limitations.

---

## 💡 Tip for Matching Timing

If a song plays too fast or slow, **adjust the Subdivision** until the total duration **matches** the playback on the Virtual Piano site. Try round values like `2`, `4`, or `8`. If that doesnt work you can use float values(ex. `2.32`, `1.45`) to get the exact time and it should work fine.

> Example: If the sheet plays too fast, increase the subdivision.

---

## 🔧 Config

All global settings are saved in `vp_autoplayer.json` in the same folder as the EXE.
Sheet specific configs are saved within the Sheet metadata.

---

## 📁 Sheet Format & Metadata

Example sheet with metadata:
```
#META {"bpm": 100, "subdiv": 4, "note": "Transposed -1"}
[A F G] r r u o | s d f | o f f f d x
```
---

## 🖥 Requirements

- Windows 10 or later
- No Python or installation needed

> ⚠️ **Note:** VP Autoplayer is currently only available for **Windows**.
---

## 🤝 Contributing

Want to help improve VP Autoplayer?  
Check out [CONTRIBUTING.md](./CONTRIBUTING.md) and open a pull request!

Make sure to [add a star ⭐](https://github.com/DayLime/VP-Autoplayer/) if you like the project!

---

© 2025 VP Autoplayer — Not affiliated with VirtualPiano.net
