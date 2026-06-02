# Last Light Protocol

## Overview

**Last Light Protocol** is a first-person horror prototype made with Unreal Engine 5.6.

The player explores an abandoned industrial facility affected by power failures. The gameplay focuses on darkness, flashlight usage, simple interactions, generators, doors, notes, and atmospheric horror events.

## Project Information

| Information | Value |
|---|---|
| Game Title | Last Light Protocol |
| Team Name | K-Corp |
| Genre | First-Person Horror |
| Engine | Unreal Engine 5.6 |
| Platform | PC |
| Project Type | Prototype / School Project |

## Concept

The game focuses on tension, exploration, and visibility management.

The player must move through dark industrial environments, use a flashlight to see, interact with objects, and restore power systems while discovering what happened inside the facility.

Main gameplay pillars:

- First-person exploration
- Flashlight-based visibility
- Environmental horror
- Power failure events
- Door and generator interactions
- Notes and environmental storytelling
- Abandoned industrial facility atmosphere

## Story

After a major incident inside a remote industrial facility, all communication with the site is lost.

The player enters the facility to investigate and restore the emergency power protocol. Once inside, the power system collapses completely. The flashlight becomes the only reliable source of light.

As the player progresses, they discover that the failure was not accidental. Something inside the facility is still active, and the darkness becomes more dangerous as the player goes deeper.

## Features

### Flashlight System

The flashlight is the player's main tool for navigation and survival.

Current or planned behavior:

- Toggle flashlight on and off
- Navigate dark areas
- Light flicker effect
- Battery-related tension
- Horror events linked to light failures

### Interaction System

The project contains interaction-based gameplay elements.

Examples:

- Open doors
- Interact with generators
- Pick up items
- Inspect objects
- Read notes
- Trigger horror events

### Horror Events

The atmosphere relies on simple horror elements:

- Flickering lights
- Sudden power cuts
- Distant sounds
- Dark corridors
- Industrial rooms
- Environmental tension

### Environment

The project uses industrial, office, forest, and horror-oriented assets to build the level.

Environment elements include:

- Industrial props
- Power station elements
- Office assets
- Electrical equipment
- Doors
- Notes
- Flashlight and battery assets
- Outdoor and indoor decoration assets

## Controls

| Action | Input |
|---|---|
| Move | WASD |
| Look Around | Mouse |
| Interact | E |
| Flashlight | F |
| Sprint | Left Shift |
| Crouch | Ctrl |
| Pause | Escape |

## Project Structure

```txt
Content/
├── DarkwoodDescent/
│   ├── Audio/
│   ├── Blueprints/
│   │   ├── Data/
│   │   ├── Interfaces/
│   │   └── Items/
│   ├── Inputs/
│   │   └── Actions/
│   ├── Levels/
│   ├── Materials/
│   ├── Meshes/
│   │   ├── MapComponents/
│   │   ├── S_Battery/
│   │   ├── S_Central/
│   │   ├── S_CoolingWater/
│   │   ├── S_Flashlight/
│   │   ├── S_HorrorDoor/
│   │   ├── S_HorrorDoorFrame/
│   │   ├── S_Note/
│   │   ├── S_Substation/
│   │   └── S_TransmissionTower/
│   ├── Textures/
│   └── UI/
│
└── Packages_FAB/
    ├── CyberpunkIndustries/
    │   ├── Maps/
    │   ├── Materials/
    │   ├── Meshes/
    │   └── Textures/
    │
    ├── IndustryPropsPack6/
    │   ├── Maps/
    │   ├── Materials/
    │   ├── Meshes/
    │   └── Textures/
    │
    ├── PS1_Office/
    │   ├── Maps/
    │   ├── Materials/
    │   ├── Material_Instance/
    │   ├── Static_Mesh/
    │   └── Textures/
    │
    └── Stylized_Spruce_Forest/
        ├── Audio/
        ├── Blueprints/
        ├── Demo/
        ├── Landscape_Layers/
        ├── Materials/
        ├── Meshes/
        ├── Particles/
        ├── Procedural/
        ├── Textures/
        └── UI/
```

## Main Project Folder

The main gameplay content is located in:

```txt
Content/DarkwoodDescent/
```

This folder contains the custom content of the prototype:

- Audio
- Blueprints
- Inputs
- Levels
- Materials
- Meshes
- Textures
- UI

The external asset packs are separated inside:

```txt
Content/Packages_FAB/
```

This keeps third-party assets separated from the custom gameplay content.

## Technical Elements

The project includes or is expected to include:

- First-person player controller
- Enhanced Input actions
- Flashlight system
- Interaction Blueprint Interface
- Door interaction system
- Generator and power event system
- Pickup and item Blueprints
- UI elements
- Audio assets for horror atmosphere
- Industrial environment meshes

## Installation

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Open the project with **Unreal Engine 5.6**.

3. Open a level from:

```txt
Content/DarkwoodDescent/Levels/
```

4. Press **Play** in the editor.

## Build

To package the project for Windows:

1. Open the project in Unreal Engine.
2. Go to:

```txt
Platforms > Windows > Package Project
```

3. Select an output folder.
4. Wait for the packaging process to finish.

## Git Ignore Recommendation

The following folders should not be committed to Git:

```txt
Binaries/
DerivedDataCache/
Intermediate/
Saved/
.vs/
```

These folders are generated by Unreal Engine and can become very large.

The important project files and folders to keep are usually:

```txt
Config/
Content/
Plugins/
Source/
*.uproject
```

For this project, the most important folder is:

```txt
Content/DarkwoodDescent/
```

## Known Issues

Current prototype limitations:

- Some systems may still use placeholder logic.
- Some imported assets may not be optimized yet.
- Some audio and horror events may still be temporary.
- The level design can still change.
- Some external asset packs may increase the project size.
- The final gameplay loop is still in prototype state.

## Team

**K-Corp**

| Role | Name |
|---|---|
| Game Designer | Mathis Zucchero |
| Developer | Mathis Beugnies |
| Level Designer | Sacha Polerowicz |
| Sound / Atmosphere | Theo Fisch |

## External Assets

External assets are grouped inside:

```txt
Content/Packages_FAB/
```

This folder contains third-party asset packs used to build the environment:

```txt
CyberpunkIndustries/
IndustryPropsPack6/
PS1_Office/
Stylized_Spruce_Forest/
```

Credits and licenses should be checked individually for each external asset pack before public release.

## License

This project is made for educational purposes.

Do not redistribute external assets without checking their original licenses.