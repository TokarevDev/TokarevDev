# Oleksandr Tokarev - Unity Developer | C# Gameplay Programmer

Unity Developer based in Finland with 3+ years of independent C# gameplay development experience across Android, PC, and WebGL. Available for fully remote employment or B2B opportunities.

The projects presented on this GitHub profile are independent personal projects that I designed and developed. They demonstrate my approach to gameplay architecture, performance, lifecycle management, debugging, build delivery, and post-release support.

I build maintainable, performance-aware Unity systems with clear responsibility boundaries, explicit dependencies, predictable object lifecycles, and production-focused workflows.

Email: **otokarevdev@gmail.com**

## Main Links

- Portfolio and CV: https://tokarevdev.github.io/
- LinkedIn: https://www.linkedin.com/in/oleksandr-tokarev/
- Google Play release: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle
- Gameplay prototypes: https://sd7games.itch.io/

## Featured Projects

### 2D Asteroids Survival - Complete PC and Android Game

- Case study and playable builds: https://tokarevdev.github.io/projects/asteroids.html
- Public source: https://github.com/TokarevDev/2D_Asteroids_Survival
- Gameplay video: https://youtu.be/MV7N_iHXxiU

A feature-complete Unity 2022 LTS survival game independently designed and developed from scratch, inspired by the classic Asteroids formula.

Key engineering work:

- Built custom fixed-step 2D physics, collision tests, toroidal world coordinates, asteroid fragmentation, projectiles, a rechargeable multi-target laser, UFO pursuit, scoring, and a three-life survival loop.
- Separated Core, Infrastructure, Gameplay, and UI through four Assembly Definitions with explicit dependency direction.
- Used Zenject composition roots, dependency injection, interfaces, factories, SignalBus, and MVVM-style UI to keep responsibilities clear.
- Implemented separate desktop and mobile input strategies behind shared contracts.
- Pooled asteroids, fragments, UFOs, projectiles, logical entities, and collision VFX to control runtime object churn.
- Delivered playable Windows and Android builds with public source and a gameplay demonstration.

### Emoji Battle - Shipped Google Play Game

- Case study: https://tokarevdev.github.io/projects/emoji-battle.html
- Public source: https://github.com/TokarevDev/Emoji_Battle
- Google Play: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle

Solo-developed in Unity 6 and shipped to Google Play within a three-month independent development cycle.

Key results:

- Owned the complete player loop, progression, persistence, UGUI flow, advertising, store preparation, publishing, and post-release support.
- Implemented three AI difficulty modes through the Strategy Pattern, separating decision logic from board rendering and lobby UI.
- Improved performance on older Android devices from approximately 30 FPS to a stable 60 FPS.
- Validated adaptive 90 FPS and 120 FPS targets on supported devices by reducing UI draw calls and separating gameplay from presentation.

### Last Seed Survivor - Modular Mobile Survival Systems

- Case study: https://tokarevdev.github.io/projects/last-seed.html
- Public source: https://github.com/TokarevDev/Force_of_Nature_Last_Seed

Unity 6 mobile auto-shooter focused on modular combat, weapons, runtime stat modifiers, Physics2D enemies, ScriptableObject-driven rewards, pooling, and deterministic balance tooling.

Key results:

- Separated gameplay, presentation, runtime data, UI binding, bootstrap, and balance tooling by responsibility.
- Pooled projectiles and enemy segments to reduce runtime object churn in high-density combat.
- Built a one-click deterministic test that runs 4,000 battles per cycle across four player-behavior scenarios.
- Repeated test cycles completed with zero detected combat-logic failures.

## Professional Focus

- Gameplay programming: combat, weapons, projectiles, enemies, AI strategies, progression, rewards, save/load, and runtime stat systems.
- Architecture: SOLID/SRP, dependency injection, composition roots, Assembly Definitions, MVVM-style presentation, services, events, and ScriptableObjects.
- Async and lifecycle: UniTask, async/await, CancellationToken, lifecycle-bound cancellation, symmetric subscriptions, and explicit resource cleanup.
- Performance: Unity Profiler, GC allocation profiling, object pooling, cached references, mobile frame-time optimization, and allocation-conscious hot paths.
- Delivery: Android, Google Play, PC, WebGL, build preparation, publishing, Git/GitHub, task tracking, and collaborative planning.
- Multiplayer: Netcode for GameObjects, UGS Relay/Lobby/Auth, RPCs, NetworkVariables, and lobby UI.

## Technical Stack

Unity 2022 LTS / Unity 6, C#, MonoBehaviour lifecycle, UGUI, Input System, Physics2D, DOTween, URP, SOLID/SRP, MVVM, Zenject, dependency injection, composition roots, Assembly Definitions, services, events, ScriptableObjects, UniTask, async/await, CancellationToken, object pooling, Unity Profiler, Netcode for GameObjects, UGS Relay/Lobby/Auth, Git/GitHub.

## Background

- 3+ years of independent Unity development experience.
- Public GitHub projects are independent personal work with reviewable source code and delivery evidence.
- Delivered playable builds across Android, PC, and WebGL.
- Education: Xamk - South-Eastern Finland University of Applied Sciences, Introduction to Video Games Creation, Flexible Modular Open UAS Studies, 1-35 ECTS, Jul-Dec 2026.
- Languages: English B1 (improving), Russian native, Ukrainian native.
