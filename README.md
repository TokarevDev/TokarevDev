# Unity Gameplay Developer (C#)

I build modular gameplay systems with a focus on maintainability, performance, and clear separation of responsibilities.

Focused on gameplay programming, performance optimization, and improving existing Unity codebases without introducing regressions.

---

## Shipped Game

### Emoji Battle — Mobile Game (Unity 6)

Released on Google Play.

**Problem:**  
Small mobile projects can quickly become hard to maintain when gameplay flow, UI logic, AI behavior, and progression are tightly coupled.

**Solution:**  
Structured the project using MVC/SRP principles, separated UI, state, and gameplay logic, and implemented AI behavior through the Strategy pattern.

**Result:**  
- Released a complete mobile game on Google Play  
- Built predictable turn-based gameplay flow  
- Implemented scalable AI difficulty logic  
- Added progression, save/load, and ads integration  
- Improved maintainability through clearer separation of responsibilities  

Google Play: https://play.google.com/store/apps/details?id=com.sd7gamestudio.emojibattle  
GitHub: https://github.com/SD7Games/Emoji_Battle  

---

## Current Project

### Force of Nature: Last Seed — Modular 2D Auto-Shooter

**Focus:** modular gameplay systems, runtime performance, and fast gameplay iteration.

**Problem:**  
As weapons, rewards, enemies, and combat logic grow, hardcoded values and tightly coupled systems make balancing and feature changes slower.

**Solution:**  
- Built ScriptableObject-based weapon and reward systems  
- Implemented runtime modifiers for weapon upgrades  
- Added projectile pooling to avoid frequent Instantiate/Destroy during gameplay  
- Structured combat, rewards, UI, and enemy logic into smaller responsibilities  
- Developed segmented enemy logic and reward upgrade flow  

**Result:**  
- Faster gameplay balancing without changing core logic  
- Reduced runtime allocations in high object count scenarios  
- Easier extension of weapons, rewards, and combat behavior  
- Cleaner gameplay flow with less coupling between systems  

GitHub: https://github.com/SD7games/Force_of_Nature_Last_Seed  

---

## Additional Playable Prototypes

- **FPS Prototype:** raycast shooting, weapon switching, ScriptableObject weapon configs, NavMesh enemies, pickups, UI, audio/VFX  
- **Galaxy Strike:** 3D space shooter with Input System, Timeline sequences, Particle System weapons, UI, scene flow, PC build  
- **Royal Run:** 3D endless runner with Rigidbody movement, procedural chunk generation, pickups, Cinemachine, UI, WebGL build  
- **Multiplayer Tank Prototype:** Netcode for GameObjects, UGS Relay/Lobby/Auth, ServerRpc/ClientRpc, networked health, coins, leaderboard, minimap  

Playable builds: https://sd7games.itch.io  

---

## Tech Focus

Unity 6, C#, Gameplay Programming, ScriptableObjects, Object Pooling, UGUI, TextMeshPro, New Input System, Physics2D, DOTween, Unity Profiler, Git, Android, PC, WebGL

---

## Contact

Email: OleksandrTokarevDev@gmail.com  
LinkedIn: https://www.linkedin.com/in/oleksandrtokarev/  
Location: Finland
