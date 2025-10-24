# Jimbo Game

A Unity-based 2D game project featuring NPC interactions and tile-based level design.

## Project Overview

This is a Unity game project called "Jimbo Game" developed by DefaultCompany. The project includes a compiled Windows executable along with game assets and graphics resources.

## Project Structure

```
.
├── game/                           # Main game build directory
│   ├── Jimbo Game.exe             # Windows executable
│   ├── UnityPlayer.dll            # Unity runtime library
│   ├── UnityCrashHandler64.exe    # Crash reporting utility
│   ├── WinPixEventRuntime.dll     # Performance profiling support
│   │
│   ├── Jimbo Game_Data/           # Game data and assets
│   │   ├── Managed/               # .NET assemblies and game code
│   │   │   ├── Assembly-CSharp.dll          # Main game scripts
│   │   │   ├── SuperTiled2Unity.dll         # Tiled map integration
│   │   │   ├── Unity.TextMeshPro.dll        # Text rendering
│   │   │   └── UnityEngine.*.dll            # Unity engine modules
│   │   │
│   │   ├── Resources/             # Game resources
│   │   ├── boot.config            # Boot configuration
│   │   ├── app.info               # Application metadata
│   │   ├── globalgamemanagers*    # Unity scene management
│   │   ├── level0                 # Level data
│   │   └── sharedassets0.*        # Shared game assets
│   │
│   └── MonoBleedingEdge/          # Mono runtime environment
│       ├── EmbedRuntime/          # Embedded Mono runtime
│       └── etc/                   # Runtime configuration
│
└── gfx/                           # Graphics and design assets
    ├── Dealer.png                 # Dealer character sprite
    ├── NPC_test.png               # Test NPC sprite
    ├── npc_Quique.png             # Quique NPC character sprite
    └── Tiled2Unity-1.0.13.2-win64-setup.msi  # Tiled map editor installer
```

## Technical Details

### Engine & Framework

- **Engine**: Unity (Windows build)
- **Scripting Runtime**: Latest .NET version
- **Graphics**: Native graphics jobs enabled
- **VR Support**: Disabled
- **HDR Display**: Disabled

### Key Dependencies

- **SuperTiled2Unity**: Integration for Tiled map editor, enabling tile-based level design
- **TextMeshPro**: Advanced text rendering system
- **Unity Physics2D**: 2D physics simulation
- **Unity UI**: User interface system

### Game Features

Based on the project structure, the game appears to include:

- Tile-based level design (via SuperTiled2Unity)
- NPC character system (Dealer, Quique, and test NPCs)
- 2D sprite-based graphics
- Scene management with at least one level

## Graphics Assets

The `gfx/` folder contains character sprites and design resources:

- **Dealer.png**: Character sprite for a dealer NPC
- **npc_Quique.png**: Character sprite for an NPC named Quique
- **NPC_test.png**: Test sprite for NPC development

## Development Tools

The project uses Tiled2Unity (v1.0.13.2) for level design, which allows creating tile-based maps in the Tiled Map Editor and importing them into Unity.

## Platform

- **Target Platform**: Windows (64-bit)
- **Build Type**: Standalone executable

## Running the Game

To run the game:

1. Navigate to the `game/` directory
2. Execute `Jimbo Game.exe`
3. Ensure all DLL files and the `Jimbo Game_Data/` folder remain in the same directory

## Notes

- This is a compiled build; source code is not included in this repository
- The game uses the Mono scripting backend
- Native graphics jobs are enabled for improved rendering performance
