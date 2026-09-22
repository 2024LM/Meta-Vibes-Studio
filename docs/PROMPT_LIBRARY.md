# Prompt Library

> Optional templates for scene images, references, transitions, and videos. Use only the details relevant to your request.

[Documentation Home](README.md) · [User Guide](USER_GUIDE.md) · [Prompt Writing Guide](PROMPT_WRITING_GUIDE.md)

---

## How to use this library

1. Copy the closest template.
2. Replace every `[BRACKETED VALUE]`.
3. Remove instructions that do not apply.
4. Add project-specific continuity details.
5. Review the prompt with the scorecard in the [Prompt Writing Guide](PROMPT_WRITING_GUIDE.md).

These prompts are ready to paste into Meta Vibes Studio. Replace bracketed values before use.

## 1. Scene generation — character and action

```text
Create an image of [CHARACTER] performing [ACTION] in [LOCATION] at [TIME OF DAY]. The character is positioned at [POSITION] and carries or interacts with [PROP]. Show the important parts of the location: [LOCATION DETAILS]. Preserve the character’s exact face, hairstyle, clothing, body proportions, and the location’s layout. Use [OPTIONAL STYLE] only if required. Avoid text, logos, watermarks, extra people, duplicate props, face changes, distorted hands, and unwanted changes to the location.
```

## 2. Scene generation — establishing location

```text
Create a clear overview of [LOCATION] immediately before [EVENT]. Show its entrances, paths, important landmarks, layout, and weather conditions. Place [CHARACTER] at [POSITION] if required. Maintain the same architecture, object placement, and colors for later scenes. Avoid text, unreadable signs, logos, extra structures, and elements that were not requested.
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
Generate a [DURATION]-second video of [SUBJECT] performing [ACTION] in [LOCATION]. The video begins with [START STATE] and ends with [END STATE]. Optional movement or viewpoint: [MOVEMENT]. Preserve facial identity, clothing, object shapes, and the location. Keep motion continuous and understandable. Avoid unwanted cuts, time jumps, extra characters, face changes, duplicate objects, flicker, logos, and watermarks.
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
Create a clear reference image for [OBJECT NAME]. Show the object centered and include the views needed to understand its shape. Define its dimensions, silhouette, materials, surface condition, colors, functional parts, and distinctive markings: [DETAILS]. Use a plain background. Preserve this design, scale, materials, and color placement in later scenes. Avoid hands, people, decorative additions, text, logos, and alternate versions.
```

## 10. Dialogue-free emotional close-up

```text
Create a close view of [CHARACTER] reacting to [EVENT] without speaking. The emotion changes from [INITIAL EMOTION] to [FINAL EMOTION] through natural facial movement and breathing. Preserve the exact identity, hairstyle, clothing, and background from the previous scene. Avoid exaggerated expressions, tears unless specified, face changes, beauty retouching, text, and extra people.
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
