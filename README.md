# PROMPTA — Professional Genre Prompt System

A data-driven prompt generator for **Suno AI Custom Mode**. Generate precise, historically-grounded, royalty-safe music prompts without artist names.

**22 Genres · 150+ Subgenres · 600+ Curated Era Anchors · Bilingual (DE/EN) · Single-File HTML · Offline First**

---

## What is PROMPTA?

PROMPTA is a specialized prompt generator designed for music producers using Suno AI to create commercial sample packs, loops, and compositions.

Instead of generic prompts like *"cinematic, atmospheric, deep"*, PROMPTA delivers **data-driven variants**:
- Historically positioned (era-anchored with dual-layer descriptions)
- Sound-precise (drum patterns, bass characteristics, mixing topology)
- Artist-name-free (GEMA-safe for commercial production)
- Browser-based, offline, no tracking

---

## Who is this for?

Producers who:

- Build commercial sample packs on Suno and need artist-name-free prompt workflows (compliance with Suno ToS, legal safety, platform risk mitigation)
- Want variation and control, not algorithmic lottery
- Need precise control over tempo, key, era-context, and mix character
- Work with niche subgenres not in standard ChatGPT/Claude vocabularies: Dungeon Synth, Lowercase Ambient, Forest Psy, Drift Phonk, Brazilian Phonk, Acid Jazz, Berlin School, Fourth World, Psybient, etc.

---

## Core Features

### 1. Artist-Name-Free Architecture
- **600+ era anchors** contain zero artist, band, label, or venue names
- All descriptions are sound-property specific: drum patterns, bassline character, BPM, modality, mix topology
- External audit verification on every release
- **Safe for commercial pack production and sale**

### 2. Two-Layer Era Anchors
Each subgenre includes 4 curated historical anchors with dual descriptions:
- **Label** (UI): "1986 New York deep aesthetic"
- **Prompt** (Suno): "warm Rhodes chords, jazz-tinged 7ths, soft swung hi-hats, deep round sub bass, soulful vocal chops, no acid"

Suno receives both context and concrete sound instruction, not vague style terms.

### 3. Suno Custom Mode Compliance
- **Style Description**: Hard-capped at 1000 characters (including humanization)
- **Exclude Styles**: Separate field, comma-separated, no "no"/"-" prefixes
- **Standardized Humanization**: *"loose live performance, heavy swing, slightly behind the beat, natural room bleed, human imperfections"* (~94 chars)

### 4. Intelligent Contradiction Detection
- **35+ synonym groups** and **11 contradiction pairs**
- Real-time warnings if selections conflict (e.g., "atmospheric" + "brutal")
- **v5.1+**: Deep analysis of era-anchor sound contents
- If an anchor contains "aggressive distortion" and you've excluded "aggressive elements" → red warning

### 5. Musician-Realistic Bar Structures
- Intro/Outro: 4/8/16 bars
- Verse: 16/32 bars
- Hook/Chorus: 8/16 bars
- Section: 16/32/64 bars
- Natural variation, not mechanical repetition
- Minute-mode preserved for Ambient/Score work

### 6. Optional Creative Layers
- **Curveball**: Injects one genre-foreign element per variant (e.g., dub-techno stab in house)
- **Second Steer**: "Genre A meets Genre B" DNA injection ("deep house carrying breakbeat-garage shuffled 2-step")

### 7. Song Structure Generator
- 150+ subgenre-specific structures with section tags
- Suno lyrics-field ready: `[Break]`, `[Intro Silence Xs]`, `[Fade Out]`, etc.

---

## How to Use

1. **Select Genre & Subgenre** → UI populates with curated vocabulary
2. **Choose Era Anchors** (optional, recommended) → live preview shows what Suno receives
3. **Check Moods, Instruments, Production Character**
4. **Set/Exclude BPM & Keys**
5. **Review Negatives** (what should NOT appear)
6. **Check Integrity Bar** → no contradictions
7. **Generate Variations** (1–10) → each has Style Description + Exclude Styles, copy-ready

---

## Why This Matters

Vague prompts → vague tracks. Precise prompts → precise outputs.

PROMPTA systematizes concrete prompting for producers who use Suno as a tool, not a lottery.

---

## Technical Details

- **Single HTML file**: Runs entirely in-browser, zero dependencies
- **Offline**: No cloud, no logins, no tracking
- **Storage**: Prompts saved locally in browser localStorage
- **Language**: UI bilingual (DE/EN), all outputs English (Suno language)

---

## Legal & Compliance

### PROMPTA's Role
PROMPTA generates **text prompts only**. It does not generate, produce, or distribute music. The tool itself is premise-agnostic and does not endorse, encourage, or facilitate copyright infringement.

### Your Responsibility: Suno Usage
- **PROMPTA is not affiliated with, endorsed by, or sponsored by Suno**
- **Suno is a trademark of its respective owner**, referenced here solely for compatibility
- **Your use of Suno** is governed exclusively by [Suno's Terms of Service](https://suno.ai)
- **For commercial use of Suno-generated music**: A paid Suno plan **at creation time** is required per Suno ToS
- **You are solely responsible** for ensuring compliance with Suno's terms

### Generated Content Safety
- PROMPTA-generated prompts contain **zero artist/band/label names** by design (verified via audit script)
- No warrant as to legal usability of Suno-generated music
- PROMPTA is not legal advice

### Intellectual Property
- PROMPTA's era-anchor data, subgenre logic, and prompt pools are proprietary
- Unauthorized reproduction, distribution, or commercial use without written permission is prohibited
- Violations will be pursued legally

### No Warranty
PROMPTA is provided "as-is" without warranty of any kind. Use at your own risk.

---

## Version History

| Version | Core Changes |
|---------|--------------|
| v5.1 | Era-reset on subgenre change · Integrity check for era content · Suno live preview |
| v5.0 | Complete name scrub · 600 two-layer era anchors · artist-name-free architecture |
| v4.8 | Musician-realistic bar mode |
| v4.6/4.7 | Selection analysis with contradiction detection |
| v4.4 | Era-anchor layer introduction |
| v4.2 | Structure templates for all 150+ subgenres |

---

## Built By

**Daniel / Locoseed** with Claude — Music producer, Suno enthusiast

---

## License

PROMPTA's data, logic, and prompt pools are proprietary. See legal section above.

The tool is provided for personal and commercial prompt generation use. Redistribution of PROMPTA itself (modified or unmodified) without authorization is prohibited.
