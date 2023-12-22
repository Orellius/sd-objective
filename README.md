# sd-objective

## Overview

Objective Progress UI is a customizable in-game UI resource for FiveM servers, designed to display and track objectives and their progress.

## Features

- **Dynamic Progress Tracking:** Real-time updates of objectives.
- **Customizable Appearance:** Configurable themes, colors, and positions.
- **Smooth UI Transitions:** Fade-in and fade-out effects for UI visibility.
- **Exports for Integration:** Control UI from other resources.

## Installation

1. Clone or download this resource.
2. Place it in the server's resource directory.
3. Add the resource to your server config.

## Usage

### Exports

- `ShowObjectiveUI(title, description, steps)`
- `UpdateProgress()`
- `HideObjectiveUI()`

### Event Handlers

- `sd-objective:client:showUI`
- `sd-objective:client:updateProgress`
- `sd-objective:client:hideUI`

### Example Usage

```lua
-- Start an objective
exports['your-resource']:ShowObjectiveUI('Title', 'Description', 4)

-- Update progress
exports['your-resource']:UpdateProgress()

-- Hide the UI
exports['your-resource']:HideObjectiveUI()
```

## Customization

Customize UI appearance and behavior through `config.js`.
