# Goal Counter

A big, bright, full-screen football score counter that runs in the browser and installs as an app (PWA).

- Huge GOAL! button and score for each team, plus "Take one off" for mistakes
- Little cartoon players running around the pitch, confetti and a trumpet fanfare on every goal
- Match clock: counts up, or counts down with a set game length (5, 10, 15 min…) and a full-time whistle
- Team names and colours, background music, and sound switches
- Results saved at full time, with a league table (most wins) and a list of previous games
- Everything is saved in the browser's local storage and works offline

## Play it

**Online:** https://waynebsx.github.io/game-football-scores/

The game is hosted on GitHub Pages straight from the `main` branch, so every push to `main` goes live within a minute or two.

### Install it as an app

Open the link above, then:

- **Android / Chrome / Edge (phone, tablet or computer):** tap **📲 Install app** at the top of the screen (or "Install" in the browser menu).
- **iPhone / iPad:** in Safari tap **Share → Add to Home Screen**.

Once installed it opens full screen and works offline.

### Run it locally

Open `index.html` in a browser to play. Installing as an app needs `https://` or `http://localhost`, so to test that locally:

```sh
python -m http.server 8000
# then open http://localhost:8000
```

## Updating

1. Change the files and bump `VERSION` in `sw.js` (e.g. `goal-counter-v2` → `goal-counter-v3`) so installed copies fetch the new version.
2. Commit and push to `main`; GitHub Pages republishes automatically.
3. Installed apps download the update in the background and show it the next time they are opened.

Scores, team names and results are stored in each device's browser (local storage), so they stay on that device and aren't uploaded anywhere.

## Credits

- Font: Lilita One by Juan Montoreano, SIL Open Font License (`fonts/OFL.txt`)
- Instrument samples: FluidR3 General MIDI soundfont (MIT), via [gleitz/midi-js-soundfonts](https://github.com/gleitz/midi-js-soundfonts) (MIT)
