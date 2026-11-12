# Techfest 30: 3D Interactive Website

A scroll-driven 3D website for Techfest, IIT Bombay (30th edition), built with **Three.js (r128)**, plain HTML, CSS and JavaScript. No build step.

**Built by:** Babun Mal, Bhadrak Autonomous College (Techfest College Ambassador)

## What you will see
1. **Origin:** a glowing 3D core (wireframe icosahedron, emissive dodecahedron and three orbiting rings) that tilts with your mouse.
2. **Core:** the camera orbits the core as you scroll.
3. **Experience:** the camera flies through a corridor of four interactive 3D objects: a gear (Robowars), an atom (Workshops), a microphone (Lectures) and a torus knot (Exhibitions). Hover to wake an object up, click or tap to open its details. Buttons below also open them, for keyboard and touch users.
4. **Portal:** a tunnel of pulsing rings the camera travels through.
5. **Join:** a large glowing "30" appears at the end with a call to action.

## Techniques
- Scroll progress drives a keyframed camera path with eased interpolation, smoothed with damping
- Background and fog colours blend between sections for dynamic transitions
- Raycasting for hover and click on 3D objects
- Canvas-generated textures for 3D labels and the final "30"
- Starfield particle system, tunnel rings and per-object animation
- Responsive: lower pixel ratio and fewer particles on phones
- Accessibility: `prefers-reduced-motion` support, labelled controls, Escape closes the modal, WebGL fallback message

## Run it
Open `index.html` in a modern browser with an internet connection (Three.js loads from cdnjs and fonts from Google Fonts). Scroll to travel through the scene.

