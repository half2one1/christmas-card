# 🎄 Cozy Christmas Card

One self-contained page (`index.html`) with a wax-sealed envelope, an animated snowy scene,
handwritten letters and a synthesized music-box *Silent Night* (public domain).
No audio or image files needed. `preview.png` is the image shown in link previews and emails.

## 1. Host it (free, ~1 minute)
Email can't run animation or music, so the card lives on a web page and the email links to it.
- **Netlify Drop**: go to https://app.netlify.com/drop and drag this whole folder in. You get a URL right away.
- or **GitHub Pages**: push the folder to a repo, then Settings → Pages → Deploy from branch.

## 2. Write and send
1. Open your hosted URL. You'll see the **"Write your card"** box. Type your message (Korean, English and emoji all work).
2. **Preview the card** shows exactly what the recipient will see. ✎ brings you back to editing.
3. Send it one of these ways:
   - **Open in Gmail**: opens a new Gmail draft with the link already in it.
   - **Copy for email**: copies a styled block (the preview image plus a red "Open your card ✉" button). Paste it into the body of a new email.
   - **Copy link**: just the link, for any messenger.

Your message is stored in the link after `#`, so it never touches a server.

## Things to tap
| Tap | What happens | Song |
|---|---|---|
| 🛷 Sledding kids | they slide faster, "Wheee!" | Jingle Bells (with sleigh bells) |
| ⛸ Skaters on the pond | they spin, "Wooo!" | Deck the Halls |
| ☃ Snowman | hops and talks | We Wish You a Merry Christmas |
| 🎄 Tree | light pattern changes | Silent Night (music box) |
| 🏠 Cabin | door opens, someone walks out, leaves footprints, waves and goes back in (also happens every ~30–45 s) | |
| 🌙 Moon | northern lights on/off | |
| Sky | notes, low on the left and high on the right | |
| Snow | tap or drag to leave footprints, which new snow slowly fills in | |
| Press & hold | snowstorm (snow piles up much faster) | |
| Top edge of the letter | brush off the snow that has settled on it | |

Snow builds up over time on the ground, the cabin roof, the chimney, the snowman's hat and the letter.
The **song pill** (bottom left) switches between songs; 🔊 mutes.
Move the mouse or tilt the phone for parallax.

## Regenerate the preview image (optional)
Serve the folder (for example `python3 -m http.server`), then run headless Chrome with
`--window-size=1200,630 --screenshot=preview.png http://localhost:8000/index.html?shot`
