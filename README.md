# Taali Meter

An applause meter for the People's Choice award at GDG Ahmedabad Garbathon 2026. The crowd claps for each finalist, the laptop mic measures how loud and how long, and the highest score wins.

**Live:** https://dadiyanidhi.github.io/taali-meter/

## Run it

Open the live link in Chrome (or open `index.html` locally), click **Turn on mic**, allow microphone access, and stay quiet for 3 seconds while it measures the room.

| Key | Action |
|---|---|
| Space | Start a round (3-2-1, then clap) |
| ← / → | Previous / next finalist |
| R | Redo the current finalist |
| C | Re-measure the room |
| W | Reveal the winner |
| S | Setup: finalist names, clap time, sensitivity |
| F | Fullscreen |

## Before the event

- Do one test clap in the real room. Loud applause should land around 90; lower sensitivity if it hits 100 too easily.
- Keep the laptop in the same spot for every finalist so scores stay comparable.
- Scores are saved in the browser, so a refresh doesn't lose them. Use **Reset all scores** in setup to start fresh.

Scoring: each round samples the mic level every frame; score = 70% average level + 30% 90th-percentile level, scaled 0–100.
