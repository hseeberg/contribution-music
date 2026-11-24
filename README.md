# Contribution Music

Turn any GitHub contribution graph into music.

Live: https://hseeberg.github.io/contribution-music/
Direct link to a user: https://hseeberg.github.io/contribution-music/#USERNAME

## Reading modes

- **A · Chords** – left to right. Column = beat, row = pitch, level = volume.
- **B · Melody 7/8** – top to bottom. Week = 7-beat bar, level = pitch. Week density picks the scale (Am / Dm / C).
- **C · Drums** – row = instrument, column = step, level = hit strength.
- **D · Vikings** – like B, played by frame drum, lyre and drone.

## How it works

- One static file: `index.html`. No build step.
- Data comes from [github-contributions-api](https://github.com/grubersjoe/github-contributions-api) (unofficial, cached for one hour).
- All sound is synthesised in the browser with the Web Audio API.
- If the data service is unreachable, the page shows a sample graph.
