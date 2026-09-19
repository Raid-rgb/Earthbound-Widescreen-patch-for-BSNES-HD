
A .bps patch that enables 16:9 widescreen rendering when played on the bsnes-hd emulator.

<p align="center">
  <img width="650" alt="widescreen patch test-003" src="https://github.com/user-attachments/assets/88d758bd-b67a-44ca-9b58-f7d90747d7ec" />
</p>

---

## Installation (patching)

Patch your ROM with the matching .bps file from [Releases](../../releases) using any BPS patcher (such as [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)).

---

## Emulator Configuration (`bsnes-hd`)

* **Settings → Enhancements:**
  * **Widescreen:** `All`
  * **Aspect Ratio:** `16:9`
  * **Sprites:** `Unsafe` *(makes sprites render past native 8:7 bounds)*

---

## Known Limitations & Issues

* **Outer Edge Clipping:** Sprites will pop out/cut off near the outer edges of the 16:9 frame due to the engine's hardcoded entity active range.
* **Cheat Compatibility:** Some cheat codes (such as RetroArch cheat database entries, Action Replay, or Game Genie codes) may conflict with altered memory addresses and cause crashes.
