# Goal Counter

A big, bright, full-screen football score counter that runs in the browser and installs as an app (PWA).

- Huge GOAL! button and score for each team, plus "Take one off" for mistakes
- Little cartoon players running around the pitch, confetti and a trumpet fanfare on every goal
- Match clock: counts up, or counts down with a set game length (5, 10, 15 min…) and a full-time whistle
- Team names and colours, background music, and sound switches
- Results saved at full time, with a league table (most wins) and a list of previous games
- Everything is saved in the browser's local storage and works offline

## Run it

Open `index.html` in a browser to play.

To install it as an app, it must be served over `https://` (or `http://localhost`):

```sh
python -m http.server 8000
# then open http://localhost:8000 and press "Install app"
```

Any static host works (GitHub Pages, Netlify, …). After changing any file, bump `VERSION` in `sw.js` so installed copies update.

## Credits

- Font: Lilita One by Juan Montoreano, SIL Open Font License (`fonts/OFL.txt`)
- Instrument samples: FluidR3 General MIDI soundfont (MIT), via [gleitz/midi-js-soundfonts](https://github.com/gleitz/midi-js-soundfonts) (MIT)
