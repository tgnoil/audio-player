# 🎵 Audio Player

A compact, dependency-light HTML audio player that automatically organizes your music collection by **album release date**. No backend required.


## 🎵 Music File Naming

**Required format**

YYYY-MM-DD - Artist - Album - Track# - Title.ext


**Example**

2025-01-13 - flat broke - 1111 - 01 - cozumel (ext).mp3


**How it works**

- `2025-01-13` → Album sort date (first track sets album date)
- `flat broke` → Artist
- `1111` → Album name
- `01` → Track number
- `cozumel (ext)` → Song title
- `.mp3` / `.flac` → Supported formats

## 🚀 Quick Setup
1. Save `index.html` as your main page
2. Create a `/music/` folder beside it
3. Add MP3 or FLAC files using the naming convention above
4. Open `index.html` in any modern browser

## ✏️ Customization
Edit the `<style>` in the AudioPlayer constructor or modify:

- `:host { max-width: 500px; }` → Change player width
- `#controls` colors / background
- Button icons or text

## 🛠️ Tech
- Vanilla HTML / CSS / JS (no frameworks)
- [jsmediatags](https://github.com/aadsm/jsmediatags) for metadata
- Shadow DOM for style encapsulation
- Fetch API for directory scanning

---

_Built for dropping new tracks without breaking sort order._
