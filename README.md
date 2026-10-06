# AiT Portals Compat

Forge 1.20.1 (47.4.10) addon that re-enables Immersive Portals compatibility for Adventures in Time.

## Build
- Push to GitHub: the **Actions** tab builds the jar (artifact: `ait-portals-compat`).
- Locally (JDK 17): `gradle wrapper --gradle-version 8.1.1` once, then `./gradlew build`.
  Jar ends up in `build/libs/`.

## Setup checklist
1. Rename package `com.example.aitportalscompat` and `mod_group_id` in `gradle.properties`.
2. Set Adventures in Time's real mod id in `mods.toml` and `AitPortalsCompat.java`.
3. Add both mods as `compileOnly fg.deobf(...)` deps in `build.gradle` to code against them.
