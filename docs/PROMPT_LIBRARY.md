# Production Prompt Library

> Copy-ready building blocks for consistent scene images, references, transitions, and videos.

[Documentation Home](README.md) · [User Guide](USER_GUIDE.md) · [Prompt Writing Guide](PROMPT_WRITING_GUIDE.md)

---

## How to use this library

1. Copy the closest template.
2. Replace every `[BRACKETED VALUE]`.
3. Remove instructions that do not apply.
4. Add project-specific continuity details.
5. Review the prompt with the scorecard in the [Prompt Writing Guide](PROMPT_WRITING_GUIDE.md).

These prompts are ready to paste into Meta Vibes Studio. Replace bracketed values before use.

## 1. Scene generation — cinematic character shot

```text
Create a cinematic medium-wide shot of [CHARACTER] walking through [LOCATION] at [TIME OF DAY]. The character moves from the left foreground toward the center while carrying [PROP]. Show a clear foreground, a readable middle ground, and the defining architecture of the location in the background. Use a natural eye-level camera with a gentle forward dolly. Warm directional light from the [DIRECTION] creates soft shadows and a calm [MOOD] atmosphere. Preserve the character’s exact face, hairstyle, clothing, body proportions, and the location’s geography. Photorealistic cinematic style, subtle film texture, natural colors. Avoid text, logos, watermarks, extra people, duplicate props, face changes, distorted hands, and impossible architecture.
```

## 2. Scene generation — establishing location

```text
Create a wide establishing shot of [LOCATION] immediately before [EVENT]. The environment is the main subject: show its scale, entrances, paths, important landmarks, and the weather conditions. Place [CHARACTER] small but clearly readable at [POSITION] to establish geography. Use a locked-off 24mm cinematic composition with balanced layers and realistic depth. Lighting is [LIGHTING DESCRIPTION], creating a [MOOD] tone. Maintain consistent architecture and color palette for later shots. Avoid text, signage that cannot be read, logos, extra structures, and fantasy elements unless specified.
```

## 3. Reference generation — character identity sheet

```text
Create a clean character reference image for [NAME], a [AGE]-year-old [ROLE]. Show a centered three-quarter portrait and a full-body view in one coherent neutral presentation. Identity details: [FACE], [HAIR], [SKIN TONE], [BUILD], and [DISTINGUISHING FEATURE]. Wardrobe: [CLOTHING AND COLORS]. Use soft even studio lighting, a simple neutral background, and a clear silhouette. This is a continuity reference: preserve the exact face, hair, proportions, clothing colors, and defining feature in every future scene. Avoid text, logos, dramatic perspective, heavy shadows, accessories not listed, and alternate identities.
```

## 4. Reference generation — location reference

```text
Create a detailed location reference for [LOCATION NAME]. Show the exact layout, major architectural forms, entrance and exit points, ground materials, color palette, and distinctive objects: [LIST DISTINCTIVE ELEMENTS]. Use a neutral wide architectural view with straight believable geometry and soft daylight. The location must remain recognizable from multiple camera angles in later scenes. Preserve scale, geography, materials, and landmark placement. Avoid people, text, logos, invented buildings, and changes to the described architecture.
```

## 5. Video generation — image to video

```text
Animate the supplied opening image into a smooth [DURATION]-second [ASPECT RATIO] shot. [CHARACTER OR SUBJECT] performs one continuous action: [ACTION]. Begin exactly from the supplied frame, then use a slow [CAMERA MOVE] while maintaining the original composition and subject identity. Preserve the exact face, clothing, body proportions, props, architecture, lighting direction, and color palette. Motion should have natural weight and believable timing. End on the supplied final frame with a stable composition. Avoid cuts, morphing, new objects, duplicated limbs, flicker, camera jumps, text, logos, and watermarks.
```

## 6. Video generation — text to video

```text
Generate a [DURATION]-second cinematic [SHOT TYPE] of [SUBJECT] [ACTION] in [LOCATION]. The shot begins with [START STATE] and ends with [END STATE]. Camera: [ANGLE AND MOVEMENT]. Lighting: [LIGHTING]. Mood: [MOOD]. Use realistic physics, coherent facial identity, stable clothing, consistent object geometry, and smooth continuous motion. The scene must be visually clear without dialogue or text. Avoid cuts, time jumps, extra characters, face morphing, duplicate objects, flicker, logos, and watermarks.
```

## 7. Continuity prompt for a sequence

```text
This shot continues directly from the previous scene. Preserve [CHARACTER IDENTITIES], [WARDROBE], [PROPS], [LOCATION GEOGRAPHY], [TIME OF DAY], and [LIGHTING DIRECTION]. Start from [PREVIOUS END STATE], perform [NEXT ACTION], and finish at [NEXT END STATE]. Use the same lens feel, camera height, color palette, and visual style. Do not introduce new people, objects, architecture, wardrobe changes, or unexplained lighting changes.
```

## 8. Quality-control instruction

```text
Before finalizing, check: identity consistency, correct number of people, correct props, readable geography, natural anatomy, stable lighting, coherent camera movement, and a clean final frame. If any element conflicts with the reference, prioritize the reference and continuity instructions. No text, logos, watermarks, glitches, flicker, or accidental duplicates.
```

## 9. Product or object reference

```text
Create a clean production reference for [OBJECT NAME]. Show the object centered from a three-quarter angle with one smaller side or rear view. Define its exact dimensions, silhouette, materials, surface wear, colors, functional parts, and distinctive markings: [DETAILS]. Use neutral studio lighting and a plain background. Preserve this exact design, scale, materials, and color placement in every later scene. Avoid hands, people, decorative additions, text, logos, alternate versions, and dramatic perspective.
```

## 10. Dialogue-free emotional close-up

```text
Create a cinematic close-up of [CHARACTER] reacting to [EVENT] without speaking. The emotion develops from [INITIAL EMOTION] to [FINAL EMOTION] through subtle eye movement, breathing, and facial tension. Camera is stable at eye level with a natural portrait lens feel. [LIGHT SOURCE] shapes the face while preserving skin texture and exact identity. Keep hairstyle, wardrobe, background, and light direction consistent with the previous shot. Avoid exaggerated expressions, tears unless specified, face morphing, beauty retouching, text, and extra people.
```

## 11. Controlled transition between frames

```text
Create a continuous transition from the supplied opening frame to the supplied ending frame. Begin with [START ACTION], move through [MIDDLE BEAT], and arrive naturally at [END COMPOSITION]. Use one smooth [CAMERA MOVEMENT] with no cuts. Preserve all identities, wardrobe, props, architecture, weather, and lighting direction. Motion must remain physically believable and the final second must settle into the supplied ending frame. Avoid teleportation, dissolves, body morphing, duplicated objects, flicker, sudden camera acceleration, text, logos, and watermarks.
```

## 12. Prompt customization checklist

- [ ] Every bracket has been replaced.
- [ ] The aspect ratio matches the project.
- [ ] Character and location names match saved references.
- [ ] Camera movement supports the action.
- [ ] The final composition is explicitly described.
- [ ] Continuity details match adjacent shots.
- [ ] Negative constraints address likely failures.

---

[Back to Documentation Home](README.md)
