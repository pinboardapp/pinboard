# PinBoard

**Save and back up your Pinterest boards locally.**

Download full-resolution images, GIFs, and videos from your Pinterest boards. Runs entirely on your machine — no proxies, no cloud, no data collection.

→ **[Download for Free](https://github.com/pinboardapp/pinboard/releases/latest)** · [Website](https://pinboard-download.vercel.app) · [FAQ](https://pinboard-download.vercel.app/#faq) · [Report a Bug](https://pinboard-download.vercel.app/#report)

---

## Features

- **Images & GIFs** — Full-resolution originals (JPG, PNG, GIF)
- **Video downloads** — Automatically converts HLS streams to MP4
- **Private boards** — Access your own private boards with session cookies
- **Browse & pick** — Preview every file before downloading, or grab them all at once
- **100% local** — Everything runs on your machine, nothing leaves your computer

## Free vs Pro

| | Free | Pro ($14) |
|---|---|---|
| Images | ✓ (25 per board) | ✓ Unlimited |
| GIFs | — | ✓ |
| Videos | — | ✓ |
| Private boards | — | ✓ |
| Devices | 1 | Up to 3 |

**[Get Pro →](https://pinboard-download.vercel.app/#pricing)**

## Download

### macOS
Download the `.dmg` from the [latest release](https://github.com/pinboardapp/pinboard/releases/latest), open it, and drag PinBoard to your Applications folder.

### Windows
Coming Soon...
<!-- Download the `.exe` installer from the [latest release](https://github.com/pinboardapp/pinboard/releases/latest) and run it. -->

## Quick Start

### Public boards

1. Open a Pinterest board in your browser
2. Open **DevTools** → **Network** tab → scroll the board
3. Find the `BoardFeedResource` request → copy the `board_id` from the URL
4. Enter the **Board ID**, **username**, and **board slug** in PinBoard
5. Hit **Load Board** → download what you need

### Private boards (Pro)

For your own private boards, you'll also need your Pinterest session cookies:

1. Open DevTools → Network → find `BoardFeedResource`
2. Go to Headers → find the `cookie:` header
3. Copy these 4 values: `csrftoken`, `_routing_id`, `_pinterest_sess`, `_b`
4. Paste them into PinBoard's "Private board cookies" section

> **Tip:** Cookies expire when your Pinterest session ends. If downloads stop working, just grab fresh cookies from DevTools.

For detailed steps with screenshots, see the [setup guide](https://pinboard-download.vercel.app/#setup).

## FAQ

**Do I need cookies for public boards?**
No. Just the Board ID, username, and board slug.

**Is my data safe?**
PinBoard runs entirely on your machine. No analytics, no tracking, no data collection. Your cookies and pins never leave your computer.

**Can I use my license on multiple computers?**
Yes — each Pro license works on up to 3 machines.

**How do video downloads work?**
Pinterest serves videos as HLS streams. PinBoard includes bundled ffmpeg that converts them to standard MP4 files automatically.

## Support

- [FAQ](https://pinboard-download.vercel.app/#faq)
- [Report a Bug](https://pinboard-download.vercel.app/#report)

## License

This software is proprietary. See [LICENSE](LICENSE) for details.
