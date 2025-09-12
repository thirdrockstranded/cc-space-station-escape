# Space Station Escape - Project Context

## Project Overview

This is a learning project designed as preparation for a larger **Alternate Reality remake**. The goal is to create a publishable roguelike game while building foundational skills and systems that will transfer to the more complex AR project.

## Game Concept

**Setting:** Space station under alien attack
**Genre:** Real-time roguelike with resource management
**Theme:** Post-apocalyptic survival with sci-fi horror elements

### Narrative Hook
- Player wakes up in medical bay after alien invasion has begun
- The same portal-opening aliens from Alternate Reality have attacked the station
- Most crew are missing/dead, station systems failing
- Must escape to shuttle bay/escape pods before being captured
- Creates thematic bridge to the planned Alternate Reality remake

## Core Gameplay Loop

### 1. Exploration Phase (Primary Focus)
- Navigate procedurally generated station levels
- Manage limited resources (flashlight battery, oxygen, food)
- Search containers/rooms for supplies and lore
- Avoid or sneak past alien hunters when possible

### 2. Resource Management Phase (Secondary Focus)
- Oxygen recyclers failing (limited air in sealed sections)
- Power cells for doors/elevators running down
- Emergency rations scattered around
- Makeshift weapons from engineering tools

### 3. Combat Phase (Tertiary Focus)
- Real-time combat system
- Environmental hazards
- Risk/reward decision making

## Technical Specifications

**Engine:** Godot 4.x
**Primary Language:** GDScript (despite C# experience, staying with engine-native language)
**Platform:** PC initially
**Art Style:** Retro/pixelated aesthetic matching AR project goals

### Why Godot?
- Excellent 2D capabilities with pixel-perfect rendering
- Strong 3D support for potential future AR project
- Node-based architecture maps well to software engineering principles
- Free and open-source
- Purpose-built for games (no fighting the language)

## Starting Implementation

### Med Bay Opening Sequence
**Environmental Storytelling:**
- Player wakes on medical bed, IV attached
- Flickering lights, sparking panels
- Medical equipment beeping/silent
- Blood stains, overturned furniture
- Covered body on nearby bed

**Tutorial Elements:**
- Medical terminal (interface tutorial)
- Scattered supplies (inventory introduction)
- Emergency flashlight (lighting mechanics)
- Keycard access (progression gates)
- Station schematic (layout reference)

**First Gameplay Beats:**
1. Examine surroundings (interaction system)
2. Find flashlight (visibility mechanics)
3. Access terminal (interface + lore)
4. Search supplies (inventory management)
5. Door puzzle (keycard system)
6. Enter corridor (world transition)

### Core Systems to Build First

**Exploration Mechanics:**
- Smooth WASD movement with collision
- Flashlight cone with battery drain
- Fog of war system
- Searchable containers
- Interactive terminals
- Audio cues for discovery/danger

**Level Generation:**
- Rectangular rooms connected by corridors
- Room types: medical, storage, living quarters, labs, maintenance
- Logical item placement
- Connectivity validation

**Progression Gates:**
- Locked doors (keycards/tools required)
- Debris blocking paths
- Hazard zones requiring equipment
- Elevator/stair access to other decks

## Technical Implementation Notes

### Godot-Specific Tools:
- `TileMap` for level generation
- `Area2D` for searchable containers
- `RayCast2D` for flashlight visibility
- `CharacterBody2D` for player movement
- State machines for AI behaviors

### Version Control Setup
- **Primary:** Git with Git LFS for large assets
- Track: `*.png`, `*.jpg`, `*.wav`, `*.ogg`, `*.fbx`
- Add `.godot/` to `.gitignore`
- Consider separate "raw assets" folder for source files

## Skills Transfer to AR Project

This roguelike will provide hands-on experience with:
- Character stats and progression systems
- Real-time movement and collision
- Inventory management
- Procedural generation techniques
- Save/load with permadeath options
- Resource management mechanics
- Environmental storytelling
- Audio design and atmosphere

## Development Approach

**Priorities:**
1. **Exploration** - Core movement, discovery, and navigation
2. **Resource Management** - Limited supplies create tension
3. **Combat** - Action systems for player agency

**Scope Management:**
- Start with single station level
- Focus on core loop satisfaction
- Build complexity iteratively
- Maintain publishable quality standards

## Connection to Alternate Reality Remake

This project serves as a practical training ground for the ambitious AR remake, sharing:
- Same alien antagonists (narrative continuity)
- Real-time gameplay mechanics
- Resource scarcity and tough choices
- Environmental storytelling through terminals/logs
- Urban exploration translated to station navigation
- Stealth/avoidance mechanics

The confined space station setting allows for faster iteration and testing of systems that will scale up to AR's open city environment.