# Darkwood Descent – Lecture 11 Prototype

## Overview
This project is a first-person horror prototype developed in Unreal Engine 5.6 as part of the Lecture 11 implementation tasks.

The prototype focuses on:
- Player movement and camera systems
- Interactive environment objects
- Examination mechanics
- Flashlight and battery management
- Environmental horror atmosphere
- Basic resource management gameplay

---

# Implemented Features

## Player Controller & Movement
- First-person movement system using Enhanced Input
- Mouse look system
- Sprint functionality
- Head bob system with:
  - Walking and sprint variations
  - Smooth interpolation
  - Horizontal and vertical offsets

---

## Interaction System
Implemented a complete interaction tracing system:
- Camera line trace
- Interface-based interaction system (`BPI_Interactable`)
- Dynamic interaction prompts
- Current interactable tracking

---

## Door System
Implemented `BP_Door` featuring:
- Smooth timeline-based opening animation
- Open / close state handling
- Adjustable opening angle
- Locked door support
- Dynamic interaction prompts

---

## Examination System
Implemented an object inspection system:
- Object attachment to camera anchor
- Mouse-based object rotation
- Zoom functionality using mouse wheel
- Player movement disabling during examination
- Object restoration after inspection

The system uses `BPI_Examinable`.

---

## Flashlight System
Implemented a complete flashlight survival mechanic:
- Toggleable flashlight
- Battery drain system
- Dynamic battery UI
- Flickering behavior based on battery level
- Automatic shutdown at 0%
- Battery pickup system

Battery states dynamically affect gameplay atmosphere.

---

## UI Systems
Implemented:
- Interaction prompt widget
- Battery indicator widget using a 4-bar system
- Dynamic UI updates

---

## Horror Environment
Created a small horror test room featuring:
- Dark enclosed environment
- Dynamic flashlight lighting
- Volumetric fog
- Post-processing effects
- Film grain
- Vignette
- Ambient occlusion

The room contains:
- Interactive door
- Examinable note
- Battery pickup

---

# Technical Architecture

## Interfaces
- `BPI_Interactable`
- `BPI_Examinable`

## Main Blueprints
- `BP_HorrorCharacter`
- `BP_Door`
- `BP_BatteryPickup`
- `BP_ExaminableNote`

## Widgets
- `WBP_InteractPrompt`
- `WBP_BatteryMeter`

---

# Known Limitations
- Inventory/key system is partially prepared but not fully implemented
- Environment art remains placeholder/blockout quality
- Sound design implementation is minimal
- Flicker system could be further optimized
- AI systems are not yet implemented

---

# Additional Notes
The project was designed with modularity in mind to support future systems such as:
- Enemy AI
- Larger mansion environments
- Advanced inventory systems
- Audio-driven horror gameplay
- Save/load systems
- Resource scarcity mechanics

The prototype establishes the technical and atmospheric foundations for a larger survival horror experience.