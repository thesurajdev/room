# Room

A shared little space to listen to music together, chat live, and set a background — just open the page, no sign-up.

## What it does

- **Listen Together** — load a YouTube playlist and it plays in sync for everyone in the room.
- **Live chat** — real-time messaging with whoever else is in the room.
- **Shared background** — drop in an image, GIF, or video and it shows up for everyone.
- **Shareable link** — join a room and your URL becomes an invite link; anyone who opens it lands straight in the same room.

No accounts, no server, no data stored anywhere — everything runs peer-to-peer in the browser and disappears when both tabs close.

## How to use it

1. Open `hero.html` in a browser (or your hosted link).
2. Tap the chat icon (top right) and enter a room code — anything you like, e.g. `movie-night`.
3. Tap **Join**.
4. Share the link with the other person:
   - Tap **Copy link** in the chat panel, or
   - Just send them your address bar URL — it now includes `?room=your-code`.
5. When they open the link, they're auto-joined and connected to you directly.

## Changing the vibe

- **Music** — paste a YouTube playlist URL into the player bar and hit **Load**. It syncs for the whole room automatically.
- **Background** — tap the image icon (top right) to upload a photo, GIF, or video, or just drag one onto the page on desktop.

## Notes

- Playback and background sync use WebRTC (via [PeerJS](https://peerjs.com/)) — direct peer-to-peer, nothing passes through a server except the initial handshake.
- Large video backgrounds may take a moment to sync to the other person since they're sent in chunks over the data channel.
- Works on desktop and mobile; chat opens fullscreen on small screens.
