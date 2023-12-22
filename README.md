# sd-objective

It provides an elegant and intuitive way to display objectives and track progress in-game. With customizable themes, positions, and progress animations.

# Features
- Dynamic Progress Tracking: Display and update objectives and their progress in real-time.
- Customizable Appearance: Configure themes, colors, and positions to match your game's style.
- Fade-In/Fade-Out Animations: Smooth transitions for showing and hiding the UI.
- Exports for Easy Integration: Use exports to control the UI from other resources.

# Installation
1. Clone the repository or download the resource.
2. Place the resource in your server's resource directory.
3. Add the resource to your server's configuration.
4. Ensure config.js is correctly set up to reflect your preferred settings.

# Usage
## Exports
ShowObjectiveUI(title, description, steps): Display the UI with a specific objective.

title: The title of the objective.
description: A brief description of the objective.
steps: Total number of steps to complete the objective.

UpdateProgress(): Update the progress of the current objective. Should be called when a step towards the objective's completion is made.

HideObjectiveUI(): Immediately hide the UI, regardless of progress.

# Event Handlerssd-objective:client:showUI: Triggers the UI to show with the specified objective details.
sd-objective:client:updateProgress: Updates the progress of the objective.
sd-objective:client:hideUI: Hides the UI immediately.
Examples
Starting an Objective
lua
Copy code
-- Starting an objective with 4 steps
exports['your-resource-name']:ShowObjectiveUI('Objective Title', 'Objective Description', 4)
Updating Progress
lua
Copy code
-- Update progress typically called upon completion of a step
exports['your-resource-name']:UpdateProgress()
Hiding the UI
lua
Copy code
-- Hide the UI
exports['your-resource-name']:HideObjectiveUI()
