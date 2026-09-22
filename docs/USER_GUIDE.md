# Meta Vibes Studio — Complete User Guide

> A step-by-step explanation of the extension’s current features and controls.

[Documentation Home](README.md) · [Prompt Writing Guide](PROMPT_WRITING_GUIDE.md) · [Prompt Library](PROMPT_LIBRARY.md)

---

## Contents

1. [Before you start](#1-before-you-start)
2. [The workspace](#2-the-workspace)
3. [Recommended workflow](#3-recommended-workflow)
4. [Troubleshooting](#4-troubleshooting)
5. [Project file structure](#5-project-file-structure)
6. [Operational checklist](#6-operational-checklist)

Meta Vibes Studio is a browser extension for organizing projects, preparing scene prompts, managing character and location references, generating images on Meta AI, and generating videos on Vibes.ai.

## 1. Before you start

1. Open Chrome or Edge.
2. Open `chrome://extensions` (or `edge://extensions`).
3. Enable **Developer mode**.
4. Choose **Load unpacked** and select the project folder.
5. Pin **Meta Vibes Studio** to the browser toolbar.
6. Keep either `meta.ai` or `vibes.ai` open. The extension reports which supported site is active.

The extension stores project state, preferences, statistics, and diagnostics locally in the browser. It does not require an account.

## 2. The workspace

### Project area

Create a project and give it a recognizable name. A project keeps prompts, references, and video tasks together. Use **Choose project** to reopen a saved project folder.

### Scenes tab

Paste one scene prompt per block. Separate blocks with two or more blank lines, then select **Split prompts**. Review the generated scene cards before starting the queue.

To link saved references, add `character | Name` or `location | Name` on separate lines inside the scene block. The name must match a saved reference.

### References tab

Create characters and locations from structured text or add them manually. Give every reference a stable name and a detailed description. Link references to the scenes that use them. Generate reference images on Meta AI when visual identity must remain consistent.

The structured importer requires `character | Name | Description` or `location | Name | Description`, with one reference per line.

### Videos tab

Choose **Image to video** when a scene image is the starting frame. Choose **Text to video** when motion should be generated from the written description. For image-to-video, select a start frame and optionally an end frame.

For scene-number linking, place `START | 1` and optionally `END | 2` above the motion prompt. For a local frame, choose the upload option from the start or end selector on that video card. Text-to-video prompts do not use frame tags.

### Queue controls

The scene queue runs in order: it uploads linked references, sends the prompt, waits for the result, and continues. The video queue follows the same controlled workflow on Vibes.ai. Reset statuses only when you intentionally want to retry work.

### Save and export

Choose a local project folder when prompted. Export scenes, references, videos, or the full project. Keep the folder structure intact so the project can be reopened later.

### Settings

Settings controls the save location, language, appearance, generation statistics, and diagnostics export. Diagnostics are local and older entries are automatically removed after seven days.

## 3. Recommended workflow

1. Create the project and choose its image format.
2. Write or import scene prompts.
3. Extract the characters and locations needed by those scenes.
4. Generate and review reference images first.
5. Generate scene images on Meta AI.
6. Move to Vibes.ai and create videos from approved scenes.
7. Review results, then export the full project.

## 4. Troubleshooting

- **Unsupported page:** open Meta AI or Vibes.ai and retry.
- **No editor found:** wait for the site to finish loading, then retry.
- **Missing reference:** add a description or generate/upload its image first.
- **Queue blocked:** inspect failed cards, correct the prompt or frame, then retry.
- **No files to save:** complete at least one generation before exporting.
- **Old data appears:** choose the project again from its folder; the extension intentionally starts sessions with a clean in-memory workspace.

## 5. Project file structure

When you save a complete project, keep this structure intact:

```text
project-name/
├── prompts/
│   ├── scene-prompts.txt
│   ├── reference-prompts.txt
│   └── video-prompts.txt
├── images/
│   ├── references/
│   └── scenes/
├── videos/
└── settings/
    └── project-settings.json
```

Do not rename numbered scene and video files unless you also update the corresponding prompts. Stable names help the extension match media when a project is reopened.

## 6. Operational checklist

### Before generation

- [ ] The correct supported website is open.
- [ ] The connection indicator is active.
- [ ] The correct project is open.
- [ ] Every scene prompt describes one clear shot.
- [ ] Required references have descriptions or images.

### Before video generation

- [ ] Vibes.ai is open on a project page.
- [ ] Image-to-video or text-to-video mode is correct.
- [ ] Every video has a valid prompt.
- [ ] A start image is selected or uploaded for image-to-video.
- [ ] The optional end image matches the intended final composition.

### Before export

- [ ] Failed items have been reviewed.
- [ ] The preferred result is selected when multiple outputs exist.
- [ ] The save location is correct.
- [ ] The full project export includes prompts, images, and videos.

---

[Back to Documentation Home](README.md)
