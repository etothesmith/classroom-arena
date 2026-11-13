# Fallacy Smash — Gemini Art Script

**Total: 2 Gemini generations** (3 if you also want the optional mascot pose). Do it all in **one new Gemini chat**, then send Claude the images in one zip.

**How it fits the game:** the game is already set up to use this art automatically. Claude cuts the sheet apart, removes the white background and builds it in. The words on the signs and the "MYTH BUSTED" / "THAT'S A FACT" stamps stay drawn by the game, so **no text is needed from Gemini**, which means nothing to garble.

---

## Step 0: Paste once at the start of a new Gemini chat

```
You are the game artist for "Fallacy Smash," a U.S. History classroom game for high school students. Students read statements on wooden signs that pop out of burrows, then bop the MYTHS and let the FACTS go.

STYLE for every image in this chat:
- Bright, friendly 2D game art: clean vector shapes, soft shading, rounded corners, no harsh outlines.
- Fun but not babyish — think a polished educational mobile game for teenagers.
- Palette: royal blue #1D4ED8, navy #0B1F4B, sky #38BDF8, warm wood browns, grass greens, cream #FFFBEB, small amber #F59E0B accents.
- One soft light source from the top-left.

TEXT RULE: absolutely NO words, letters, numbers, logos or watermarks anywhere. Signs, books and banners stay BLANK.
No real people and no copyrighted characters.
Reply "Ready" and wait.
```

---

## Generation 1: Background
*Save as* `wf_bg.png`

```
Image 1 — the game background. Wide 5:3 landscape.
A sunny lawn in front of a classical museum with white columns and a few blue-and-white pennant flags (no writing) far in the background at the very top. The museum sits small and distant in the top 25% of the image. The rest of the image is a calm, evenly lit green lawn seen from the front, slightly lighter in the middle, with a few small flowers only along the left and right edges. Keep the middle and lower 75% simple and low-contrast, with no objects, holes, paths or characters, because game pieces will be placed on top. Soft, cheerful morning light.
```

## Generation 2: Game pieces sheet
*Save as* `wf_pieces.png`

```
Image 2 — a sprite sheet of 4 game pieces on a pure solid WHITE background, arranged in a 2-by-2 grid with wide white gaps. Each piece is a single object, front view, same lighting and style, nothing touching the edges:
1) TOP-LEFT: a dirt burrow hole seen from the front — a wide, flat dark oval opening with a rim of brown soil and a few grass tufts around the edge. Very wide and short (about 3 times wider than tall).
2) TOP-RIGHT: a BLANK wooden sign board for writing on — a wide rectangle of smooth cream parchment (#FFFBEB) set inside a rounded warm-wood frame with two small brass nail heads at the top corners. Landscape, about 3:2. The parchment area must be completely empty and evenly lit.
3) BOTTOM-LEFT: a friendly gopher mascot wearing small round spectacles and a tiny navy scholar's cap, peeking up with both paws raised high above its head as if holding something up. Shown from the chest up. Cute but clever-looking.
4) BOTTOM-RIGHT: a cartoon wooden mallet with a royal-blue rubber head, standing upright with the head at the top.
Square 1:1.
```

## Generation 3 (optional): Mascot reactions
*Save as* `wf_mascot_moods.png`

Only do this if you have generations to spare. It adds a happy and a dizzy gopher for right and wrong answers.

```
Image 3 — the same gopher mascot from image 2 (same spectacles, cap, colors and style), two poses side by side on a pure white background with a wide white gap between them:
LEFT: cheering with both arms up and a big smile.
RIGHT: dizzy with swirly eyes and a small bump on its head, still friendly (not hurt).
Chest-up view, both the same size. Landscape 2:1.
```

---

## Before you send them to Claude

- **Look for stray text:** zoom in on the sign and the flags. If any letters appeared, say in the same chat: *"Erase all writing on the [object]; keep everything else exactly the same."*
- **The sign must be blank and evenly colored.** The game writes the statement there, so a busy texture would make it hard to read.
- **Don't fix small problems.** Claude can trim edges, remove the white background, even out colors and resize. Only spend a generation on a wrong object or stray text.
- Zip the 2–3 images and upload them.
