# Oleksandr Tokarev - Unity Developer | C# Gameplay Programmer

Unity Developer based in Finland with nearly three years of hands-on C# gameplay programming across Android, PC, and WebGL. Available fully remote through employment or B2B.

I solo-developed and shipped an Android game on Google Play, owning architecture, implementation, profiling, debugging, build preparation, publishing, and post-release support. I build maintainable, performance-aware Unity systems with SOLID/SRP, dependency injection, Assembly Definitions, ScriptableObjects, UniTask, and clear runtime/presentation boundaries.

Email: **otokarevdev@gmail.com**

## Main Links

- Portfolio and CV: https://tokarevdev.github.io/
- Google Play release: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle
- LinkedIn: https://www.linkedin.com/in/oleksandr-tokarev/
- Gameplay prototypes: https://sd7games.itch.io/

## Professional Focus

- Gameplay programming: combat, weapons, projectiles, AI strategies, progression, save/load, rewards, enemies, and runtime stat modifiers.
- Architecture: SOLID/SRP, MVVM-style presentation, Zenject, dependency injection, composition roots, Assembly Definitions, services, events, and ScriptableObjects.
- Async and lifecycle: UniTask, async/await, CancellationToken, lifecycle-bound cancellation, explicit subscription and resource cleanup.
- Performance: Unity Profiler, GC allocation profiling, object pooling, cached references, mobile frame-time optimization, and no hot-path scene searches.
- Delivery: Android, Google Play, PC, WebGL, Git/GitHub, ClickUp, task tracking, and collaborative planning.
- Multiplayer: Netcode for GameObjects, UGS Relay, Lobby, Auth, RPCs, NetworkVariables, and lobby UI.

## Featured Projects

### Emoji Battle - Shipped Google Play Game

Public source: https://github.com/TokarevDev/Emoji_Battle

Google Play: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle

Development: Sep 2025 - Feb 2026

Solo-developed in Unity 6 and shipped to Google Play within a six-month independent development cycle.

Key results:

- Owned the full player loop, progression, save data, UGUI flow, Unity Ads, store preparation, and post-release support.
- Implemented three AI difficulty modes through Strategy Pattern, separating decision logic from board rendering and lobby UI.
- Improved performance on older Android devices from approximately 30 FPS to a stable 60 FPS.
- Validated adaptive 90 FPS and 120 FPS targets on supported devices by reducing UI draw calls and separating gameplay from presentation.

Code review map:

- Domain logic: `Assets/Scripts/Domain/`
- Persistence and services: `Assets/Scripts/Infrastructure/`
- Gameplay and UI: `Assets/Scripts/Presentation/`
- Bootstrap: `Assets/Scripts/App/`

### Last Seed Survivor - Mobile 2D Auto-Shooter

Public source: https://github.com/TokarevDev/Force_of_Nature_Last_Seed

Development: Mar 2026 - present

Unity 6 mobile survival project focused on modular combat, weapons, runtime stat modifiers, Physics2D enemies, and ScriptableObject-driven reward selection with rarity and DPS-aware tuning.

Key results:

- Pooled projectiles and enemy segments to reduce runtime object churn in high-density combat.
- Separated gameplay, presentation, runtime data, UI binding, bootstrap, and balance tooling by responsibility.
- Built a one-click deterministic test that runs 4,000 battles per cycle.
- The cycle covers four player-behavior scenarios of 1,000 battles each, including ad engagement and revive combinations.
- Repeated runs completed with zero detected combat-logic failures.

Code review map:

- Bootstrap: `Assets/_Project/App/Bootstrap/`
- Combat, weapons, projectiles, and rewards: `Assets/_Project/App/Gameplay/Combat/`
- Segmented enemy and balance tools: `Assets/_Project/App/Gameplay/Enemy/Worm/`
- Presentation: `Assets/_Project/App/Presentation/`

### 2D Asteroids Survival - Architecture Sample

Public source: https://github.com/TokarevDev/2D_Asteroids_Survival

Compact Unity 2022 LTS survival prototype built as a reviewable architecture sample.

What it demonstrates:

- Four Assembly Definition modules: Core, Infrastructure, Gameplay, and UI.
- Zenject composition roots, dependency injection, and SignalBus communication.
- UniTask-based bootstrap and scene transitions.
- Input System behind `IInputReader` and scene loading behind `ISceneLoader`.
- MVVM-style game-over flow with lifecycle-safe subscriptions.
- ScriptableObject-driven asteroid variants.
- Prewarmed projectile and asteroid pools with duplicate-return protection.
- Cached references and allocation-conscious Update/FixedUpdate paths.

## Technical Stack

Unity 2022 LTS / Unity 6, C#, MonoBehaviour lifecycle, UGUI, Input System, Physics2D, DOTween, URP, SOLID/SRP, MVVM, Zenject, dependency injection, composition roots, Assembly Definitions, services, events, ScriptableObjects, UniTask, async/await, CancellationToken, object pooling, Unity Profiler, Netcode for GameObjects, UGS Relay/Lobby/Auth, Git/GitHub.

## Background

- Independent Unity Developer, Sep 2023 - present.
- Delivered playable builds for Android, PC, and WebGL.
- Education: Xamk - South-Eastern Finland University of Applied Sciences, Introduction to Video Games Creation, Flexible Modular Open UAS Studies, 1-35 ECTS, Jul-Dec 2026.
- Languages: English B1 (improving), Russian native, Ukrainian native.
