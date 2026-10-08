# Son Room Camera Editor

A small browser-only 3D camera editor for visualizing the same fixed room and doorway from different camera positions.

## Website

- Home: https://rayray12zx3-sys.github.io/son-room-camera-editor/
- S01 camera editor: https://rayray12zx3-sys.github.io/son-room-camera-editor/s01-camera/

**The addresses are only live once GitHub Pages is enabled and the deployment succeeds.**

## How to enable GitHub Pages on GitHub Free

This repository is public and contains only reviewed, static camera-editor content. In this repository:

1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Choose branch **main** and folder **/(root)**, then click **Save**.
4. Wait for the Pages deployment to complete. Open the website and verify the camera viewport is visible.

Future pushes to `main` automatically update the published site with this setup; no separate Actions workflow needed.

## Using the tool

- Drag the orange point on the plan to reposition the hallway camera.
- Drag the 9:16 viewport to turn the camera; adjust height/FOV with sliders.
- Camera starts at the approved S01 trial position, with the fixed door geometry unchanged.
- Camera changes are stored in the **current browser** via `localStorage`, not synced online.
- Export PNG and JSON for reference, backup or passing a new camera setup to the production project.
- **Restore approved S01 camera** resets the editor to the fixed accepted starting position.

No AI model API, generation service, CDN, or login is needed for camera moves. The website itself is publicly readable. Original source photos, private production notes, and character reference assets were not copied here.

## Scope and caveats

- This is a simplified greybox with *approximate* room proportions and a chosen 53° working door opening; it is **not a measured 3D scan**.
- S01 camera geometry was previously accepted by the project operator, but son/phone character layout and final video storyboard need separate QC.
- This public repository intentionally **does not** contain the private production repository.
