# PSYCHRONIC_GifAnimationMZ

**RPG Maker MZ Plugin**

Plays animated GIFs on specified events with optional zoom and z-index (MZ).

## What It Does

This plugin allows you to play animated GIFs on specified events in RPG Maker MZ. You can control whether the GIF should loop or not, set the transparency level, specify a zoom level, and control the z-index.

## Plugin File

- `PSYCHRONIC_GifAnimationMZ.js`
- Version: `2.0`
- Target: RPG Maker MZ
- Author: Psychronic
- URL: https://psychronic.itch.io

## Plugin Commands

- `PlayGif`
- `StopGif`

## Installation

1. Download `PSYCHRONIC_GifAnimationMZ.js`.
2. Place it in your RPG Maker MZ project's `js/plugins/` folder.
3. Enable it from the RPG Maker Plugin Manager.
4. Configure any plugin parameters or commands listed below.

## Full Plugin Help

### Introduction
This plugin allows you to play animated GIFs on specified events in RPG
Maker MZ. You can control whether the GIF should loop or not, set the
transparency level, specify a zoom level, and control the z-index.

### Plugin Commands (RPG Maker MZ)
Use the Plugin Command interface in RPG Maker MZ's event editor to access
the following commands:

1. Play GIF
Plays an animated GIF on a specified event.
Parameters:
- Event ID: The ID of the event where the GIF will be displayed.
- GIF Name: The name of the GIF file (without .gif extension).
Files should be placed in: img/animations/
- Loop: true or false, whether the GIF should loop continuously.
- Transparency: 0-255 (0=fully transparent, 255=fully opaque).
- Zoom: Magnification level (e.g., 1=normal, 2=2x size).
- Z-Index: Layer depth (higher=in front, 0=behind player).

2. Stop GIF
Stops the GIF animation on a specified event.
Parameters:
- Event ID: The ID of the event to stop the GIF on.

### Performance Notes
This plugin uses Web Workers to decode GIF frames in a separate thread,
ensuring smooth performance even with large, complex GIFs. The main game
thread is not blocked during GIF processing

### Terms of Use
cc0 (Public Domain), can use without credit, although credit is appreciated
https://psychronic.itch.io

## Source

This standalone repository is generated from the latest PSYCHRONIC plugin source in the RPG Reactor Complex template.

## License

MIT. See `LICENSE`.
