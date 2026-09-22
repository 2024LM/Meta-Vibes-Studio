# Prompt Library

> Examples written in the formats currently accepted by Meta Vibes Studio.

[Documentation Home](README.md) · [User Guide](USER_GUIDE.md) · [Prompt Writing Guide](PROMPT_WRITING_GUIDE.md)

---

## Important

These are editable examples, not automatic commands. Replace names and descriptions before use. Keep pipe separators (`|`) and blank-line spacing where shown.

## 1. Reference definitions

Paste into **References**, edit the values, then select **Create and save references**.

```text
character | Lina | Adult woman, short black hair, blue jacket, dark trousers, brown shoulder bag
character | Omar | Older man, grey hair, round glasses, beige shirt, dark green apron
location | Repair shop | Narrow workshop, green entrance door, wooden workbench, metal shelves
location | Courtyard | Small stone courtyard, old fountain, climbing plants on the walls
```

## 2. Scene prompts without references

Each block becomes one scene. Keep two empty lines between blocks.

```text
An old camera rests on a wooden workbench beside a screwdriver and folded cloth.


A hand opens the camera battery compartment and removes the damaged battery.
```

## 3. Scene prompts with linked references

Reference names must match saved references.

```text
character | Lina
location | Repair shop
Lina enters the repair shop and places an old camera on the wooden workbench.


character | Lina
character | Omar
location | Repair shop
Omar examines the camera while Lina waits beside the workbench. Preserve their faces, clothing, and the workshop layout.
```

## 4. Image-to-video with start and end scenes

```text
START | 1
END | 2
Lina walks from the entrance to the workbench and places the camera in front of Omar.
```

## 5. Image-to-video with only a start scene

```text
START | 2
Omar lifts the camera, turns it carefully, and examines the battery compartment.
```

## 6. Multiple image-to-video prompts

Keep two empty lines between blocks.

```text
START | 1
END | 2
Lina crosses the workshop and places the camera on the workbench.


START | 2
END | 3
Omar opens the battery compartment while Lina watches from the other side of the table.
```

## 7. Image-to-video with local images

```text
The subject moves from the opening position to the final position with continuous natural motion. Preserve identity, clothing, objects, and background.
```

After selecting **Add videos**, choose **Upload start image from computer** from the start-frame selector. Optionally choose **Upload end image from computer** from the end-frame selector. The files are attached to that video card.

## 8. Text-to-video prompts

Select **Text to video**. Do not use `START` or `END`.

```text
A paper airplane crosses an empty classroom, circles above the desks, and lands beside an open notebook.


Rainwater flows along a quiet street and gathers around the wheels of a parked bicycle.
```

## 9. Validation checklist

- [ ] References use `type | name | description`.
- [ ] Scene reference links use existing names.
- [ ] Blocks are separated by two or more empty lines.
- [ ] Image-to-video has a start scene or uploaded start image.
- [ ] `END` is not used without `START` when scene numbers are used.
- [ ] Text-to-video contains no frame tags.
- [ ] Local images are selected on the correct video card.

---

[Back to Documentation Home](README.md)
