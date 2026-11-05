# Media files

index.html contains **no embedded media**: every image and the video are plain files in this folder, linked by path.
To change one, overwrite the file and keep the **same name** (nothing else to edit). If you must use another
extension or name, change that one path in `index.html` (search for the old file name).

| File | Where it shows | Size / format | Notes |
|---|---|---|---|
| `video/hero.mp4` | Hero, right-hand panel (always playing, muted, loops) | 1080x1350 (4:5), H.264 `yuv420p`, no audio, ideally under 3 MB | Currently the LUUP. avatar moonwalking (temporary). Must be H.264 MP4 to play everywhere. **Background must be LUUP black `#070707`** (the page colour) or the video shows as a box; H.264 shifts near-black by one level, so check a decoded frame, not just the source. |
| `video/hero-poster.jpg` | Hero panel for the instant before the video starts | 1080x1350 JPG | Use the first frame of the video (same `#070707` background). |
| `img/app-map.png` | "Your crowd will find the bar first time." (row 1) | 1080x2340 PNG (9:19.5, a phone screenshot) | Currently a mock-up. Replace with a real screenshot of the map. |
| `img/app-lineup.png` | "Your crowd will know who's on next." (row 2) | 1080x2340 PNG | Currently a mock-up. Real line-up screenshot. |
| `img/app-news.png` | "Your crowd will hear the news from you." (row 3) | 1080x2340 PNG | Currently a mock-up. Real news/info screenshot. |
| `img/founders.jpg` | "Tech geeks. Festival lovers." block, shown as a 120 px circle | 800x800 JPG, square, faces centred | Placeholder. |
| `img/og-image.jpg` | Link previews (WhatsApp, LinkedIn, iMessage, Slack...) | 1200x630 JPG | Default card (logo + slogan). Swap any time. |
| `img/luup-logo.png` | Header and footer | PNG, off-white on transparent | Only works on dark backgrounds. |

Alt text for the screens and photo lives in `index.html` (PT and EN, keys `r1alt`..`r3alt`, `photoAlt`, `heroAlt`).
