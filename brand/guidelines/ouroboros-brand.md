# Ouroboros Consulting — Brand Guidelines

---

## Identity

**Wordmark:** OUROBOROS CONSULTING  
**Arc:** ♟ → ♛ &nbsp; Forward-only. Full transformation.

The ♟→♛ pair operates on two levels simultaneously: for clients, it is the survivor arc; for Apostolos, it is the autobiography. No other symbol in the system carries both readings at once.

---

## Color System

### Surfaces

| Token | Hex | Role |
|-------|-----|------|
| `--bg1` | `#141414` | Page background |
| `--bg2` | `#1E1E1E` | Cards, panels |
| `--bg3` | `#252525` | Elevated headers |
| `--border` | `#333333` | Default borders |
| `--calloutbg` | `#2A2A2A` | Callout blocks |

### Luminance Hierarchy (all pass WCAG AA on `--bg1`)

| Token | Hex | Contrast | Use |
|-------|-----|----------|-----|
| `--bright` | `#FFFFFF` | 18.4:1 | Emphasis only |
| `--text` | `#E8E4DC` | 14.5:1 | Body copy |
| `--subdued` | `#B0AAA0` | 8.0:1 (AAA) | Secondary text |
| `--muted` | `#999999` | 6.5:1 (AA) | Metadata |

### Accent Colors

| Token | Hex | Pillar | LaTeX |
|-------|-----|--------|-------|
| `--gold` | `#C9A84C` | Institutions | `[accent=gold]` |
| `--amethyst` | `#967ABB` | Psychopathology | `[accent=amethyst]` |
| `--sage` | `#6A8E7F` | Technology | `[accent=sage]` |
| `--steel` | `#7B8FA1` | Miscellaneous | `[accent=steel]` |
| `--teal` | `#4a6b5f` | Logo frame only | — |

Each accent ships with `--{name}-dim` (35% α) and `--{name}-ghost` (12% α) variants.  
`--gold-border: #B1935D` — opaque, for 1px visible borders.

---

## Elevation System

Three levels. Scallop pitch signals depth: finer = recessed, coarser = elevated.

| Level | Mixin | Background | Scallop |
|-------|-------|------------|---------|
| Recessed | `@include elevation-recessed` | `--bg1` | 12px pitch |
| Standard | `@include elevation-standard` | `--bg2` + shadow | 16px pitch |
| Elevated | `@include elevation-elevated` | `--bg2` + `--bg3` gradient + shadow | 24px pitch |

Scallop accent hex passed as SCSS arg without `#` — e.g. `@include scallop-elevated('C9A84C')`.

---

## Typography

| Role | Family | Weight | Size | Color |
|------|--------|--------|------|-------|
| Display / Wordmark | Poppins | 700 | 26–30px | `--gold` |
| Heading | Poppins | 600 | 18–22px | `--text` |
| Section label | Poppins | 600 | 10–11px uppercase | `--subdued` |
| Body | Lora | 400 | 15px / 1.75 leading | `--text` |
| Body italic / pull quote | Lora | 400i | 15px | `--subdued` |
| Caption | Lora | 400i | 12px | `--muted` |
| Code / tokens | JetBrains Mono | 400 | 11–12px | `--sage` |

SCSS variables: `$font-serif`, `$font-sans`, `$font-mono`.

---

## Chess Symbolism

| Piece | Glyph | Represents |
|-------|-------|------------|
| Pawn | ♟ | Clients · survivors · forward-only movement · transforms |
| Queen | ♛ | Apostolos · polymath range · moves in every direction |
| Rook | ♜ | Institutional rigidity |
| Bishop | ♝ | Credentialed blind spots · diagonal-only thinking |
| Knight | ♞ | Navigating obstacles · unconventional paths |

---

## Content Pillars

| Accent | Pillar | Piece | Topics |
|--------|--------|-------|--------|
| Gold | Institutions | ♜ | Betrayal, power structures, survivor advocacy |
| Amethyst | Psychopathology | ♝ | Diagnostic harm, epistemic failures, credentialed blind spots |
| Sage | Technology | ⎈ | AI ethics, data privacy, access equity |
| Steel | Miscellaneous | ♞ | Brand intro, cross-pillar, meta |

Every carousel deck requires a sources slide. Every Substack essay ends with a LinkedIn CTA.

---

## Dingbat Vocabulary

No emoji. Dingbats only — in prose, decks, and social copy.

| Glyph | Use |
|-------|-----|
| ❖ | General callout |
| ♟ | Client / survivor |
| ♛ | Consulting self |
| ♜ | Institution |
| ♝ | Credential / bias |
| ♞ | Obstacle / workaround |
| ⎈ | Technology / systems |
| ◆ | Section break |
| → | Transformation arc |

---

## Voice

**Do:** Direct. No filler. Subject + verb. Claims backed by sources. Freyd framework when citing betrayal. Pawn→Queen arc stays visible.

**Don't:** Overuse em dashes. "The gap", "it matters", "dive into". Unverified credentials or timelines. Diplomatic softening of hard facts. First drafts without outline approval.

---

## Publishing Cadence

| Channel | Schedule |
|---------|----------|
| LinkedIn | New carousel · Friday · Text post (Substack repurpose) · mid-week |
| Substack | Essay · Tuesday · Essay · Sunday |
| GitHub Pages | Substack essays mirrored for SEO |

Target: +5% LinkedIn engagement / 30 days.
