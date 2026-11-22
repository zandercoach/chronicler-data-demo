# IMAGE-STYLE.md — Chronicler demo

Claude writes the briefs, never the images; Christian or Morten generates an image from its brief.

This file supplements the core `C:\claude\IMAGE-STYLE.md`, the „zander.coach flipchart style"; what it does not say is governed from there. The demo is the engine's shop window for the readers of Adaptive × AI, so it speaks as Christian and the core applies. **What the demo adds and why:**

| | Demo | Reason |
|---|---|---|
| Subjects | Heroes, non-player characters, creatures, places and adventure covers of an invented fantasy chronicle | The chronicle is fiction; its pictures show the story, not a training point |
| Figures | People are the core's flipchart figures, told apart by gear and clothing (a cloak, a hammer, a purse); creatures and places are simple marker shapes | Recognisable at thumbnail size without leaving the core's figure |
| Mood | Mist and night as flat fields of the deep tones, inviting rather than grim | The Nebelmoor is dark; the core's light, warm mood is kept through the motif, not given up |
| Lettering | None | Titles and names are HTML next to the picture |
| Format | Square for heroes, non-player characters and creatures; portrait 2:3 for adventure covers; landscape 3:2 for places | The page layouts the engine already uses |

## The medium block

Edit here, then run `python material/tooling/sync-image-style.py`.

<!-- medium-block:start -->
Illustrations for an invented fantasy chronicle. People are the same flipchart figures, told apart only by their gear and clothing — a cloak, a hammer, a purse, a hood — never by realistic faces, armour detail or weapons drawn to threaten. Creatures and places are simple marker shapes. Mist, water and night are flat fields of deep sea, deep petrol and pale petrol, never gradients; the mood stays inviting and curious rather than grim. One subject per image, centred, with plenty of white space around it. No words, letters, numbers or digits anywhere in the image.
<!-- medium-block:end -->

## The style block, to be copied verbatim

Generated from the core block and the medium block; never edited here.

<!-- style-block:start -->
Hand-drawn flipchart illustration, as sketched live by a trainer with markers: clean near-black marker outlines on a plain white background, simple friendly shapes. Human figures are always drawn with a body — a round head, an oval torso, and single-line arms and legs attached to that torso, each ending in a small round hand or foot, never a head with limbs hanging directly off it — and the posture carries the expression. Each figure is about five heads tall: a large round head, a tall narrow oval torso about one and a half heads long, long straight legs. Faces are two dot eyes and a small curved smile, no nose, the head often turned slightly to one side; hair is a few loose marker strokes that tell the figures apart. Torsos are filled flat or left white. One even line weight throughout, like a medium marker at about half a percent of the image width, never thicker for emphasis. Colours only from this palette, applied as wide, slightly uneven marker strokes and flat fills. Petrol (#008888) is the eye-catcher: used sparingly, on the one or two things the eye should land on first. Supporting accents: deep petrol (#005F5F), deep sea (#06393A), pale petrol (#C7DBD8) and sand (#A98B5B), the only warm colour. Quiet neutrals for secondary shapes: soft ink (#354544), muted grey-green (#556564), light surface (#F1F5F4) and pale line grey (#DCE5E3). Outlines and lettering in ink (#0F1A1A); no pure black, no other colours. No hatching, no cross-hatching, no paper texture, no grain, no gradients, no shading, no photorealism. Few details and plenty of white space. Light, warm, optimistic mood. Illustrations for an invented fantasy chronicle. People are the same flipchart figures, told apart only by their gear and clothing — a cloak, a hammer, a purse, a hood — never by realistic faces, armour detail or weapons drawn to threaten. Creatures and places are simple marker shapes. Mist, water and night are flat fields of deep sea, deep petrol and pale petrol, never gradients; the mood stays inviting and curious rather than grim. One subject per image, centred, with plenty of white space around it. No words, letters, numbers or digits anywhere in the image.
<!-- style-block:end -->

## The brief

One file per image in `briefs/<type>/<file name>-imageprompt.txt`; the image goes to `img/<type>/<file name>.jpg`. The briefs stay outside `img/`, because the whole of `img/` is published. The file name is the entry's name as the engine looks it up: lower case, spaces as `_`, umlauts kept (`jörn_eisenfaust`); a type's placeholder is `default.jpg`.

Images are generated as PNG and stored as JPEG, at most 1000 px on the long side, quality 85 — about 30–90 KB instead of over 1 MB. The pages show them far smaller; the engine finds `.png` and `.jpg` alike.

```
IMAGE STYLE GUIDE ("zander.coach flipchart style", Chronicler demo variant)
==========================================================================
<the block above, verbatim>

IMAGE BRIEF ("<entry name>", <type>) — GOAL, NOT A CHECKLIST
============================================================
WHO OR WHAT IT IS
<two to four sentences from the chronicle: who this is, what they did>

WHAT THE PICTURE SHOULD DO
<what the reader should recognise at thumbnail size; what it must not suggest>

THE MOTIF DIRECTION
<the pose or scene; the one or two things in petrol; what to steer away from>

WHAT IS FIXED
The style guide above. <format>, white background. No words, letters or digits anywhere. Deliver as PNG.

WHAT IS YOURS
The staging, the pose, the details within the style.
```

## History

- **2026-11-22.** Set up with the first eighteen briefs: the demo's three heroes, two non-player characters, two creatures, four places, two adventure covers and a placeholder per type. Direction A of two (Christian): the core's flipchart hand, not a classic ink-and-watercolour RPG illustration, because the demo speaks as Christian.
- **2026-11-22.** All eighteen images drawn. Three regenerated after review, their briefs sharpened: the Nebelmoor cover showed Mirela hooded, which reads as Ylva; on the tithe cover figures floated without ground; the place placeholder's milestone read as a door. Lesson for covers: name each figure's look as in their portrait. Stored as JPEG, 1000 px.
