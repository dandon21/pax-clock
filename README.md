# Pax Clock

A cue-driven stage clock for theatre. One HTML file, no install, works offline.
The operator presses GO at each cue; the clock projects to a second screen with synthesised sound.

**Use it:** open https://dandon21.github.io/pax-clock/ in Chrome (or download `pax-clock.html` and open it), click **Open projector window**, drag that window onto the projector and press `F` for fullscreen. Press any key once to arm the audio.

## Cues

| # | Cue | What happens |
|---|---|---|
| 1 | Normal | White clock, ticking, silent |
| 2 | Rewind | Spins anticlockwise and keeps accelerating until you press GO |
| 3 | Slow-mo | Hard stop, then purple with heavy glitching, ticking 60% slower |
| 4 | Blackout 1 | Projector goes black |
| 5 | Lights up | Back to the normal clock |
| 6 | Freeze | Stops dead, blue tint, wavy warp (like metamorphopsia) and a drone |
| 7 | Resume | Normal ticking returns |
| 8 | Blackout 2 | Black for the rest of the show |

## Keys

`Space` / `→` / `PgDn` / `Enter` GO · `←` / `PgUp` back · `1`–`8` jump to a cue · `P` Start / Pause / Resume · `M` mute

Back and jump are silent, so fixing a mistake never re-fires the impact sounds. A second GO within half a second is ignored.

## Make it yours

Everything tunable is in the `CONFIG` block at the top of the script: start time on the face, slow-mo speed, rewind acceleration, colours, glitch strength, warp amount and the volume of each sound. Cue names and notes are in the `CUES` list just below it. Projector size, position, brightness and volume are sliders in the operator window and are remembered per browser.

## Notes

- Keys only reach the clock when its laptop window is focused. Click it before each cue.
- Turn off display sleep and the screensaver in macOS before the show.
- All sound is generated in the browser, so there are no audio files.

MIT licence.
