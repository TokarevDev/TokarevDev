# Oleksandr Tokarev — Unity Developer | C# Gameplay Programmer

I design and implement production-oriented gameplay systems in C#. My work keeps domain rules testable outside Unity, dependencies and frame order explicit, and runtime ownership safe across initialization, cancellation, rollback, cleanup, and scene transitions.

The two public projects below connect architectural decisions to playable behavior, source code, validation, and practical performance constraints.

## Selected Work

### Last Seed Survivor

[Case study](https://tokarevdev.github.io/projects/last-seed.html) · [Source code](https://github.com/TokarevDev/Last_Seed_Survivor) · [Gameplay](https://youtube.com/shorts/HiQBlYjienI?feature=share)

An architecture-first Unity 6 mobile auto-shooter built around explicit ownership, deterministic gameplay rules, and project-wide validation.

- Seven production/tooling assemblies separate engine-free contracts and domain state from gameplay, infrastructure, presentation, bootstrap, and Editor code.
- Domain-focused Zenject installers describe composition without runtime service location; a single frame coordinator captures one immutable input snapshot and runs named gameplay stages.
- Segmented-worm construction and pooled-object registration use staged reverse rollback; cleanup preserves ownership even when later operations fail.
- Reward generation, policy, commit, application, presentation, and guarded rewarded-ad operations have separate contracts and failure behavior.
- `ObjectPool<T>` protects identity ownership while specialized projectile, worm-segment, and damage-popup adapters handle Unity-specific lifecycle.
- Worm Balance Lab reuses production reward, weapon-power, HP, progression, reroll, ad, and revive rules for deterministic balance simulation.
- Current baseline: project build, 299 EditMode tests, 29 PlayMode tests, configuration and serialized-reference validation, plus Zenject validation for all three enabled scenes.
- Runtime work includes pooled high-churn entities, dictionary-backed ownership lookup, allocation-aware hot paths, explicit profiler markers, and conservative 60/90/120 FPS selection. Android hardware profiling remains a separate release gate.

### 2D Asteroids Survival

[Case study](https://tokarevdev.github.io/projects/asteroids.html) · [Source code](https://github.com/TokarevDev/2D_Asteroids_Survival) · [Gameplay](https://youtu.be/MV7N_iHXxiU)

A feature-complete Unity 2022 LTS survival game built around custom simulation, explicit dependency direction, and predictable runtime ownership.

- `GameplayFixedLoop` is the single fixed-step entry point, running named movement, integration, projectile, world-boundary, collision, and presentation stages over custom 2D physics and toroidal coordinates.
- Core, Infrastructure, Gameplay, and UI are separated through Assembly Definitions; domain installers compose them with Zenject without runtime service lookup or magic execution-order values.
- Validated JSON maps hold player, enemy, and world parameters and reject missing, unknown, null, duplicate, or incorrectly cased enemy keys before gameplay starts.
- Generic `ObjectPool<T>` storage and `EnemyPool<TEnemy, TInitialization>` centralize FIFO reuse, duplicate-return protection, initialization, registration, activation, teardown, and rollback for enemies, projectiles, and collision VFX.
- Desktop and mobile strategies use Unity's classic `Input` API behind one contract; `PlayerInputStateProvider` samples the selected strategy once per rendered frame for every gameplay consumer.
- MVVM-style game-over UI, SignalBus events, guarded UniTask navigation, Firebase Analytics, and optional AdMob adapters keep presentation and platform concerns outside gameplay rules.
- Playable Windows and Android builds are available; final Android device and release-build validation remains an explicit delivery gate.

## Engineering Focus

- **Gameplay architecture:** engine-free rules and state, validated JSON and ScriptableObject-authored data, narrow subsystem contracts, domain snapshots, and Unity-facing adapters.
- **Composition and execution:** Zenject, SignalBus, constructor injection, domain installers, Assembly Definitions, and named frame stages instead of hidden service lookup or magic execution-order values.
- **Lifecycle and failure safety:** validation before mutation, reverse-order rollback, best-effort cleanup, cancellation-aware async flows, symmetric subscriptions, and explicit scene ownership.
- **Performance:** object pooling, cached and dictionary-backed lookups, allocation-aware hot paths, single-frame input sampling, profiler markers, and mobile frame-time constraints.
- **Verification and tooling:** NUnit, Unity Test Framework, EditMode/PlayMode coverage, scene dependency and serialized-reference validation, deterministic Editor simulation, Git, and GitHub.

## Core Stack

Unity 2022 LTS / Unity 6 · C# · custom 2D simulation / Physics2D · classic Unity Input / Input System · UGUI · Zenject · SignalBus · UniTask · JSON / ScriptableObjects · Assembly Definitions · NUnit · Unity Test Framework · Unity Profiler · Git

## Contact

Based in Finland and open to remote B2B or contractor roles as a Unity Developer and C# Gameplay Programmer.

- Portfolio: https://tokarevdev.github.io/
- LinkedIn: https://www.linkedin.com/in/oleksandr-tokarev/
- Email: **otokarevdev@gmail.com**
