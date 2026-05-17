

# 🤖 AzzyAI-RE
> A highly optimized, modernized fork of the legendary Dr. Azzy's Mercenary/Homunculus AI, explicitly refactored and patched to ensure compatibility with modern Ragnarok Online renewal and Zero clients (`ragexe`).

![Lua](https://img.shields.io/badge/Language-Lua-blue?style=for-the-badge&logo=lua)
![Ragnarok](https://img.shields.io/badge/Client-Ragexe__RE__%2F__Zero-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Stability-Production__Ready-green?style=for-the-badge)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/AoShinRO/AzzyAI-RE)

The original `AzzyAI` codebase is actually outdated. This repository bridges that gap, implementing direct fixes for state-machine loops, tick calculations, and multi-return positioning issues common in modern client versions.

---

## 🔬 Verified Client Compatibility Matrix

This fork has been strictly audited, reverse-engineered for compatibility, and field-tested across the following `ragexe` / `ragexeZero` compilation dates:

| Client Timestamp / Name | Build Flavor | Notes |
| :--- | :--- | :---: |
| `2017-05-17aRagexeRE` | Renewal | Legacy RE stable support. |
| `2018-06-21aRagexeRE` | Renewal | Standard packet structure verified. |
| `2020-01-15_2aRagexe_zero` | RO Zero | Handles initial Zero custom mechanics. |
| `2022-04-06_Ragexe_1648707856` | Renewal | Fully compatible with 160+ packets. |
| `2022-10-24_Ragexe_1666317162_zero`| RO Zero | Core AI state machine responsive. |
| `2022-11-16_Ragexe_1668558245_zero`| RO Zero | Zero skill cooldown intervals patched. |
| `2023-09-06_Ragexe` | Renewal | Native positioning hooks stable. |
| `2024-08-07_RagexeZeroRE` | Zero-RE Hybrid| Handles hybrid packet routing schemas. |
| `2025-06-03_Ragexe` | Modern Renewal| Verified on the latest client boundaries. |

---

### ⚡ Homunculus S & Mercenary Skill Delay Patch
* Full mapped database matrices inside `H_SkillList.lua` for Homunculus S (including Bayeri, Dieter, Eira, Eleanor, and Sera) and high-tier Mercenaries.
* Pre-configured cooldown maps (`AutoSkillCooldown`) preventing the AI from trying to spam skills that are currently locked behind client/server-side global cooldowns (GCD), effectively eliminating packet spam kicking.

---

## 🚀 Installation & Deployment

1. Download the repository source code from the **[GitHub Releases](https://github.com/AoShinRO/AzzyAI-RE/releases)** or clone the main branch.
2. Locate your Ragnarok Online game directory.
3. Open or create the `AI` folder, and look for the `USER_AI` directory:
```bash
   # Standard path structure
   C:\Gravity\Ragnarok Online\AI\USER_AI\
   C:\Gravity\Ragnarok Online\AI_sakray\USER_AI\
```

4. Copy&Paste the contents of this repository inside it replacing all files. (if your client have `AI_sakray` folder, need to copy&replace on both folders)
5. In Setup.exe, enable `/hoai` and ingame type `/hoai` to switch from official AI to Custom AI.
6. Vaporize and re-summon your Homunculus (or call a new Mercenary) to initialize the modernized Lua state machine.

---

## ⚖️ Legal Disclaimer

This repository provides custom user-end scripting files intended for personal automation setups, educational purposes, and sandbox testing environments within Ragnarok Online emulators (rAthena/Hercules). It does not perform executable patching, memory manipulation, or unauthorized DLL injection. This project is entirely unofficial and not affiliated with Gravity Co., Ltd. or any official regional Ragnarok Online publishing branch.
