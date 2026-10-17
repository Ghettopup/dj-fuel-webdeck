# DJ FUEL WEBDECK v0.1

First functional prototype. Open `index.html` in a desktop browser to test local MP3 import, Deck A/B loading, playback, waveform, seeking, two saved cue points per track, crossfader, editable ID3 Comments, library ordering and four-second auto fade (audio fades, then pauses).

## Important limitations
- Imported MP3 audio is session-only. After closing or reloading the page, reimport MP3s. Comments and cues are stored in localStorage, keyed by file name, size and last modified timestamp.
- Wi-Fi transfer and durable offline audio storage are **not implemented yet**.
- iOS Safari may not allow local `file://` HTML to work correctly. Use an HTTPS deployment for iPad testing. Private GitHub repositories do not provide GitHub Pages on the Free plan.
- This is not a production-safe ceremony playback system yet. Test thoroughly before relying on it at an event.
- Large audio files can require substantial memory to decode for waveform drawing.
