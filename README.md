# Wardogs Fire Control

Mortar and artillery calculator for [Wardogs](https://store.steampowered.com/app/1867240/WARDOGS/).

**Use it:** https://ahmadqwer.github.io/wardogs-fire-control/

Paste your mortar's map coordinates and the target's. You get:

- **RNG**: the range in meters to set on the scope's RNG scale
- **Heading**: the compass heading, shown the way the scope compass shows it (for example `251° W`)
- **Reach**: whether the L81 mortar or the artillery tank can hit that distance
- **Adjust fire**: paste where a shell landed to get the corrected RNG and how far to turn

## Getting coordinates in game

1. Open the map and zoom in on your mortar. Right-click it and choose **Mark coordinates**.
2. The coordinates appear in chat as `x98.43, y110.38`. Press `Ctrl+A`, then `Ctrl+C`, and paste them into the page.
3. Do the same on the target.

## The math

Map coordinates are in 100 m units. Distance = √(Δx² + Δy²) × 100 m. The heading is measured clockwise from north (map y grows to the north).
The distance is flat map distance, so a target well above or below you can land long or short. Adjust fire corrects for that.

Method from [SwoleBenji's mortar guide](https://www.youtube.com/watch?v=9X8U-eHCMgI). Fan-made, not affiliated with the developers of Wardogs.
