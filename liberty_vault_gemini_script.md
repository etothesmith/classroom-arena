# The Liberty Vault: Artifact Hunters — Gemini Art Script

**Total: 5 Gemini generations.** Your original list would have taken about 12, so this script combines pieces onto sheets. Do it all in **one new Gemini chat**, then send Claude every image in one zip. Claude cuts the sheets apart, removes the magenta backgrounds, and builds everything into the game, which is already set up to use this art.

**Already in the game, so don't make these again:** student avatars (Money Moves Avatar 3.0), Coach Smith, Prof. Reyes, Judge Holloway, Tyler, and the gold corner flourishes on the certificate.

---

## Step 0: Paste once at the start of a new Gemini chat

**Before you paste this,** attach one image from Money Moves or Counsel for the Defense (for example, a Prof. Reyes or Coach Smith picture) so Gemini matches the art style. Attaching an image doesn't use a generation.

```
You are the game artist for "The Liberty Vault: Artifact Hunters," a National Treasure–style U.S. History classroom game for high school students. It shares characters with my games Money Moves and Counsel for the Defense — the attached image shows that style. Match it.

STYLE for every image in this chat:
- Crisp, cohesive 2D illustrated game art: clean outlines, vibrant readable silhouettes, soft cel shading, one light source from the top-left.
- Treasure-hunt mood: warm gold and brass, deep navy and royal blue (#0B1F4B, #1D4ED8), aged parchment tones.
- Historically accurate objects and clothing; respectful and dignified.

BACKGROUND RULES:
- Sprites and icons go on a pure, flat solid magenta background #FF00FF. Do not use magenta or pink anywhere on the objects themselves, and add no shadows on the background.
- Scene backgrounds have no magenta.

TEXT RULE: absolutely NO words, letters, numbers, labels, logos or watermarks. Documents, maps and signs show only faint unreadable lines.
No real people's likenesses.
Reply "Ready" and wait.
```

---

## Generation 1: Artifact sheet A (Eras 1–2)
*Save as* `lv_artifacts_A.png`

```
Image 1: a sprite sheet of 6 collectible artifact icons in a 3-by-2 grid on solid magenta #FF00FF, with wide even gaps. Each artifact is centered, the same size, same lighting, no text:
1) a printed 1868 broadside poster on aged paper with a decorative border, rolled slightly at the corners (a Reconstruction document)
2) a gleaming ceremonial golden railroad spike with subtle engraved filigree
3) a folded 1887 land deed on parchment tied with a faded ribbon, beside a small surveyor's compass
4) a small 1900s immigration inspection card on a string tag, with an old steamship ticket stub behind it
5) a heavy brass canal lock key on an iron ring, with a tiny anchor charm
6) an aged parchment telegram with a red wax seal and a faint grid of cipher numbers (unreadable)
Square 1:1.
```

## Generation 2: Artifact sheet B (Eras 2–3)
*Save as* `lv_artifacts_B.png`

```
Image 2: same style, same layout — 6 artifact icons in a 3-by-2 grid on solid magenta #FF00FF, wide even gaps, no text:
1) a purple, white and gold women's suffrage sash draped beside a round brass ballot-box seal
2) a 1930s Civilian Conservation Corps enamel badge with a pine tree emblem, next to a small hand trowel
3) a vintage olive-drab WWII military field radio with brass dials and a coiled handset
4) a chrome-and-red megaphone resting beside a leather-bound legal brief tied with string
5) a black-and-white aerial reconnaissance photograph print in a manila folder, with a magnifying loupe on top
6) a metallic Apollo-era launch console key on a royal-blue and red lanyard
Square 1:1.
```

## Generation 3: All four backgrounds on one sheet
*Save as* `lv_backgrounds.png`

The game darkens backgrounds behind its cards, so a 2×2 sheet is sharp enough and saves three generations.

```
Image 3: ONE image divided into a 2-by-2 grid of four separate 16:9 scenes with thin dark gutters. Atmospheric, text-free, with calm open space in the center and bottom:
TOP-LEFT — The Liberty Vault Hub: a grand, dimly lit underground stone archive with brass gears, glass display pedestals and warm golden spotlight beams.
TOP-RIGHT — Gilded Age & Industrial Vault (1860–1910): a Victorian mahogany library joined to a steel-riveted bank vault door, warm gaslight glow.
BOTTOM-LEFT — Crossroads & War Room (1890–1940): a 1920s–1940s map room with a large wooden strategy table, brass compass and vintage wall maps (no legible text).
BOTTOM-RIGHT — Modern & Space-Age Archive (1940–present): sleek mid-century mission control blended with a marble courthouse gallery, dramatic blue and gold lighting.
Overall image 16:9.
```

## Generation 4: The Revisionist
*Save as* `lv_revisionist.png`

```
Image 4: "The Revisionist," a mysterious, sharp-dressed rival treasure hunter and leader of a syndicate that erases history. Long dark trench coat, tinted glasses, gloved hand holding a locked briefcase, confident sly smirk. Full-body standing pose, facing slightly toward the viewer, same style and proportions as the attached character art. Solid magenta #FF00FF background. Portrait 3:4.
```

## Generation 5: Liberty Vault Mastery Seal
*Save as* `lv_seal.png`

```
Image 5: an ornate embossed circular museum and treasure seal in gold and royal blue, featuring a torch, a quill and a compass rose, with a ribbon below. Text-free. Centered on a pure white #FFFFFF background (this one is white, not magenta). Square 1:1.
```

---

## Before you send them to Claude

- **Check for stray text:** zoom in on the broadside, telegram, deed, brief and maps. If letters appeared, say in the same chat: *"Erase all writing on the [object]; keep everything else exactly the same."*
- **No magenta on objects:** if pink or magenta crept into an artifact (the suffrage sash is the riskiest), ask for that one item to be recolored.
- **Don't fix small problems.** Claude can trim, remove backgrounds, even out sizes and adjust colors. Only spend a generation on a wrong object or stray text.
- **Zip all 5 files** and upload them.

### Where each image goes in the game
| Sheet | Position | Artifact / use |
|---|---|---|
| A | 1–6 | 14th Amendment Broadside · Golden Spike · Dawes Act Deed · Ellis Island Card · Panama Canal Lock Key · Zimmermann Telegram |
| B | 1–6 | Suffrage Sash & Ballot Seal · Florida CCC Badge · Code Talker Radio · Civil Rights Megaphone & Brown Brief · Cuban Missile Crisis Photo · Cape Canaveral Launch Key |
| Backgrounds | TL, TR, BL, BR | Vault hub · Era 1 · Era 2 · Era 3 |
| Revisionist | — | Story villain in every briefing |
| Seal | — | Gold seal on the certificate |
