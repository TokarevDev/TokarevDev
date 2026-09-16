# Alexander Tokarev — Unity Developer | 6+ years

Unity Developer with 6+ years of experience designing and implementing gameplay and mobile game systems in C#. I keep domain rules testable outside Unity, dependencies and frame order explicit, and runtime ownership safe across initialization, cancellation, rollback, cleanup, and scene transitions.

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

- **Gameplay and progression:** combat, weapons, rewards, inventory, equipment, crafting, tutorials, save systems, stable IDs, schema migration, and idempotent state changes.
- **Architecture and execution:** engine-free rules, narrow contracts, Zenject, SignalBus, constructor injection, Assembly Definitions, validated JSON and ScriptableObjects, and named frame stages.
- **Async and lifecycle safety:** Addressables ownership, `async`/`await`, UniTask, `CancellationToken`, validation before mutation, reverse-order rollback, symmetric subscriptions, and deterministic cleanup.
- **Performance and memory:** Unity Profiler, Memory Profiler, object pooling, non-alloc APIs, cached and dictionary-backed lookups, allocation-aware hot paths, and mobile frame-time constraints.
- **Verification and delivery:** NUnit, Unity Test Framework, EditMode/PlayMode coverage, Editor tooling, content validation, Git, CI/CD, Android, iOS, and code review.

## Core Stack

Unity 2022 LTS / Unity 6 · C# · UGUI · ScriptableObjects · Addressables · Zenject · SignalBus · UniTask · UniRx · DOTween · Spine · Unity IAP · Firebase Analytics / Remote Config · JSON · NUnit · Unity Test Framework · Unity Profiler / Memory Profiler · Git / CI/CD

## Education & Languages

- **Xamk — South-Eastern Finland University of Applied Sciences:** Open UAS Studies, Game Development (2026)
- **Donetsk National Technical University:** Software Engineering (2014)
- **Languages:** Ukrainian — native · Russian — native · English — B1

## Contact

Based in Finland and open to remote B2B or contractor roles as a Unity Developer.

- Portfolio: https://tokarevdev.github.io/
- LinkedIn: https://www.linkedin.com/in/oleksandr-tokarev/
- Email: **otokarev@gmail.com**
