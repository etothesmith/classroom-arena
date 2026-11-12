# Classroom Arena — Gallery Walk Gemini Script, Part 2

**What this covers:**
- **Fix 1:** erases the garbled writing in the Emancipation Proclamation and 14th Amendment pictures.
- **Generations 3–8, 10 and 11:** the 8 remaining images, which cover 24 more stations.

**Total: 9 Gemini generations.** Do everything in **one new Gemini chat**, then send Claude all the files in one zip.

**What's new:** a stricter text rule in Step 0. Gemini garbles small writing, so now only the short labels in quotation marks may appear, and they must be big. Every other newspaper, sign, document or envelope stays blank.

---

## Step 0: Paste once at the start of a new Gemini chat

```
You are illustrating teaching images for a U.S. History classroom app. In this chat I will ask for images using these style codes:
- ENGRAVING: black-and-white wood engraving like an 1860s–1870s American illustrated weekly; fine parallel-line hatching, dramatic light and shadow.
- PUCK: full-color chromolithograph like an 1880s–1900s American humor magazine; bold black outlines, flat pastel colors, allegorical scene, ornate title banner across the top.
- INK: 1910s–1920s newspaper editorial cartoon; loose black-ink brushwork with soft crayon shading on textured newsprint.
- CRAYON: 1930s–1940s newspaper editorial cartoon; heavy ink outlines and grease-crayon shading.
- WPA: 1930s WPA silkscreen poster; flat earthy colors, simplified geometric shapes, bold sans-serif lettering.
- HOMEFRONT: 1940s U.S. homefront poster; flat bold colors, silkscreen texture, strong diagonal composition, large blocky headline.
- INKWASH: 1950s–1960s editorial cartoon; expressive brush line with gray ink-wash tones, sparse background.
- TEXTBOOK: muted watercolor-and-ink textbook illustration with historically accurate clothing and setting.

TEXT RULES (very important):
1. The ONLY words allowed are the labels I put in quotation marks. Spell them exactly, in LARGE, bold, clear capital letters.
2. Every other newspaper, letter, book, sign, poster, envelope, banner or document must be BLANK or show only faint wavy lines. Never invent words, never write small print.
3. No signatures, no watermarks, no extra captions.

OTHER RULES: Original artwork — do not copy any existing cartoon, poster or photograph, and do not show the likeness of any real person. When I ask for panels, make ONE image divided into separate panels with thin white gutters; panels must not bleed into each other.
Reply "Ready" and wait.
```

---

## Fix 1: Erase the garbled writing (1 generation)

**Attach** `engraving_3panel_1863_1868_1886.jpg`, the 3-panel engraving sheet from your bundle, then paste:

```
Edit the attached image. Keep the style, people, poses and composition EXACTLY the same. Make only these two changes:
1. Left panel: erase all writing on the newspaper the officer on horseback is reading — make it a blank page with only faint wavy lines.
2. Middle panel: erase all writing on the paper lying on the table inside the doorway — make it blank. Keep the large sign "EQUAL PROTECTION OF THE LAWS" above the door exactly as it is.
Do not change anything else.
```
*Save as* `gallery_01_fixed.png`. Claude only uses the left and middle panels from this, so it doesn't matter if the right panel changes.

---

## Generation 3: PUCK
*Save as* `gallery_03.png`. Station: The Roosevelt Corollary.

```
Style PUCK. One single illustration, 4:3 landscape.
Scene: a giant figure in a campaign hat labeled "U.S. POLICE POWER" wades across the Caribbean Sea carrying an enormous club labeled "BIG STICK", towing a line of small warships labeled "DEBT COLLECTOR". Title banner: "SPEAK SOFTLY... — 1904".
```

## Generation 4: INK
*Save as* `gallery_04.png`. Stations: The Zimmermann Telegram · A Return to Normalcy · The Eighteenth Amendment.

