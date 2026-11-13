# Classroom Arena — Gemini Design Script v4: the "Clarity" pass

**Goal:** make the site calmer, more beautiful and quicker to understand, using **4 Gemini generations** (5 if you want the front-page hero).
**Workflow:** use **one Gemini chat**. Download the images and upload them all to Claude in **one message**. Claude cuts the sheets apart, removes the white backgrounds, compresses everything and builds it into both sites.

---

## What the research says (and how this script uses it)

| Finding | What it means for our art |
|---|---|
| Working memory holds about **4 chunks** at a time. Clutter, too many choices and unclear labels all use it up. | Fewer, bigger, clearer pictures. No busy backgrounds. Every picture does one job. |
| Distracting or unnecessary design elements add mental effort without helping anyone learn ("extraneous load"). | **No decoration for its own sake.** Art only goes where it explains something: mode tiles, study steps, empty screens, celebrations. |
| Icons are easiest to understand **with a text label beside them**. | The app writes every label. Gemini never draws text. |
| Duolingo keeps a style recognizable by using the **fewest shapes possible** (about 15 per character), **rounded edges only** and a **flat, front-facing perspective**. | Built into the style rules below. |
| Empty screens should explain what the space is for, why it's empty and what to do next: a short message, a simple picture and an action button. | Image 3 makes four "moment" illustrations for exactly those screens. |
| Consistency means people learn something once and can use it everywhere. | One style setup at the start, used for every image in the same chat. |

---

## Step 0: Set the style once

**Before you paste this,** attach one image Gemini made for you last time, such as the old icon sheet, so the new art matches. Attaching an image doesn't use a generation.

```
You are the illustrator for "Classroom Arena," a professional U.S. History learning platform sold to schools. The attached image shows our current style — match it. Rules for EVERY image in this chat:

STYLE
- Flat vector illustration, front-facing flat perspective, very subtle soft gradients, no outlines.
- Use the FEWEST shapes possible: about 12–18 shapes per object. Simple beats detailed.
- Every corner is rounded. No sharp points, no spikes, no jagged edges.
- One soft light source from the top-left on every object, so a whole set looks lit the same way.
- Friendly but official: premium edtech for teenagers and teachers — not babyish, not clip art, not 3D renders, not photo-real.

COLOR (use only these)
- Royal blue #1D4ED8 (main), navy #0B1F4B (darks), sky blue #38BDF8 (lights), white #FFFFFF
- Small accents only: amber #F59E0B, emerald #059669, soft coral #F87171
- Skin tones vary naturally; no other colors.

LAYOUT
- Pure solid white background unless I say otherwise, with nothing touching the edges.
- No ground shadows, no floor, no scenery behind objects unless I ask.
- Absolutely NO text, letters, numbers, logos, flags with text, or watermarks.
- No real people's likenesses.

Reply "Ready" and wait.
```

---

## Image 1: Mode icon sheet (8 icons)

These replace the emoji on the student mode buttons and the Present screen, which is the biggest polish upgrade on the site.

```
Image 1: a sheet of 8 app icons arranged in a 4-by-2 grid with wide, even white gaps between them. Every icon sits inside the same size rounded-square tile filled with a very light blue (#EFF4FF). Same scale, same lighting, same style. In order, left to right, top row then bottom row:
1) an open book with a small glowing lightbulb rising from the pages (Study Lab)
2) a compass with a royal-blue needle (Mastery Gauntlet)
3) a gold picture frame holding a tiny parchment document (Gallery Walk)
4) a rounded mountain with a small amber flag on the peak (Summit)
5) a game controller with royal-blue buttons (Arcade)
6) a 3-by-3 grid of royal-blue game-show tiles, one tile glowing amber (Category Clash)
7) a classroom smartboard with a speech bubble beside it (Live Question)
8) a picture frame with three small circles below it, like viewers watching together (Live Gallery Walk)
Landscape 2:1. Icons must not touch each other.
```

## Image 2: Study Lab steps + progress badges (6 icons)

