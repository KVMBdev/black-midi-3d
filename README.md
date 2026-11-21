# Black MIDI Visualizer

3D Black MIDI visualizer in one `index.html` file.
No install, no build.

## Features

- Single file, open in browser and play
- 3D piano-roll with bloom, up to 1.28M notes
- Real SF2 sound, any `.sf2`
- Tempo map, pitch bend, volume, pan, sustain

## Quick Start

1. Download `index.html`
2. Open in Chrome / Edge / Brave
3. LOAD SF2 -> pick `.sf2`
4. LOAD MIDI -> pick `.mid`
5. START PLAY

## Controls

| Control | What it does |
| --- | --- |
| Pixel Ratio | Resolution. Lower = more FPS |
| Z Speed | Note fly speed |
| Render Dist | How far ahead you see |
| Max Polyphony | Max voices, 86-1024 |
| Max Instances | Max notes on screen |

## How it works

MIDI -> NoteBuffer -> SF2 Mapper -> Audio Chunks -> Playback

Audio is rendered in chunks while playing.

## Performance

- Black MIDI 500k+ notes: Polyphony 256, Pixel Ratio 1.0
- Use small SF2 for Black MIDI
- Desktop Chrome recommended
