# Cue

Send the song from the good part. Cue makes a link that opens a Spotify song already set to the moment you choose.

Live at [cue.unisonarity.com](https://cue.unisonarity.com/).

## How it works

1. Paste a Spotify song link and a time (`1:30`, `90`, or `1m30s`).
2. Cue gives you a link like `cue.unisonarity.com/?track=…&t=90`, with buttons for Text, Email, WhatsApp, X and Facebook.
3. The listener opens a small page with the Spotify player and presses **Play from 1:30**.

The page is one static HTML file. There is no server and no account.

## What listeners hear

- Signed in to Spotify in their browser: the full song, starting at the chosen time.
- Not signed in: Spotify's embed only has a short preview, so Cue plays the preview from the beginning and shows **Open in Spotify, then skip to 1:30**. On phones that opens the Spotify app.

## Link parameters

| Parameter | Meaning |
|---|---|
| `track` | Spotify track or episode ID |
| `type` | `episode` for podcasts (default is a song) |
| `t` | start time in seconds |
| `n` | optional note shown above the player (140 characters) |
| `by` | `unisonarity` shows the Unisonarity credit line |
| `s` | which share button made the link (`sms`, `email`, `whatsapp`, `x`, `facebook`, `copy`, `share`) |

## Privacy

Cue sets no cookies and stores no personal data. If a GoatCounter site code is set in `index.html` (`var GC`), it counts page views and button presses as anonymous events and honors Do Not Track. With the code empty, nothing is sent.

## Credits

Made by [Unisonarity](https://www.linkedin.com/pulse/unisonarity-benjamin-linford-cfa-az4yc/). Hear the songs on [Spotify](https://open.spotify.com/playlist/6a1oImkmuQMOuLcPSnE5Co) or [Suno](https://suno.com/playlist/faa0098b-5872-4598-9124-b0180282cb1b). Not affiliated with Spotify. The player is Spotify's own embed, used under Spotify's embed terms.
