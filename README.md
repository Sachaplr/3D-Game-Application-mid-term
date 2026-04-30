# README

## Project Title
Third Person Combat Game - Unreal Engine 5

## Project Overview
This project is a third-person shooter combat game built in Unreal Engine 5 using the Third Person template and primitive assets. The player fights against three AI-controlled enemies inside an arena. Both the player and enemies use projectile bullets, have health systems, and the game ends with a win or lose screen depending on the result.

## Core Features
- Third-person player movement and camera
- Player shooting system with projectile bullets
- Ammo system (100 bullets maximum)
- Three AI enemies with independent HP and ammo
- Enemy AI using Behavior Tree and Blackboard
- Enemy line-of-sight detection using line traces
- Enemy retreat behavior when player is too close
- HUD showing player HP, ammo, and enemy HP bars
- Win / Lose screen with restart button

## Controls
- WASD = Move
- Mouse = Look around
- Space = Jump
- Left Mouse Button = Fire

## AI Behavior
Enemies use a Behavior Tree with three main states:
- Retreat: Move away when player is too close
- Attack: Shoot when player is visible
- Roam: Move randomly when player is not detected

## Win / Lose Conditions
### Win
Defeat all three enemies.

### Lose
- Player HP reaches 0
- Player ammo reaches 0 while at least one enemy is still alive

## Design Decisions
- Used primitive meshes for level obstacles to match assignment requirements.
- Kept projectile damage simple (1 hit = 1 HP).
- Used separate HP and ammo values for each enemy.

## Known Issues
- Enemy movement may occasionally pause briefly near obstacles.
- Projectile collisions may feel inconsistent at very close range.
- UI bars may update one frame late in rare cases.

## Improvements If More Time Was Available
- Better enemy cover usage and smarter AI tactics
- Sound effects and shooting animations
- Multiple levels or wave mode
- Better visual effects for hits and explosions
- Improved UI polish

## Sources Used
- Unreal Engine 5 Official Documentation
- Unreal Engine YouTube tutorials
- Unreal Engine Forums / Community posts
- Course lecture materials
- ChatGPT for debugging help and documentation support

## Build / Run
Open the `.uproject` file in Unreal Engine 5 and run the level `Arena_Main`.

## Author
Sacha Polerowicz 7702241