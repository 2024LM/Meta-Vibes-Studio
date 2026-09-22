# Prompt Writing Guide

> This guide describes the text formats that Meta Vibes Studio currently reads and how the extension uses them.

[Documentation Home](README.md) · [User Guide](USER_GUIDE.md) · [Prompt Library](PROMPT_LIBRARY.md)

---

## 1. Scene prompts

Enter scene prompts in **Scenes**. Separate scenes with two or more empty lines, then select **Split prompts**.

```text
A person opens the workshop door and looks inside.


The person walks to the table and examines the old camera.
```

The extension creates one numbered card for each block. Subject, action, location, important objects, and continuity details are usually enough. Camera, lighting, and style wording is optional text passed to the generation website; it is not an extension setting.

## 2. Reference definitions

The **References** importer reads one reference per line using pipe characters (`|`).

```text
character | Character name | Character description
location | Location name | Location description
```

Accepted types are `character`, `characters`, `location`, `locations`, `place`, and `places`.

```text
character | Lina | Adult woman, short black hair, blue jacket, brown shoulder bag
location | Repair shop | Narrow room, wooden workbench, metal shelves, green entrance door
```

Select **Create and save references** after entering the lines. Lines without a recognized type, name, and description are ignored.

## 3. Linking references to scenes

Add reference-link lines inside a scene block:

```text
character | Lina
location | Repair shop
Lina enters the repair shop and places the old camera on the workbench.
```

The name must match an existing reference. The extension removes recognized link lines from the generated prompt and links the matching references to that scene.

## 4. Image-to-video prompts

Choose **Image to video**. Reference generated scene numbers with `START` and `END` lines:

```text
START | 1
END | 2
The person walks from the doorway to the table while the camera remains stable.
```

- `START | number` selects the opening scene image.
- `END | number` selects the optional ending scene image.
- `START` without `END` creates a start-frame-only task.
- `END` without `START` is invalid and the end frame is removed.
- `STAR` is accepted for compatibility, but `START` is the documented form.

The frame selectors on each video card can replace scene images with local images. A local image is attached to that specific video and uploaded to Vibes.ai during generation.

## 5. Text-to-video prompts

Choose **Text to video** and do not add `START` or `END` lines.

```text
A paper airplane crosses an empty classroom, circles above the desks, and lands beside an open notebook.
```

Separate multiple video prompts with two or more empty lines.

## 6. What the extension does not control

The current project interface does not set image orientation, image resolution, video resolution or quality, video duration, aspect ratio, camera, lighting, or visual style. These may be written as optional prompt instructions if the generation website supports them, but the extension does not enforce them.

---

[Back to Documentation Home](README.md)
