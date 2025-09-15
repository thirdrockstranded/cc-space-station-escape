# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Godot 4.x roguelike game** called "Space Station Escape" - a real-time survival horror game set on an alien-infested space station. The project serves as a learning platform for building foundational systems that will transfer to a larger Alternate Reality remake project.

## Technology Stack

- **Engine**: Godot 4.x
- **Language**: GDScript (engine-native language preferred over C#)
- **Platform**: PC initially
- **Art Style**: Retro/pixelated aesthetic

## Development Commands

Since this is a Godot project, development happens primarily through the Godot editor. Key workflows:

- **Open Project**: Launch Godot editor and open `project.godot`
- **Run Game**: F5 in Godot editor or play button
- **Export**: Project → Export in Godot editor
- **Version Control**: Standard git workflow (no special build commands needed)

## Architecture & Core Systems

### Game Structure

- **Genre**: Real-time roguelike with resource management
- **Setting**: Space station under alien attack
- **Core Loop**: Exploration → Resource Management → Combat

### Key Godot Components to Implement

- `CharacterBody2D` for player movement
- `TileMap` for procedural level generation
- `Area2D` for searchable containers and interactions
- `RayCast2D` for flashlight visibility mechanics
- State machines for AI behaviors

### Level Design Architecture

- **Room Types**: medical, storage, living quarters, labs, maintenance
- **Generation**: Rectangular rooms connected by corridors with logical item placement
- **Progression Gates**: Locked doors (keycards), debris blocking paths, hazard zones

### Core Systems Priority

1. **Exploration Mechanics**: WASD movement, flashlight with battery drain, fog of war
2. **Resource Management**: Limited oxygen, power cells, emergency rations
3. **Combat Systems**: Real-time combat with environmental hazards

## File Organization

Expected Godot project structure once development begins:

- `scenes/` - .tscn scene files
- `scripts/` - .gd script files  
- `assets/` - sprites, audio, etc.
- `project.godot` - main project file
- `.godot/` - engine cache (should be gitignored)

## Version Control Setup

The project should use:

- Git with Git LFS for large assets
- Track: `*.png`, `*.jpg`, `*.wav`, `*.ogg`, `*.fbx`
- `.godot/` should be added to `.gitignore`
- Consider separate "raw assets" folder for source files

## Game Design Context

Reference `docs/project-context.md` for detailed game design, narrative elements, and technical implementation notes. The med bay opening sequence serves as the tutorial introduction, teaching core mechanics through environmental storytelling.

This project connects thematically to a planned Alternate Reality remake, sharing alien antagonists and core gameplay mechanics while providing a constrained environment for rapid iteration and testing.