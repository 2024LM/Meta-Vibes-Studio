# Professional Prompt Writing Guide

> A practical system for writing controllable, consistent prompts for still images, references, and motion.

[Documentation Home](README.md) · [User Guide](USER_GUIDE.md) · [Prompt Library](PROMPT_LIBRARY.md)

---

## Contents

- [The prompt formula](#the-prompt-formula)
- [Scene prompt template](#scene-prompt-template)
- [Reference prompt template](#reference-prompt-template)
- [Video prompt template](#video-prompt-template)
- [Expert rules](#expert-rules)
- [Prompt review scorecard](#prompt-review-scorecard)

Write prompts as production instructions, not as vague ideas. The generator performs best when the subject, action, environment, camera, lighting, style, continuity, and exclusions are explicit.

## The prompt formula

```text
Subject + action + environment + composition + camera + lighting + style + continuity + constraints
```

## Scene prompt template

```text
Create a [shot size] scene of [character or subject] [specific action] in [location and time].
Composition: [foreground, middle ground, background, subject placement].
Camera: [lens feel, angle, height, movement or locked-off].
Lighting: [source, direction, color, contrast, mood].
Style: [realistic, cinematic, editorial, illustrated, etc.].
Continuity: preserve [identity, clothing, props, geography, color palette].
Avoid: text, logos, watermarks, extra people, duplicated objects, distorted hands, face changes.
```

## Reference prompt template

```text
Create a clean reference image for [character/location name].
Identity: [age range, face, hair, skin tone, build, defining features].
Wardrobe or architecture: [specific details].
Pose and framing: neutral, centered, full or three-quarter view, clear silhouette.
Background: simple and unobtrusive.
Style: consistent with the project’s visual language.
Preserve this identity in every later scene. Avoid text, logos, dramatic angles, and unrelated props.
```

## Video prompt template

```text
Animate the supplied opening frame into a [duration]-second [aspect ratio] shot.
Action: [one continuous physical action with a clear beginning and end].
Camera: [camera movement and speed].
Subject continuity: preserve faces, clothing, proportions, props, and location.
Motion: natural weight, believable timing, stable geometry, realistic light and shadows.
Ending: finish on [the supplied end frame or exact final composition].
Avoid: cuts, morphing, new characters, duplicated limbs, flicker, text, logos, and camera jumps.
```

## Expert rules

- Describe one primary action per shot.
- Use concrete nouns and measurable spatial relationships.
- Specify what must remain unchanged when using a reference image.
- Use an end frame when the final composition matters.
- Keep the camera direction and lighting consistent across adjacent scenes.
- Put negative constraints at the end; do not write contradictory instructions.
- Treat each scene as a shot in a sequence, not as a complete story.

## Prompt review scorecard

Score each category from 0 to 2 before generation. A production-ready prompt should score at least 12/14.

| Category | 0 | 1 | 2 |
| --- | --- | --- | --- |
| Subject | Missing | General | Specific and identifiable |
| Action | Missing | Multiple/unclear | One clear action |
| Environment | Missing | Generic | Concrete and spatially clear |
| Composition | Missing | Implied | Shot size and placement defined |
| Lighting | Missing | Mood only | Source, direction, and mood defined |
| Continuity | Missing | Partial | Identities, props, and geography locked |
| Constraints | Missing | Generic | Relevant failure modes excluded |

## Common weak prompts and stronger revisions

| Weak instruction | Why it fails | Stronger direction |
| --- | --- | --- |
| “Make it cinematic.” | No visual decision is defined. | Specify shot size, lens feel, lighting direction, and camera movement. |
| “The person walks dramatically.” | Identity, path, and ending are unclear. | Name the character, movement path, pace, emotion, and final position. |
| “Keep everything the same.” | The model does not know which details matter. | List the exact face, wardrobe, props, architecture, and light direction to preserve. |
| “No mistakes.” | It gives no actionable constraint. | Exclude duplicate limbs, face morphing, flicker, text, logos, and geometry changes. |

---

[Back to Documentation Home](README.md)
