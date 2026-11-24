# strudel-studio

A graphical studio for [Strudel](https://strudel.cc): step sequencer, piano roll, pattern tracks, song sections, recording pads and real instruments. Everything you build is written out as real Strudel code.

Live: https://timconradinc.github.io/strudel-studio/

## Settings

App defaults live in [`settings.json`](settings.json), which the app reads when it starts (the same defaults are built into `index.html` as a fallback). It covers:

- `attribution`: the model credited in generated code
- `defaultPreset`, `maxSaves`, `undoDepth`
- `codePanel`: width, limits, collapsed, line wrapping
- `controls`: ranges and defaults for volume, pitch, tone, decay, attack, release
- `pads`: phone/desktop grid sizes, colours per instrument type, symbol colour, default pad sounds

Your own choices (pad sounds, code panel size, "prefer synths", saved grooves) are kept in the browser.

Generated with Claude Opus 5.5. Version: 2026-11-23-23 (date + build number for that day, shown under the logo and in the generated code).

## Disclaimer

Strudel Studio is vibe-coded: the whole app was written by Claude (Anthropic's AI) from plain-language requests. Generated music only follows general ideas about each genre (typical tempos, instruments, rhythms and chord moves) and is largely random, so treat it as a starting point, not a faithful example of the style.
