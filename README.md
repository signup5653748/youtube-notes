# YouTube Video Notes — Documentation

A single HTML file (`youtube-notes.html`) that lets you watch YouTube videos and take timestamped notes, with no account or backend needed.

## Hosting (required for mobile)
YouTube embeds need a real `https://` origin — opening the file directly (`file://`) breaks playback on mobile. Host it on GitHub Pages:
1. Put `youtube-notes.html` in a public GitHub repo, renamed to `index.html` (so it loads at the folder root).
2. Repo **Settings → Pages** → set source to your branch → save.
3. Open `https://<your-username>.github.io/<repo-name>/` — not the raw file.

## How it works
- **Home screen**: every video you've added, shown as a thumbnail + title card with a note count. Tap a card to open it.
- **＋ button** (bottom right): paste a YouTube URL (watch, youtu.be, shorts, or live links) to add and open a new video.
- **Inside a video**: tap "➕ Add note at current time" — it reads the exact live timestamp from YouTube's own player, no typing required. Tap any note's timestamp to jump back to that moment.
- **⋮ on a note**: Edit or Delete that note.
- **⋮ on a video card** (home screen): Delete that video and all its notes.
- **⋮ at the top of a video's page**: Copy notes (puts the video's URL + all timestamps/notes on your clipboard as plain text) or Import notes (paste that text back in — on this device or another — to restore it).

## Storage
Everything is saved in the browser's local storage on that device only. Nothing is uploaded anywhere. Use Copy/Import to move notes between devices or make a backup.
