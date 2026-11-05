# Trace Lock

A single-file web tool that locks a reference photo to your screen so you can trace it without the image shifting, zooming, or the display going to sleep.

## Features

- **Fit to screen:** The photo fills the viewport while keeping its proportions.
- **Locked view:** Scroll, pinch-zoom, and rubber-banding are disabled.
- **Stays awake:** Uses the Screen Wake Lock API to keep the display on while tracing.
- **Orientation lock:** Locks to the current orientation where the browser allows it.
- **Hold-to-activate buttons:** Fullscreen and Change / Unlock require a 3-second press with a progress ring, which prevents accidental taps.

## Usage

1. Open `Trace Lock.html` in a mobile or desktop browser.
2. Tap **Choose Photo** and pick an image.
3. Trace on top of the screen (for example with a transparent overlay or paper).
4. Hold **Fullscreen** (top right) for 3 seconds to toggle fullscreen.
5. Hold **Change / Unlock** (bottom right) for 3 seconds to return to the picker.

## Notes

- **iPhone Safari** has no page fullscreen, so the Fullscreen button hides itself. Use Share > Add to Home Screen for a bar-free version.
- Wake Lock and orientation lock depend on browser support; both fail quietly if unavailable.
- Images are loaded locally in the browser and are never uploaded anywhere.

## Tech

Plain HTML, CSS, and JavaScript. No dependencies or build step.
