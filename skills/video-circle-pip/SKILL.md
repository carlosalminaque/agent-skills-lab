---
name: video-circle-pip
description: "Remove baked black backing from an existing circular webcam video and composite it without losing narration or circle geometry."
---

# Video circle pip

Needs: FFmpeg, ffprobe and accessible source video files.

## Preserve the existing circle

Probe dimensions, duration, frame rate and audio. Inspect backing pixels. Direct compositing is acceptable when verified matching black hides the backing cleanly; otherwise use a low-tolerance black color key that preserves hair and dark clothing.

- Valid: test dark clothing while removing only backing.
- Invalid: redraw or recrop the circle to solve the backing.

## Prove alpha and timing

Use an alpha-capable intermediate and test it over a bright background. Preserve the chosen narration track; do not mix both tracks by default. Use the shorter effective duration and overlay shortest=1 without loops, freezes or padding.

- Valid: inspect a bright-background composite and the measured ending.
- Invalid: trust an alpha filename or loop the short input.

## Verify the final export

Check representative frames, full decoding, intended audio stream, duration, circle size and placement. A player showing black is not evidence that alpha was lost; use the composite test.

- Valid: report verified alpha, one narration stream and duration.
- Invalid: claim the full video verified from an alpha intermediate.
