> [!WARNING]
> **Not Recommended:** This patch is an early proof-of-concept for bsnes-hd and suffers from edge sprite-popping and visual glitches. For a glitch-free widescreen playthrough, consider one of the dedicated projects below instead.

### Recommended Projects

**EarthBound Companion** [rages4calm/earthbound-companion](https://github.com/rages4calm/earthbound-companion)
> Native PC port. Features proper glitch-free widescreen and ultrawide rendering without sprite popping, MSU-1 audio support. Supports both Vanilla EarthBound and MaternalBound Redux.

**EarthBound Reverb** [AlexanderVerde on itch.io](https://alexanderverde.itch.io/earthbound-reverb)
> Custom Snes9x-based build featuring proper glitch-free widescreen, along with QOL enhancements and gameplay adjustments. Supports only Vanilla Earthbound

### Other Alternatives

**Phase-Distorter** [TheRunaway5/Phase-Distorter](https://github.com/TheRunaway5/Phase-Distorter)
> Native PC port. Supports 16:9 and ultrawide, but as of now has rougher widescreen integration and occasional micro-stuttering.

**EarthboundNativePublic** [seanstaggsQU/EarthboundNativePublic](https://github.com/seanstaggsQU/EarthboundNativePublic)
> Precompiled standalone binary distribution of Brian Pugh's native C reimplementation.
---


A .bps patch that enables 16:9 widescreen rendering when played on the bsnes-hd emulator.

<p align="center">
  <img width="650" alt="widescreen patch test-003" src="https://github.com/user-attachments/assets/88d758bd-b67a-44ca-9b58-f7d90747d7ec" />
</p>

---

## Installation (patching)

* Patch your ROM with the matching .bps file from [Releases](../../releases) using any BPS patcher (such as [Rom Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)).

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

## Credits
* **[giovannygb](https://github.com/giovannygb)** - For his [original EarthBound patch](https://www.reddit.com/r/earthbound/comments/1rd2f2k/widescreen_patch_for_earthbound/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1) which was used in this patch to implement proper widescreen backgrounds .
