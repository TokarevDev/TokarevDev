# Oleksandr Tokarev - Unity C# Developer / C# Gameplay Programmer

Unity C# Developer based in Finland with 2+ years of hands-on Unity experience. I build gameplay features, UI/UGUI flow, data-driven systems, and stable Android, PC, and WebGL builds.

I have shipped a complete Android game on Google Play and built Unity projects covering gameplay programming, UI/UGUI, ScriptableObject configs, save/load, ads integration, object pooling, debugging, profiling, build preparation, and reviewable source code.

My strongest area is connecting clean C# architecture with practical Unity implementation: systems that are easier to extend, balance, debug, and ship without unnecessary overengineering.

## Main Links

- Portfolio / CV / project hub: https://tokarevdev.github.io/
- Google Play release: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle
- Emoji Battle source: https://github.com/TokarevDev/Emoji_Battle
- Last Seed Survivor source: https://github.com/TokarevDev/Force_of_Nature_Last_Seed
- WebGL prototypes: https://sd7games.itch.io/
- LinkedIn: https://www.linkedin.com/in/oleksandr-tokarev/

## What I Can Own

- Gameplay systems: combat, weapons, projectiles, enemies, rewards, progression, player flow, and complete playable loops.
- UI flow: UGUI screens, menus, popups, gameplay HUD, result flow, player feedback, and state-driven UI updates.
- Maintainable C#: SRP-style components, event-driven communication where it reduces coupling, service abstractions, and clear data/runtime separation.
- Mobile performance: object pooling, GC allocation awareness, cached references, profiler-minded iteration, and fewer runtime scene searches.
- Delivery workflow: Android builds, Google Play release preparation, WebGL/PC builds, Unity debugging, Git/GitHub source review readiness, refactoring, scene/prefab setup, and technical documentation.

## Main Projects

### Emoji Battle

Released Android game built in Unity 6 and C#, taken from prototype to public Google Play release.

Impact:

- Challenge: turn a small prototype into a complete Android game that could pass store review and be maintained after release.
- Action: owned combat flow, AI, persistence, UI states, popups, ads, Android build preparation, publishing steps, and post-release runtime tuning.
- Result: released a complete Android game on Google Play with reviewable source code, gameplay media, ads flow, persistence, and a complete player loop.

Post-release update: added automatic frame-rate selection for supported 90/120 Hz devices to improve gameplay smoothness on higher-refresh mobile screens.

What it demonstrates:

- Turn-based gameplay loop and board state logic.
- AI strategies for multiple difficulty levels.
- Progression, rewards, avatar selection, settings, and persistent player data.
- Popup service, UI screens, result flow, and animated feedback.
- Unity Ads integration with rewarded/interstitial flow, load timeout, resume handling, and online/offline checks.

Code review map:

- Main project code: `Assets/Scripts/`
- Domain logic: `Assets/Scripts/Domain/`
- Persistence and data services: `Assets/Scripts/Infrastructure/`
- Gameplay, lobby, UI, and popups: `Assets/Scripts/Presentation/`
- Bootstrap and runtime setup: `Assets/Scripts/App/`

Unity vendor packages and imported assets are present in the repository, but the portfolio-relevant code lives under `Assets/Scripts/`.

### Last Seed Survivor

Unity 6 mobile 2D auto-shooter/survival project focused on modular combat, ScriptableObject rewards, segmented enemy behavior, balance simulations, pooling, and Android release preparation.

Impact:

- Challenge: mobile survival gameplay needed scalable combat, rewards, enemy pressure, and tuning instead of one-off prototype logic.
- Action: separated data, runtime systems, UI binding, bootstrap, pooling, segmented enemy logic, and balance simulation tools.
- Result: closed test passed; Android release preparation continues with modular combat, pooled runtime systems, and balance tooling ready for review.

What it demonstrates:

- Modular weapon systems with runtime stat modifiers.
- ScriptableObject-driven rewards, rarities, HP scaling, and pressure tuning.
- Projectile and enemy segment pooling to reduce runtime object churn.
- Reward roll/apply services separated from UI binding and gameplay effects.
- Custom Unity Editor balance lab for deterministic reward/HP simulations.

Code review map:

- Main project code: `Assets/_Project/App/`
- Bootstrap and scene startup: `Assets/_Project/App/Bootstrap/`
- Gameplay combat, weapons, projectiles, and rewards: `Assets/_Project/App/Gameplay/Combat/`
- Segmented enemy systems and balance tooling: `Assets/_Project/App/Gameplay/Enemy/Worm/`
- Presentation/UI-related gameplay flow: `Assets/_Project/App/Presentation/`

Unity vendor packages and imported assets are present in the repository, but the portfolio-relevant code lives under `Assets/_Project/App/`.

## Core Stack

Unity 6, C#, gameplay programming, UI/UGUI, ScriptableObjects, event-driven systems, Strategy Pattern, object pooling, Physics2D, DOTween, Unity Ads, Unity Profiler, Git, GitHub, version control, Android, PC, WebGL.
