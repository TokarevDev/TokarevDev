# Oleksandr Tokarev - Unity C# Developer / C# Gameplay Programmer

Unity C# Developer based in Finland with 2+ years of hands-on Unity experience. I build gameplay features, UI/UGUI flow, data-driven systems, and stable Android, PC, and WebGL builds.

Portfolio: https://tokarevdev.github.io/

I have shipped a complete Android game on Google Play and built Unity projects covering gameplay programming, UI/UGUI, ScriptableObject configs, save/load, ads integration, object pooling, debugging, profiling, and build preparation.

My strongest area is connecting clean C# architecture with practical Unity implementation: systems that are easier to extend, balance, debug, and ship without unnecessary overengineering.

## Main Links

- Portfolio / CV / project hub: https://tokarevdev.github.io/
- Google Play release: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle
- Emoji Battle source: https://github.com/TokarevDev/Emoji_Battle
- Last Seed Survivor source: https://github.com/TokarevDev/Force_of_Nature_Last_Seed
- WebGL prototypes: https://sd7games.itch.io/

## What I Can Own

- Gameplay systems: combat, weapons, projectiles, enemies, rewards, progression, player flow, and complete playable loops.
- UI flow: UGUI screens, menus, popups, gameplay HUD, result flow, player feedback, and state-driven UI updates.
- Maintainable C#: SRP-style components, event-driven communication where it reduces coupling, service abstractions, and clear data/runtime separation.
- Mobile performance: object pooling, GC allocation awareness, cached references, profiler-minded iteration, and fewer runtime scene searches.
- Delivery workflow: Android builds, WebGL/PC build preparation, Unity debugging, refactoring, scene/prefab setup, and technical documentation.

## Main Projects

### Emoji Battle

Released Android game built in Unity 6 and C#, taken from prototype to public Google Play release.

What it demonstrates:

- Turn-based gameplay loop and board state logic.
- AI strategies for multiple difficulty levels.
- Progression, rewards, avatar selection, settings, and persistent player data.
- Popup service, UI screens, result flow, and animated feedback.
- Unity Ads integration with rewarded/interstitial flow, load timeout, resume handling, and online/offline checks.

Impact:

- Challenge: turn a small prototype into a complete Android game that could pass store review.
- Work: owned combat flow, AI, persistence, UI states, ads, Android build preparation, and publishing steps.
- Outcome: public Google Play release with reviewable source code and gameplay media.

Code review map:

- Main project code: `Assets/Scripts/`
- Domain logic: `Assets/Scripts/Domain/`
- Persistence and data services: `Assets/Scripts/Infrastructure/`
- Gameplay, lobby, UI, and popups: `Assets/Scripts/Presentation/`
- Bootstrap and runtime setup: `Assets/Scripts/App/`

Unity vendor packages and imported assets are present in the repository, but the portfolio-relevant code lives under `Assets/Scripts/`.

### Last Seed Survivor

Current Unity 6 mobile auto-shooter project focused on modular gameplay systems, reward choices, pooled projectiles, segmented enemy logic, balance tooling, and Android release preparation.

What it demonstrates:

- Modular weapon systems with runtime stat modifiers.
- ScriptableObject-driven rewards, rarities, HP scaling, and pressure tuning.
- Projectile and enemy segment pooling to reduce runtime object churn.
- Reward roll/apply services separated from UI binding and gameplay effects.
- Custom Unity Editor balance lab for deterministic reward/HP simulations.

Impact:

- Challenge: mobile survival gameplay needed scalable combat, rewards, and tuning instead of one-off prototype logic.
- Work: separated data, runtime systems, UI binding, bootstrap, pooling, and balance simulation tools.
- Outcome: closed test passed; systems are easier to tune, profile, and review in code.

Code review map:

- Main project code: `Assets/_Project/App/`
- Bootstrap and scene startup: `Assets/_Project/App/Bootstrap/`
- Gameplay combat, weapons, projectiles, and rewards: `Assets/_Project/App/Gameplay/Combat/`
- Segmented enemy systems and balance tooling: `Assets/_Project/App/Gameplay/Enemy/Worm/`
- Presentation/UI-related gameplay flow: `Assets/_Project/App/Presentation/`

Unity vendor packages and imported assets are present in the repository, but the portfolio-relevant code lives under `Assets/_Project/App/`.

## Core Stack

Unity 6, C#, gameplay programming, UI/UGUI, ScriptableObjects, event-driven systems, Strategy Pattern, object pooling, Physics2D, DOTween, Unity Ads, Unity Profiler, Git, Android, PC, WebGL.
