# 🎄 Cozy Christmas Card

One self-contained page (`index.html`) with a wax-sealed envelope, an animated snowy scene,
handwritten letters and a synthesized music-box *Silent Night* (public domain).
No audio or image files needed. The `buddies/` folder has each card buddy as its own SVG, if you want to use them elsewhere (the card has its own built-in copies). `preview.png` is the image shown in link previews and emails.

## 1. Host it (free, ~1 minute)
Email can't run animation or music, so the card lives on a web page and the email links to it.
- **Netlify Drop**: go to https://app.netlify.com/drop and drag this whole folder in. You get a URL right away.
- or **GitHub Pages**: push the folder to a repo, then Settings → Pages → Deploy from branch.

## 2. Write and send
1. Open your hosted URL. You'll see the **"Write your card"** box. Type your message (Korean, English and emoji all work).
   Under the message, **choose a buddy** to live in the card: Mochi the hamster, Bao the dumpling, Pudding the hippo, Biscuit the dog, Mittens the cat or Flurry the snowman. Pick **None** for just the snowy scene (then Santa's presents are for the reader to open).
2. **Preview the card** shows exactly what the recipient will see. ✎ brings you back to editing.
3. Send it one of these ways:
   - **Open in Gmail**: opens a new Gmail draft with the link already in it.
   - **Copy for email**: copies a styled block (the preview image plus a red "Open your card ✉" button). Paste it into the body of a new email.
   - **Copy link**: just the link, for any messenger.

Your message (and the buddy you picked) is stored in the link after `#`, so it never touches a server.

## Things to tap
| Tap | What happens | Song |
|---|---|---|
| 🛷 Sledding kids | they slide faster, "Wheee!" | Jingle Bells (with sleigh bells) |
| ⛸ Skaters on the pond | they spin, "Wooo!" | Deck the Halls |
| 🐹 Your buddy (Mochi the hamster by default) | hops, squeaks and says hi (shivers in a snowstorm, cheers when the sleigh flies by) | |
| Footprints you leave in the snow | your buddy sniffs along and follows them | |
| ☃ Snowman | hops, talks and shakes the snow off its hat | We Wish You a Merry Christmas |
| 🎄 Tree | shakes the snow off its branches, light pattern changes | Silent Night (music box) |
| 🚪 Cabin door | your buddy walks over and goes inside, then looks out of the window (tap the window to say hi, tap the door again to call them out). Leaving footprints that end at the door works too. Half the time a harsh winter storm blows in while they're inside: howling wind, a white-out, and everyone outside shivers | |
| 🏠 Cabin | snow slides off the roof, door opens, someone walks out, leaves footprints, waves and goes back in (also happens every ~30–45 s) | |
| 🌙 Moon | northern lights on/off | |
| 🌲 Pine trees behind the meadow | each one wobbles and drops its snow | |
| 🌠 Shooting star (if you can catch one) | make a wish, and a sleigh flies across the moon right away | |
| 🎁 Presents with a little glow | they're for your buddy, who runs over and opens them (a Santa hat, a jingle bell, sunflower seeds that puff up her cheeks, a cookie or a cozy blanket) | |
| Sky | notes, low on the left and high on the right | |
| Snow | tap or drag to leave footprints, which new snow slowly fills in | |
| Press & hold | snowstorm (snow piles up much faster) | |
| **fold** (on the letter) | the letter folds up into a little note in the corner so the whole scene is free to tap; tap the note (or press Esc) to unfold it | |
| Top edge of the letter | brush off the snow that has settled on it | |

Snow builds up over time on the big tree, the pine trees, the ground, the cabin roof, the chimney, the snowman's hat and the letter.
When the big tree gets heavy it asks for help, and a fully loaded branch sometimes drops a clump by itself.
Every couple of minutes a sleigh flies across the moon and parachutes a present for your buddy down next to the tree.
The **song pill** (bottom left) switches between songs; 🔊 mutes.
Move the mouse or tilt the phone for parallax.

## Regenerate the preview image (optional)
Serve the folder (for example `python3 -m http.server`), then run headless Chrome with
`--window-size=1200,630 --screenshot=preview.png http://localhost:8000/index.html?shot`