```
Image 2: a sheet of 6 simple badge icons in a 3-by-2 grid with wide, even white gaps, all the same size and style, each a single object with no tile behind it:
1) an open book (Learn)
2) a royal-blue pencil drawing a small check mark (Practice)
3) a round target with an amber center (Mastery Check)
4) two curved arrows forming a circle (Review / Keep it)
5) a medal with an emerald ribbon (Mastered)
6) a small amber trophy (Secured)
Landscape 3:2. Keep each icon simple enough to still read clearly at 32 pixels wide.
```

## Image 3: Four "moment" illustrations

These are for screens that would otherwise be empty or need a moment of feedback. The app adds the words and the button.

```
Image 3: four small scene illustrations in a 2-by-2 grid with wide white gaps, same style, each a compact vignette with no background box:
1) TOP-LEFT "Empty classroom": a few empty student desks and a whiteboard with a small royal-blue door slightly open, inviting and calm.
2) TOP-RIGHT "All caught up": a teenager relaxing with a closed book and a small emerald check-mark badge floating nearby.
3) BOTTOM-LEFT "Not yet — keep growing": a small green sprout in a pot with a royal-blue watering can beside it, hopeful, not sad.
4) BOTTOM-RIGHT "Mastered": a teenager raising a small amber trophy with a few rounded confetti pieces.
Square 1:1. Characters use the fewest shapes possible, gender-neutral, mixed skin tones.
```

## Image 4: Study Lab banner

```
Image 4: a wide, calm banner illustration: an open history book on the left with a parchment, a small Liberty Bell and a quill rising out of it in a gentle arc, flowing toward a winding path on the right that ends at a small amber trophy. Lots of empty white space in the middle and right third because text will sit there. Very light, airy, mostly white with royal-blue and sky-blue accents. Wide 4:1.
```

## Image 5 (optional): Front-page hero

Skip this one if you're low on generations. The site already works without it.

```
Image 5: a front-page hero illustration: a teacher standing beside a large classroom display showing simple shapes (no words), with three students at desks using laptops, one raising a hand. Small floating history motifs around them: a scroll, a ballot box, a quill. Bright, clean, confident, mostly white background. Keep the left 40% of the image nearly empty for a headline. Wide 16:9.
```

---

## Making the most of each generation

- **Edit, don't start over.** If an image is close, ask Gemini to change one thing in the same chat ("make icon 3 simpler," "remove the shadow under icon 5"). Small edits usually keep everything else the same.
- **One fix per message.** Asking for several changes at once often makes Gemini redraw the whole image.
- **Download as you go.** Save each image as soon as it's good, so a later edit can't overwrite it.
- **Don't fix small problems.** Claude can trim edges, even out spacing, recolor slightly and remove stray backgrounds. Only spend a generation on something Claude can't fix, like a wrong object or text that sneaked in.
- **If you see text in an image,** say: *"Remove all text and letters; keep everything else identical."*

---

## What Claude will do when you upload the images

Along with adding the art, Claude will simplify the site using the same research:

1. **One clear next step per screen.** Each page gets a single main blue button, and everything else becomes a quieter secondary button.
2. **Fewer choices at once.** The student page leads with Study Lab and "Continue where you left off," and the other modes sit below in a calm grid with icons and labels.
3. **Chunked content.** Long screens are split into sections with short headings and more white space, and extra detail opens on demand ("Go deeper").
4. **Helpful empty screens.** No students yet, nothing due for review, a missed check and a mastered benchmark each get a picture, one sentence and the right button.
5. **Same patterns everywhere.** Matching button styles, card shapes and icon sizes across Teacher, Student and Present views.
6. **Readable at a glance.** Larger tap targets, high-contrast text and no motion for people who turn motion off in their settings.

Sources: Laws of UX (Cognitive Load); Jakob Nielsen, "Cognitive Load Is a Budget, Not an Enemy"; Duolingo Design (Illustration: Shape language); SAP Fiori and ServiceNow design guidance on empty states and illustrations.
