# Programmable LED Dance Costumes Codebase
*By: Siddharth Chattoraj*

Full Pixelblaze pattern scaffold codebase for “Programmable LED Dance Costumes: Designing Embodied Wearable Technology to Enhance Kinesthetic Expression for Dance Performance.” The performance featuring this code took place at the University of California, Santa Barbara on March 5, 2026. The video can be found at [https://vimeo.com/1199302223](https://vimeo.com/1199302223), and it demonstrates the programmable LED dance costumes in live performance, including pixel-mapped lighting patterns and movement-based visual expression.

Siddharth Chattoraj. 2026. Programmable LED Dance Costumes: Designing Embodied Wearable Technology to Enhance Kinesthetic Expression for Dance Performance. In Special Interest Group on Computer Graphics and Interactive Techniques Conference Posters (SIGGRAPH Posters ’26), July 19–23, 2026, Los Angeles, CA, USA. ACM, New York, NY, USA, 3 pages. https://doi.org/10.1145/3799825.3818701

More information about coding in Pixelblaze can be found on the [ElectroMage Language Reference](https://electromage.com/docs/language-reference). This work used a Pixelblaze V3 Standard in each costume. All code is free to reuse with attribution.

## Pattern Scaffolds (15 Total)

All pattern scaffolds can be modified live or reset at any time. Each code file creates a toggle-based UI system, where designers can increase or decrease effects in real time. Within the toggles, "On" or "Off" does not matter. The system is designed as such, rather than built to modify patterns via sliders, to enable the designer to reset the pattern scaffold.

### Unified Patterns (Both costumes respond together)

#### Pattern1.js - **Twilight Ripples**
Ripple effect pattern with base hue up/down and reset toggles, plus a smooth ripple/shimmer animation.

#### Pattern2.js - **Night Sky Field**
Starfield and nebula pattern with background-level down, star-density up, and reset toggles, plus slow nebula drift and twinkle.

#### Pattern3.js - **Kinetic Nova & Power Streams**
High-energy drop/stream pattern with A5 hyperdrive, accent hue up/down, and reset toggles, plus wash, flicker, and stream motion.

#### Pattern4.js - **Sky and Earth Rings**
Concentric top/skirt ring pattern with warmth up/down and reset toggles, plus smoothed warmth and moving ring animation.

#### Pattern5.js - **Happiness Thinning**
Smooth top/bottom wave pattern with hue up/down and reset toggles, plus crossing yellow/orange waves and a steady speed.

#### Pattern7.js - **The Midnight Tide**
Tidal takeover pattern with tide up/down and reset toggles, plus automatic blend, shimmer surges, and layered drift.

#### Pattern8.js - **Spectral Starfields**
Galaxy backdrop with galaxy/snake hue up, snake count up/down, multi-hue, and reset toggles, plus moving snakes and twinkling starfields.

#### Pattern12.js - **Resonant Inferno**
Flame pattern with speed, heat, burst, and hue toggles plus reset, with wind oscillation, flicker, and pulse-driven bursts.

#### Pattern14.js - **Turbo Thermal Crescendo**
Dual-layer thermal pattern with sunrise, hue, turbo, and reset toggles, plus cross-fade, pulse, and convection motion.

#### Pattern15.js - **Breathing Ending**
Simple ending pattern with no toggles, just a unified breathing brightness pulse across all 124 LEDs.

### Patterns with Independent Skirt Control (Can control each costume independently)

#### Pattern6_node.js - **The Dichromatic Garden**
Uses `nodeId()` to independently control each costume. Has 4 quadrant hues (top/skirt left/right), overdrive level and hue toggles, plus drifting motion.

#### Pattern9_node.js - **Psychedelic Rainbow Cascade**
Uses `nodeId()` to independently control each costume. Includes top/skirt hue toggles, craziness up/down, reset, and drifting rainbow pulse motion.

#### Pattern10_node.js - **Flamboyant Rainbow Vortex**
Uses `nodeId()` to independently control each costume. Adds hue, speed, craziness, and reset toggles, with rotating vortex, pulse, and glitch-like breakup effects.

#### Pattern11_node.js - **Dazzle Glitch**
Uses `nodeId()` to independently control each costume. Includes sprout/growth toggles for both layers, glitch toggle and hue, reset, plus bloom and shimmer animations.

#### Pattern13_node.js - **Final Showdown**
Uses `nodeId()` to independently control each costume. Includes node hue, fire, agitation, reset, and climax toggles, with a climax override animation.

## Additional Files

#### PixelMapper.js
Pixel mapping configuration for the LED costume hardware. Defines 3D coordinates for all 124 LEDs used in Pixelblaze's Pixel Mapper.
- **Top section**: 40 LEDs (8 columns × 5 rows)
- **Skirt section**: 84 LEDs (12 columns × 7 rows)

#### SystemDiagram.js
3D visualization tool using p5.js to display the costume LED layout and system architecture. Includes interactive orbit controls for rotating and zooming the visualization.

#### Loop20Patterns.js
Master pattern collection file containing all pattern scaffolds compiled for auto-looping installations. Cycles through patterns every 30 seconds with hard cuts between them.