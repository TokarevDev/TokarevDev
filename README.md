# Oleksandr Tokarev — Unity Developer | C# Gameplay Programmer

I design and implement gameplay systems in C# with clear dependency boundaries, explicit lifecycle ownership, and performance-aware Unity integration. My work focuses on maintainable production code: gameplay architecture, combat systems, runtime state, pooling, async flows, Editor tooling, and platform delivery.

The two public projects below show the source code, architecture, and engineering decisions behind playable Unity projects.

## Selected Work

### 2D Asteroids Survival

[Case study](https://tokarevdev.github.io/projects/asteroids.html) · [Source code](https://github.com/TokarevDev/2D_Asteroids_Survival) · [Gameplay](https://youtu.be/MV7N_iHXxiU)

A complete Unity 2022 LTS survival game built around explicit dependency direction and predictable gameplay lifecycle.

- Custom fixed-step 2D physics, collision tests, toroidal coordinates, asteroid fragmentation, projectiles, multi-target laser, UFO pursuit, scoring, and session flow.
- Core, Infrastructure, Gameplay, and UI separated through Assembly Definitions.
- Zenject composition roots and dependency injection without runtime service lookup.
- MVVM-style game-over presentation, SignalBus integration, and lifecycle-bound UniTask scene transitions.
- Pooled gameplay entities and separate desktop/mobile input strategies behind shared contracts.

### Last Seed Survivor

[Case study](https://tokarevdev.github.io/projects/last-seed.html) · [Source code](https://github.com/TokarevDev/Force_of_Nature_Last_Seed) · [Gameplay](https://youtube.com/shorts/HiQBlYjienI?feature=share)

A Unity 6 mobile auto-shooter demonstrating modular combat, data-driven progression, pooled runtime systems, and repeatable balance validation.

- ScriptableObject-authored rewards update isolated runtime weapon state while roll, apply, and presentation responsibilities remain separate.
- Segmented enemy logic is divided into pattern building, creation, movement, section health, combat, balance, and presentation.
- Projectiles and enemy segments use pooling to control runtime object churn in dense combat.
- A deterministic Unity Editor tool evaluates the same reward data, weapon configuration, HP rules, and DPS model used by gameplay.

## Engineering Focus

- **Gameplay:** combat, weapons, projectiles, enemies, rewards, progression, input, and session state.
- **Architecture:** SOLID/SRP, dependency injection, composition roots, Assembly Definitions, MVVM-style UI, events, and ScriptableObjects.
- **Lifecycle:** explicit ownership, symmetric event subscriptions, cancellation-aware async flows, and predictable cleanup.
- **Performance:** Unity Profiler, object pooling, cached references, allocation-aware hot paths, and mobile frame-time constraints.
- **Tooling and delivery:** Unity Editor tools, deterministic validation, Android, Windows, WebGL, Git, and GitHub.

## Core Stack

Unity 2022 LTS / Unity 6 · C# · Physics2D · Input System · UGUI · Zenject · UniTask · ScriptableObjects · Assembly Definitions · Unity Profiler · Git

## Contact

Based in Finland and open to remote Unity gameplay and systems work.

- Portfolio: https://tokarevdev.github.io/
- LinkedIn: https://www.linkedin.com/in/oleksandr-tokarev/
- Email: **otokarevdev@gmail.com**
