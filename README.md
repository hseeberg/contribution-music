# Contribution Music

Turn any GitHub contribution graph into music.

![Contribution Music: a GitHub contribution graph with a pink playhead](og.png)

- **Play it:** https://hseeberg.github.io/contribution-music/
- **Open a user directly:** `https://hseeberg.github.io/contribution-music/#USERNAME`

## How to use

1. Enter a GitHub username and select **Load graph**.
2. Choose a style.
3. Choose how many times to play: **Once**, **3 times** or **Loop**.
4. Select **Play**. A pink frame shows which square is playing.

## Styles

| Style | Reading direction | What you hear |
|---|---|---|
| **80s** | Top to bottom | Each week is one 4/4 bar: seven days plus a drum fill. Drum machine with gated snare, pulsing bass and a lead synth with echo. Week activity picks the chord: Am, F, C or G. |
| **Viking** | Top to bottom | Each week is one 7-beat bar. Frame drum, lyre and a low drone in D minor pentatonic. |
| **Drums** | Left to right | Each row is one drum, each column one step. Brighter squares hit harder. |
| **Melody** | Top to bottom | Each week is one 7-beat bar. Brighter squares play higher notes. Week activity picks the scale: A minor, D dorian or C major. A Sunday thump marks each bar. |
| **Chords** | Left to right | Each column is one beat, each row a pitch. Several active days in one week make a chord. |

## Choose what plays

- **Play range:** drag the two handles under the graph to choose the first and last week. Arrow keys, Page Up/Down and Home/End also work.
- **Skip long silences:** a run of empty weeks becomes one bar of rest.
- **Fit to activity:** trims to the first and last active week.
- **Time range:** since the first contribution, or the last 12 months.
- **Try your own pattern:** click a square to make it brighter. **Undo my changes** restores the real data.

## How it works

- Static files only: `index.html` and `og.png`. No build step, no server.
- Contribution data comes from the unofficial [github-contributions-api](https://github.com/grubersjoe/github-contributions-api). It updates every hour and shows public contributions only.
- All sound is made in the browser with the Web Audio API.
- If a username does not exist, the field says so. If the data service is down, the page keeps the last graph or shows a sample, and offers **Try again**.

## Good to know

- No sound on iPhone? Turn off silent mode.
- Private contributions appear only if the user turns them on in their GitHub profile settings.