```
Style INK. One image, single row of 3 separate panels, each panel 4:3 landscape.
Panel 1 (left): Scene, 1917: a figure in a spiked helmet labeled "GERMANY" secretly slides a blank telegram across a map toward a region labeled "MEXICO", while a codebreaker labeled "BRITISH" reads it over his shoulder with a magnifying glass. Caption: "DECODED — 1917".
Panel 2 (middle): Scene, 1920: a tired Uncle Sam steps off a gangplank from a ship labeled "WORLD WAR" onto a dock labeled "NORMALCY", while shadowy figures labeled "STRIKES" and "RED SCARE" loom in the fog. Caption: "BACK TO NORMAL? — 1920".
Panel 3 (right): Scene: a grim figure in black labeled "PROHIBITION" guards a barred saloon door labeled "CLOSED", while around the corner a sly figure labeled "BOOTLEGGER" hands crates to a doorway labeled "SPEAKEASY". Caption: "1920s".
```

## Generation 5: CRAYON
*Save as* `gallery_05.png`. Stations: Rugged Individualism · Nothing to Fear · The Court-Packing Fireside Chat · The Truman Doctrine.

```
Style CRAYON. One image, 2×2 grid of 4 separate panels, each panel 4:3 landscape.
Panel 1 (top-left): Scene, 1930: a man in a stiff collar labeled "VOLUNTARISM" offers a tiny bandage to a giant cracked figure labeled "DEPRESSION", while a long line of unemployed men waits outside a soup kitchen. Caption: "IS IT ENOUGH?".
Panel 2 (top-right): Scene, 1933: a crowd presses against the doors of a bank under a giant shadow labeled "FEAR"; a confident figure labeled "NEW DEAL" holds up a lamp whose light shrinks the shadow. Caption: "NOTHING TO FEAR — 1933".
Panel 3 (bottom-left): Scene, 1937: a figure labeled "PRESIDENT" tries to squeeze extra chairs onto a crowded bench labeled "SUPREME COURT", while a balance scale labeled "CHECKS AND BALANCES" tips. Caption: "PACKING THE COURT — 1937".
Panel 4 (bottom-right): Scene, 1947: Uncle Sam builds a brick wall labeled "CONTAINMENT" along the edge of a map of Europe while a red tide labeled "SOVIET EXPANSION" presses against it; two small figures labeled "GREECE" and "TURKEY" help hold the line. Caption: "1947".
```

## Generation 6: WPA
*Save as* `gallery_06.png`. Station: Signing the Social Security Act.

```
Style WPA. One single illustration, 3:4 portrait.
Scene, 1935 public-information poster: an older couple and a factory worker stand under a large protective umbrella labeled "SOCIAL SECURITY"; Art Deco lettering; headline "SECURITY FOR OLD AGE — 1935".
```

## Generation 7: HOMEFRONT
*Save as* `gallery_07.png`. Stations: A Date Which Will Live in Infamy · Executive Order 8802 · The Marshall Plan Speech.

```
Style HOMEFRONT. One image, single row of 3 separate panels, each panel 3:4 portrait.
Panel 1 (left): Scene: the silhouette of a burning battleship against a dawn sky over a Pacific harbor; headline "REMEMBER DECEMBER 7th".
Panel 2 (middle): Scene, 1941: a line of Black and white job-seekers waits at a defense-plant gate under a large sign "NOW HIRING — NO DISCRIMINATION"; inside, workers assemble an aircraft wing; headline "DOUBLE VICTORY".
Panel 3 (right): Scene, 1948: cargo ships unload grain and machinery in a rebuilt European port as workers cheer; flags fly (no writing on the flags); headline "REBUILDING EUROPE — 1948".
```

## Generation 8: INKWASH
*Save as* `gallery_08.png`. Stations: A Declaration of Conscience · Civil Rights Act of 1964, Title II · The Great Society · The Gulf of Tonkin Resolution.

