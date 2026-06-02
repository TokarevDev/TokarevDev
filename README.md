# Oleksandr Tokarev - Unity C# Developer

Unity C# Developer based in Finland, focused on gameplay systems, mobile/WebGL prototypes, clean feature implementation, and practical production-ready Unity workflows.

I build playable Unity features from prototype to release: gameplay logic, UI flow, scene/prefab setup, data-driven configs, save/load features, ads integration, debugging, profiling, and build preparation for Android, PC, and WebGL.

- Portfolio: https://tokarevdev.github.io/
- LinkedIn: https://www.linkedin.com/in/oleksandrtokarev/
- Playable builds: https://sd7games.itch.io/
- Released game: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle
- Email: OleksandrTokarevDev@gmail.com

## What I Can Own

- Gameplay systems: combat, weapons, projectiles, enemies, rewards, progression, player flow, and complete playable loops.
- Unity implementation: MonoBehaviour lifecycle, scenes, prefabs, UI screens, popups, input, build setup, and iteration inside the Unity Editor.
- Maintainable C#: SRP-style components, event-driven communication, service abstractions, data/runtime separation, and readable feature code.
- Mobile performance: object pooling, GC allocation awareness, cached references, fewer runtime scene searches, and profiler-minded iteration.
- Delivery workflow: Android builds, WebGL prototypes, Google Play release preparation, Git, debugging, refactoring, and technical documentation.

## Featured Projects

### Last Seed: Survival

2D mobile auto-shooter built in Unity 6 with modular weapons, reward choices, pooled projectiles, segmented worm enemy logic, custom balancing tooling, and Android release preparation.

What I built:

- Projectile weapon and Acacia Thorn weapon systems.
- Runtime modifiers for damage, fire rate, critical chance, critical power, penetration, salvo shots, projectile speed, and parallel shots.
- Reward roll/apply services with rarity slots, reward categories, rerolls, and DPS-aware reward bias.
- Segmented worm enemy with combat sections, rollback behavior, HP scaling, pressure tuning, and visual presenters.
- Projectile and worm segment pooling to reduce runtime object churn.
- Unity Editor balance lab for deterministic reward/HP simulations using real project data.

Repository: https://github.com/TokarevDev/Force_of_Nature_Last_Seed

### Emoji Battle

Released Android game with turn-based combat, AI strategy selection, progression, persistent player data, popup/UI flow, rewarded/interstitial ads, and Google Play release workflow.

What I built:

- Full turn-based gameplay loop and board state logic.
- AI strategies for multiple difficulty levels.
- Progression, rewards, avatar selection, settings, and persistent game data.
- Popup service, UI screens, result flow, and animated UI feedback.
- Unity Ads service with rewarded state handling, load timeout, resume handling, and online/offline checks.
- Google Play release preparation and Android build workflow.

Google Play: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle  
Repository: https://github.com/TokarevDev/Emoji_Battle

### Tanks Multiplayer Prototype

Unity multiplayer prototype with host/client flow, anonymous authentication, UGS Relay/Lobby, networked movement, shooting, health, respawn, coins, and leaderboard-style UI.

What I built:

- Client/host connection flow with Unity Services initialization.
- Relay allocation, join-code setup, lobby creation, lobby list, and heartbeat handling.
- NetworkVariables for player data, health, names, and coins.
- ServerRpc/ClientRpc shooting flow and networked projectile spawning.
- Respawn, leaderboard, HUD, lobby UI, and menu flow.

Repository: https://github.com/TokarevDev/Tanks_Multiplayer

## Additional Playable Prototypes

- Sharp Shooter: FPS WebGL prototype with weapon configs, raycast shooting, pickups, enemy behavior, health/shield flow, UI feedback, and browser delivery.
- Royal Run: 3D endless runner WebGL prototype with player movement, pickups, obstacle spawning, score/UI/audio flow, and chunk-based level progression.
- Galaxy Strike: 3D space shooter PC prototype with shooting interactions, collision/game state handling, score UI, dialogue/audio flow, and cinematic sequence setup.

## Technical Focus

Unity 6, C#, gameplay programming, UGUI, Input System, ScriptableObjects, event-driven systems, Strategy Pattern, object pooling, Physics2D, NavMesh exposure, DOTween, Unity Ads, Netcode for GameObjects, UGS Relay/Lobby/Auth, Unity Profiler, Git, Android, PC, WebGL.

## Current Growth Focus

- PlayMode/EditMode tests for Unity gameplay systems.
- Addressables and stronger asset lifecycle management.
- Mobile profiling with real device capture and documented before/after results.
- More short gameplay videos/GIFs for project READMEs and portfolio pages.
- English communication for international Unity teams.
