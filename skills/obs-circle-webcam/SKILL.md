---
name: obs-circle-webcam
description: "Set up or repair an OBS scene with a screen capture and circular webcam, verifying the composed preview."
---

# Obs circle webcam

Needs: OBS, an available webcam and supported desktop controls.

## Inspect and preserve the scene

Use the current Sources list and preview. Prefer existing sources and filters; keep recording stopped unless explicitly requested. A filter preview alone is not proof of the composed scene.

- Valid: verify the circle in the main scene preview.
- Invalid: call the scene fixed from a filter dialog only.

## Repair the correct failure

If the selected camera is nominally active but black, deactivate and reactivate it before rebuilding. If the feed is live but stretched, reset its transform before adjusting filters. Report observed causes without blaming another app without evidence.

- Valid: reacquire the camera and inspect its direct preview.
- Invalid: rebuild masks while the camera feed itself is black.

## Verify final geometry

Apply a circular mask, resize without distortion and place with a margin in the composed scene. Stop at a user-only device or security prompt. Capture readiness does not prove the recorded output.

- Valid: verify the composed scene and leave recording stopped.
- Invalid: claim an exported recording verified from a live preview.
