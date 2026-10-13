---
name: video-recolor
description: "Recolor a selected moving object with a tracked continuous mask while preserving shading and excluding neighboring regions."
---

# Video recolor

Needs: Source video, tracking or mask tools and a video renderer.

## Trace and track the real boundary

Inspect the unmodified source across time, including occlusion and large movement. Trace the whole target; protect skin, edges and neighboring objects. Track from original frames, adding anchors after cuts or drift.

- Valid: retrace a collar boundary that spills onto skin.
- Invalid: smooth a wrongly traced contour until it looks plausible.

## Grade continuously and preserve detail

Use a continuous mask rather than per-pixel brightness thresholds. Feather on the target side where spill matters. Darkening multiplication reduces detail contrast; retain appropriate source texture rather than inventing grain.

- Valid: adjust shade while comparing source texture and protected pixels.
- Invalid: select fabric by changing RGB thresholds that create crawling holes.

## Verify over time

Inspect a playable close-up and contour overlays across the clip, decode outputs, compare outside-mask pixels before encoding and preserve the intended audio. Lossy encoding does not support a byte-identical claim.

- Valid: inspect moving edges and compare unchanged audio.
- Invalid: prove a moving mask from one good still frame.
