# Drone Wars - Game Design Questions

## Technical Stack & Platform

**1. What platform should the game run on?**
- [ ] Web browser (HTML5/JavaScript)
- [Y] Desktop application (Electron, Python, Unity, etc.)
- [ ] Mobile app (iOS/Android)
- [ ] Other: _______________

**2. What technology stack would you prefer for the voice recognition?**
- [Y] OpenAI Whisper API
- [ ] Web Speech API (free, browser-based)
- [ ] Google Cloud Speech-to-Text
- [ ] Azure Speech Services
- [ ] Other: _______________

**3. What technology stack would you prefer for the game engine/visualization?**
- [ ] Three.js (3D web graphics)
- [Y] Unity (C#)
- [ ] Unreal Engine
- [ ] Pygame (Python)
- [ ] Phaser.js (2D web game framework)
- [ ] Custom HTML5 Canvas
- [ ] Other: _______________

## Gameplay Mechanics

**4. How should time work in the game?**
- [Y] Real-time (1:1 with real time)
- [ ] Accelerated time (e.g., 1 hour = 1 minute)
- [ ] Turn-based with time units
- [ ] Pausable real-time with speed controls
- [ ] Other: _______________

**5. How many people need to be saved to win?**
- [ ] A specific number (e.g., 5, 10, 20)
- [ ] All of them (100%)
- [Y] A percentage (e.g., 80%)
- [ ] Variable based on difficulty level
- [ ] Other: _______________

**6. What happens if the Titanic hits an iceberg?**
- [ ] Game over immediately
- [ ] Time limit decreases (still can save people)
- [ ] Some people become harder to rescue
- [Y] Damage system affects gameplay
- [ ] Other: _______________

**7. How are people located on the Titanic?**
- [ ] Automatically shown on radar/LIDAR
- [ ] Must be found by exploring with drones
- [ ] Visible on a deck/cabin map
- [Y] Combination of exploration and clues
- [ ] Other: _______________

## Voice Control & Commands

**8. What voice command structure should be used?**
- [Y] Natural language (e.g., "Send drone to grid A5")
- [ ] Command-style (e.g., "DRONE EXPLORE A5")
- [ ] Mix of both
- [ ] Menu-based voice navigation
- [ ] Other: _______________

**9. How should the system handle command confirmation?**
- [ ] Visual feedback in command line only
- [ ] Voice confirmation ("Command received: Send drone to A5")
- [Y] Both visual and voice
- [ ] No confirmation, just execute
- [ ] Other: _______________

**10. Should voice commands be interruptible?**
- [Y] Yes, can cancel mid-command
- [ ] No, must complete command before new one
- [ ] Queue system for multiple commands
- [ ] Other: _______________

## Grid System & Navigation

**11. How should the 32x32 grid be labeled?**
- [ ] Letters A-Z + Numbers 1-32 (e.g., A1, B15, Z32)
- [Y] Numbers only (1-1, 1-2, ..., 32-32)
- [ ] Letters for rows, numbers for columns
- [ ] Custom coordinate system
- [ ] Other: _______________

**12. What size does each grid cell represent in real-world distance?**
- [ ] 1 km x 1 km
- [Y] 500 m x 500 m
- [ ] 2 km x 2 km
- [ ] Variable based on zoom level
- [ ] Other: _______________

**13. Should the grid be visible on screen at all times?**
- [ ] Yes, always visible with labels
- [ ] Only visible when hovering/selecting
- [ ] Optional toggle
- [Y] Never visible, reference only
- [ ] Other: _______________

## Radar & Iceberg System

**14. How should icebergs be detected?**
- [ ] Automatically when drone gets within range
- [ ] Requires drone to actively scan the area
- [ ] Combination of passive and active detection
- [Y] Pre-populated from database, drones verify
- [ ] Other: _______________

**15. What makes an iceberg a "risk"?**
- [ ] Size (larger = more risk)
- [ ] Proximity to Titanic's path
- [ ] Speed/direction of movement
- [Y] Combination of factors
- [ ] Other: _______________

**16. Should icebergs move?**
- [ ] Yes, drifting with ocean currents
- [ ] Static positions only
- [Y] Some move, some static
- [ ] Other: _______________

**17. How should the iceberg database work?**
- [Y] Historical data from 1912
- [Y] Realistic randomly generated based on North Atlantic patterns
- [ ] Pre-scripted scenario
- [Y] Procedurally generated per game
- [ ] Other: _______________

## Drone Mechanics

**18. How many drones can be active simultaneously?**
- [ ] One at a time
- [ ] Multiple (specify number: _______)
- [ ] Unlimited
- [ ] Limited by resources/tech
- [ ] Other: _______________

**19. What happens when a drone reaches its destination?**
- [ ] Hovers and scans automatically
- [Y] Stops and waits for next command
- [ ] Returns to base automatically
- [Y] Player must command return
- [ ] Other: _______________

**20. How should the fibre optic cable limit work?**
- [Y] Maximum distance from base
- [Y] Cable can get tangled/damaged
- [ ] Unlimited length
- [ ] Limited by deployment ship position
- [ ] Other: _______________

**21. What happens if a drone crashes or is lost?**
- [ ] Game over
- [ ] Can deploy replacement (if available)
- [ ] Permanent loss affects gameplay
- [Y] Just respawns
- [ ] Other: _______________

## Boat/Ship Mechanics

**22. How should the rescue boats work?**
- [ ] Autonomous once deployed
- [ ] Player commands each boat
- [ ] Follow waypoints set by player
- [Y ] AI-assisted with player oversight
- [ ] Other: _______________

**23. How many rescue boats are available?**
- [ ] Fixed number (specify: _______)
- [ ] Unlimited
- [y and can only be used if we survive the first hour of avoiding icebergs] Limited by deployment capacity
- [ ] Variable based on mission objectives
- [ ] Other: _______________

**24. Should the Titanic be controllable or just observable?**
- [ ] Fully controllable (player steers)
- [y] Can suggest course changes
- [y] Observation only (historical path)
- [ ] Emergency override capability
- [ ] Other: _______________

## Visual & UI Design

**25. What visual style should the game have?**
- [ ] Realistic/serious
- [y] Stylized/artistic
- [ ] Retro/pixel art
- [ ] Minimalist/functional
- [ ] Other: _______________

**26. Should the 4-quadrant split be resizable?**
- [ ] Yes, user can adjust sizes
- [ ] Fixed equal quarters
- [y] Fixed but different sizes
- [ ] Optional full-screen modes
- [ ] Other: _______________

**27. How should the LIDAR visualization look?**
- [ ] Point cloud 3D view
- [ ] Top-down heat map
- [ ] Side-view cross-section
- [y] Combination view
- [ ] Other: _______________

**28. Should there be additional UI elements (menus, HUD, etc.)?**
- [y] Minimal, just the 4 quadrants
- [y] Add status bars, timers, resource indicators
- [ ] Contextual overlays
- [ ] Full game menu system
- [ ] Other: _______________

## People to Rescue

**29. Which famous people should be in the game?**
- [y] Historical figures who were actually on Titanic
- [ ] Mix of real and fictional
- [ ] Completely fictional but historically plausible
- [ ] User can customize list
- [ ] Other: _______________

**30. How should people be prioritized for rescue?**
- [ ] All equal priority
- [y] Value-based (wealthy = higher priority)
- [ ] First come, first served
- [ ] Strategic (location, time, difficulty)
- [ ] Other: _______________

**31. Should there be personality/interaction with the people?**
- [y] Yes, they can communicate or react
- [ ] No, just objects to collect
- [ ] Minimal (just names/status)
- [y] Story elements/dialogue
- [ ] Other: _______________

## Scoring & Progression

**32. How should the game track success?**
- [ ] Simple count of people saved
- [ ] Points based on person's value/importance
- [y] Time-based scoring
- [ ] Efficiency rating (people/time/resources)
- [ ] Other: _______________

**33. Should there be multiple difficulty levels?**
- [y] Yes, easy/medium/hard
- [ ] No, single difficulty
- [ ] Adaptive difficulty
- [ ] Scenario-based variations
- [ ] Other: _______________

**34. Should there be a tutorial or learning mode?**
- [y] Yes, full tutorial
- [ ] No, learn by playing
- [ ] Optional hints/help system
- [ ] Just a command reference
- [ ] Other: _______________

## Additional Features

**35. Should there be a save/load system?**
- [y] Yes, save at any time
- [ ] Checkpoint-based saves
- [ ] No saves (one-session game)
- [ ] Auto-save only
- [ ] Other: _______________

**36. Should there be multiplayer capabilities?**
- [y differnt vices at once how to ideentify ?] Yes, cooperative multiplayer
- [ ] Yes, competitive multiplayer
- [ ] Single player only
- [ ] Optional multiplayer
- [ ] Other: _______________

**37. Should there be weather/environmental effects?**
- [] Yes, fog, storms affect visibility/operations
- [y ] No, clear conditions only
- [ ] Optional weather effects
- [ y] Historical weather from that night
- [ ] Other: _______________

**38. Should there be resource management (fuel, battery, etc.)?**
- [ y but enought to last till through the icebergs in 1 hour] Yes, manage all resources carefully
- [ ] No, unlimited resources
- [ ] Some resources limited (specify which)
- [ ] Other: _______________

## Timeline & Development

**39. What's the target scope for the initial version?**
- [ y] Full-featured complete game
- [ ] Playable prototype/demo
- [ ] MVP (Minimum Viable Product)
- [ ] Proof of concept
- [ ] Other: _______________

**40. Are there any specific technologies or libraries you want to use or avoid?**
- [y ] Use: freely available or best chice for this type of game 
- [ ] Avoid: _______________
- [ ] No preference

