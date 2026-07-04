# Loopy — mini song looper

A one-file web app for making music loops. Open `index.html` in any modern browser
(or serve the folder over HTTP). Designed for an iPhone in landscape.

## How to use
1. Pick a sound tab: **Bass / Synth / Keys / Brass** and play the keyboard.
2. Tap **●** — you get a 4-beat count-in, then everything you play is recorded into the loop.
   The loop keeps cycling, so you can layer more notes on any pass, or switch sounds and
   keep recording — each sound gets its own track automatically.
3. **Drums** are premade beats: pick a kit (808 / Rock / Electro), tap a beat and it drops
   straight into the loop (playback starts so you hear it). Tap another beat to swap, tap the
   same one to remove it, or switch kits to hear the same groove with different drum sounds.
4. Tap **●** again to stop recording (playback keeps going). **▶ / ■** plays or stops the loop.
5. Each track in the left panel has **M** (mute) and **✕** (delete). To re-record a part:
   tap **✕**, then **●**.
6. **Parts can be different lengths.** The 2 / 4 / 8 selector sets the length of the *next part
   you record*. A 2-measure bass riff keeps cycling inside a 4- or 8-measure song — the song
   is automatically as long as its longest part (each track shows its length, e.g. "2m").
7. **💾 Songs** saves the current song (tracks, tempo, lengths) in your browser. Tap a saved
   song to load it back, ✕ to delete it. Saves survive page reloads.
8. Top bar: tempo (− / +, hold to scrub), part length (2 / 4 / 8 measures), metronome toggle,
   💾 songs, and **MP3 ⬇** export (choose 1–10 repeats).

Notes are lightly quantized to 16th notes so loops stay tight.

## Files
- `index.html` — the whole app (Web Audio API, no build step)
- `lame.min.js` — lamejs MP3 encoder (loaded locally, works offline)
