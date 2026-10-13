# Agent skills lab

10 self-contained public skills for agents that read `SKILL.md`. Each skill states its prerequisites and includes Valid/Invalid examples.

## Install

```bash
npx skills add carlosalminaque/agent-skills-lab
```

Installation grants no external service permissions. Choose one skill or the whole collection.

## Skills

| Skill | What it does | Needs |
|---|---|---|
| [cheaper-worker-delegation](skills/cheaper-worker-delegation/SKILL.md) | Delegate bounded mechanical work to verified lower-cost callable models while keeping judgment and integration with the lead agent. | Agent delegation tools and current model availability or cost information. |
| [codex-browser-recovery](skills/codex-browser-recovery/SKILL.md) | Recover an uncontrollable visible Codex browser by discovering the supported runtime and exact backend, then resume the original task. | Codex browser control runtime and the intended browser tab. |
| [instagram-profile-analysis](skills/instagram-profile-analysis/SKILL.md) | Analyze a public Instagram profile from its accessible bio, posts, reels, captions, and highlights when the user asks what the person is like, does, knows, or projects online. Separate direct evidence from inference and do not turn aesthetics into unsupported claims. | browser control |
| [instagram-reel-thumbnail-maker](skills/instagram-reel-thumbnail-maker/SKILL.md) | Create accurate, readable Instagram Reel cover images after reviewing the actual videos. Use for title-based covers, cover redesigns, or consistent thumbnail sets; do not infer a reel's subject from its grid image or caption alone. | video access |
| [obs-circle-webcam](skills/obs-circle-webcam/SKILL.md) | Set up or repair an OBS scene with a screen capture and circular webcam, verifying the composed preview. | OBS, an available webcam and supported desktop controls. |
| [stay-within-usage-limits](skills/stay-within-usage-limits/SKILL.md) | Manage long agent work using actual visible usage telemetry, bounded waves and a verified resume checkpoint. | Host usage telemetry; if unavailable, report that limitation. |
| [transhumanist-race-diagram](skills/transhumanist-race-diagram/SKILL.md) | Visualize AI capability and human enhancement trends with explicit concepts, stable entity colors and honest evidence provenance. | Diagram or chart tools and sources for factual claims. |
| [video-circle-pip](skills/video-circle-pip/SKILL.md) | Remove baked black backing from an existing circular webcam video and composite it without losing narration or circle geometry. | FFmpeg, ffprobe and accessible source video files. |
| [video-recolor](skills/video-recolor/SKILL.md) | Recolor a selected moving object with a tracked continuous mask while preserving shading and excluding neighboring regions. | Source video, tracking or mask tools and a video renderer. |
| [video-skill-mining](skills/video-skill-mining/SKILL.md) | Extract reusable tools and techniques from complete video sources into one prioritized list matched to the user’s actual setup. | Video access, complete transcripts and accessible source links. |

## Checks

```bash
python scripts/scrub-check.py
python scripts/skill-lint.py
```

Checks cover the explicit public scope in `publish-scope.json`. Passing checks does not prove runtime behavior or publication.
