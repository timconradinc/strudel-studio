# strudel-studio

A graphical studio for [Strudel](https://strudel.cc): step sequencer, piano roll, pattern tracks, song sections, recording pads and real instruments. Everything you build is written out as real Strudel code.

Live: https://timconradinc.github.io/strudel-studio/

## Workflow

- **New Groove** — one click, a one-bar groove in a random style.
- **New Song** — pick a Genre, Generated or Empty, then **Create Song** (Song shape and Number of parts are under More options).
- **Instrument set** — swaps the sounds in the current song; notes, rhythms, arrangement and tempo stay.
- **Randomize section** sits beside the section, with an Undo right after it.
- **+ Add Part** — New Part, Duplicate Part (independent copy) or Repeat Existing Part (a linked repeat: edits apply to every occurrence, marked 🔗). Each part's ⋯ menu has Move Up / Move Down; on a laptop you can also drag.
- **🎻 Examples** (left of My Grooves) opens the classical pieces; **My Grooves** opens your saved songs; **Save** sits beside it. The menu shows the song title — a green **New:** for an unsaved generated song, and **Unsaved changes** after editing a saved one.
- **Phones** get a bottom dock with Rewind, Play/Stop, Repeat song, Tempo, Examples, My Grooves and Save, plus full-width **Tracks / Pads / Chords / Code** views (Record stays in Pads, Run Code in Code). Laptops show the same controls side by side, with keyboard shortcuts (Space play/stop, R randomize section, Ctrl/⌘+Enter run code, Ctrl/⌘+Z undo).

## Settings

App defaults live in [`settings.json`](settings.json), which the app reads when it starts (the same defaults are built into `index.html` as a fallback). It covers:

- `attribution`: the model credited in generated code
- `defaultPreset`, `maxSaves`, `undoDepth`
- `codePanel`: width, limits, collapsed, line wrapping
- `controls`: ranges and defaults for volume, pitch, tone, decay, attack, release
- `pads`: phone/desktop grid sizes, colours per instrument type, symbol colour, default pad sounds

Your own choices (pad sounds, code panel size, "prefer synths", saved grooves) are kept in the browser.

Generated with Claude Opus 5.5. Version: 2026-11-26-01 (date + build number for that day, shown under the logo and in the generated code).

## Disclaimer

Strudel Studio is vibe-coded: the whole app was written by Claude (Anthropic's AI) from plain-language requests. Generated music only follows general ideas about each genre (typical tempos, instruments, rhythms and chord moves) and is largely random, so treat it as a starting point, not a faithful example of the style.