```
Style INKWASH. One image, 2×2 grid of 4 separate panels, each panel 4:3 landscape.
Panel 1 (top-left): Scene, 1950: a senator figure labeled "ACCUSER" waves a long blank list at a crowd of frightened citizens, while four shadowy horsemen labeled "FEAR", "IGNORANCE", "BIGOTRY" and "SMEAR" ride across the sky behind him. Caption: "1950".
Panel 2 (top-right): Scene, 1964: at a lunch counter a large "WHITES ONLY" sign is being taken down while Black and white customers sit side by side. Caption: "TITLE II — 1964".
Panel 3 (bottom-left): Scene: a president figure labeled "GREAT SOCIETY" juggles three balls labeled "MEDICARE", "HEAD START" and "WAR ON POVERTY" while a heavy iron ball labeled "VIETNAM" drags at his ankle. Caption: "1966".
Panel 4 (bottom-right): Scene: a figure labeled "CONGRESS" hands a giant check labeled "BLANK CHECK" to a figure labeled "PRESIDENT" standing at the edge of a jungle labeled "VIETNAM". Caption: "1964".
```

## Generation 10: TEXTBOOK
*Save as* `gallery_10.png`. Stations: The Thirteenth Amendment · Harlan's Dissent in Plessy v. Ferguson · "With All, and for the Good of All" · Two Paths: Washington and Du Bois.

```
Style TEXTBOOK. One image, 2×2 grid of 4 separate panels, each panel 4:3 landscape.
Panel 1 (top-left): Scene, December 1865: a Black family walks down a dirt road away from a plantation at sunrise, carrying their belongings, toward a small town with a church steeple; a large wooden signpost beside the road reads "1865".
Panel 2 (top-right): Scene, Louisiana 1892: a railroad platform beside two passenger cars with large signs "WHITE" and "COLORED"; a conductor directs a well-dressed Black passenger toward the second car. No other writing.
Panel 3 (bottom-left): Scene, Ybor City, Tampa, 1891: a crowded cigar-factory hall where workers roll cigars at long wooden tables while a reader sits on a raised platform reading aloud from a blank newspaper; Cuban flags hang from the rafters and palm trees show through tall windows. No writing anywhere.
Panel 4 (bottom-right): Scene, early 1900s: a crossroads with three paths and three large signposts — "WORK" pointing to a workshop and farm school, "RIGHTS" pointing to a courthouse, and "PRIDE" pointing to a harbor with a steamship. Sepia tones, dignified mood.
```

## Generation 11: TEXTBOOK
*Save as* `gallery_11.png`. Stations: Murphy's Dissent in Korematsu · Brown v. Board of Education · Gideon v. Wainwright · Tear Down This Wall.

```
Style TEXTBOOK. One image, 2×2 grid of 4 separate panels, each panel 4:3 landscape.
Panel 1 (top-left): Scene, 1942: Japanese American families with suitcases and blank paper identification tags wait at a train station under armed guard; a child holds a doll; a blank notice is posted on a wall. Dignified, non-stereotyped, somber mood. No writing anywhere.
Panel 2 (top-right): Scene, 1954: Black and white children walk together through the front door of a brick schoolhouse with a large sign "PUBLIC SCHOOL" over the door. No other writing.
Panel 3 (bottom-left): Scene, Florida, 1962: a man writes a letter in pencil at a small desk in a prison cell under a barred window; the letter and the envelope beside him are blank. Muted tones. No writing anywhere.
Panel 4 (bottom-right): Scene, November 1989: crowds celebrate on top of a concrete wall covered in colorful abstract paint (no letters), some swinging hammers and chisels, fireworks overhead and a stone gate in the background. Vivid, joyful mood. No writing anywhere.
```

---

## Before you send them to Claude

- **Zoom in on every label.** If anything is misspelled or there's gibberish writing, fix it in the same chat with: *"Erase all writing on the [object] in panel [number] — make it blank. Keep everything else exactly the same."*
- **One fix per message,** so Gemini doesn't redraw the whole image.
- **Send all 9 files in one zip.** Claude cuts the panels apart, swaps in the fixed Emancipation and 14th Amendment pictures, attaches the rest to their stations and updates both sites.
