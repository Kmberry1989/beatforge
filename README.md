# BeatForge v2 — Browser Drum Machine

A fully self-contained drum sequencer that runs in any modern browser. No installs, no external samples, no CDN dependencies.

## Features
- **16-step sequencer** with 13 tracks
- **4 built-in kits**: Classic Synth, TR-808, Acoustic, Lofi
- **Per-track controls**: volume, mute, solo
- **Generate beats**: Rock, Trap, House, Breakbeat, Latin + Randomize
- **Swing, tempo (60-200 BPM), tap tempo**
- **Load your own samples**: drag-and-drop WAV/MP3/OGG onto any track, or click the folder icon
- **Export**: 
  - WAV (2 or 4 bars, rendered offline)
  - MIDI (General MIDI drums, channel 10, drag straight into Ableton/FL/LMMS)
- **Save patterns**: 8 slots in localStorage
- **Keyboard**: Space = play/pause

### Tracks & MIDI mapping
- Kick 1/2 → C1 (36)
- Snare 1/2 → D1 (38)
- Closed Hat → F#1 (42)
- Open Hat → A#1 (46)
- Ride → D#2 (51)
- Ride Bell → F2 (53)
- Crash → C#2 (49)
- Splash → G2 (55)
- Floor Tom → F1 (41)
- Mid Tom → A1 (45)
- High Tom → C2 (48)

## How to run locally
1. Download `beatforge-v2.html`
2. Double-click to open in Chrome/Edge/Firefox
3. That's it — works offline

## GitHub Pages deployment
1. Create repo: `beatforge`
2. Rename `beatforge-v2.html` to `index.html`
3. Commit and push
4. Settings → Pages → Deploy from main branch
5. Your app lives at `https://yourusername.github.io/beatforge/`

## Loading samples
- Click the 📁 next to a track, or drag a file onto the row
- Samples replace the synth for that track only
- Click ✕ to revert to the built-in sound
- Samples are kept in memory (not saved to localStorage to avoid bloat)

## Kits explained
- **Classic Synth**: clean digital drums (original)
- **TR-808**: long 808 boom, snappy snare, metallic hats
- **Acoustic**: natural envelopes, darker tone, realistic decay
- **Lofi**: low-passed, bitcrushed, tape warmth + vinyl crackle

Built with vanilla Web Audio API. No frameworks, no tracking.

MIT License — do what you want with it.
