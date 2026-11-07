# Wordle

A classic Wordle puzzle with adjustable difficulty, unlimited free hints, and no ads. The whole game is a single `index.html` file — no build step, no server, no tracking.

**Live demo:** https://wordle.stories-lab.com

## Features

- **Classic rules** — guess the hidden word; green = right spot, yellow = wrong spot, gray = not in the word.
- **Adjustable difficulty**
  - Word length: 4, 5, or 6 letters
  - Attempts: 3–10
  - Word pool: everyday words, all words, or hard words
  - Hard mode: revealed hints must be used in later guesses
  - Presets (Easy / Normal / Hard / Expert) plus up to 4 saved custom presets
- **Unlimited free hints** — reveal a letter's position, a letter that's in the word, a letter that isn't, or see how many candidate words remain.
- **One unlisted-word guess per game** — submit a word that isn't in the dictionary once (press Enter twice to confirm).
- **Click any tile** in the current row to type there, without filling earlier letters first.
- **Custom word challenges** — enter your own word and share a link; whoever opens it plays that word.
- **Accessibility & comfort** — colorblind mode, light/dark/system theme, on-screen and physical keyboard.
- **English / 한국어 UI** — English by default; switch in Settings.
- Stats (played, win %, streak) are stored locally in your browser.
- **Korean Wordle (`ko.html`)** — three ways to play: *Jamo split* (one tile per consonant/vowel), *Syllable* (compose whole syllables, with initial/vowel/final indicator bars), and *Choseong* (initial consonants given). Unlimited hints, including meaning hints.

## Run locally

Just open `index.html` in a browser. Nothing to install.

## Notes

- Answers come from a hand-picked word list (4-letter ≈ 640, 5-letter ≈ 990, 6-letter ≈ 570). Guesses are checked against a larger dictionary derived from the macOS system word list plus common inflections, so a few obscure words may be accepted and a few valid ones may be missing.
- Custom-word links encode the word in the URL (base64, not encrypted).

## Deploy

Hosted on Vercel:

```bash
vercel deploy --prod --yes
```
