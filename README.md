# 🌌 The Rave Momo - Official Portfolio Website

Welcome to the official, high-fidelity portfolio website codebase for **The Rave Momo**—the iconic Creepypasta Cosplay Raver of the EDM community. 

This website is a professionally designed, single-page interactive application engineered to showcase the artist’s dual nature: **the eerie, thrilling horror cosplay** of the legendary urban myth, and **the pure-hearted, positive PLUR (Peace, Love, Unity, Respect)** community representative.

---

## 🎨 Immersive Features & Interactive UX

1. **Dual-Vibe Transcendence (The Horror/PLUR Toggle):**
   - At the top of the page, visitors can toggle between **"Creepy Mode"** (default) and **"PLUR Mode"**. 
   - Switching modes dynamically morphs the site’s entire aesthetic: fonts, colors, background scanlines, descriptions, and taglines shift seamlessly.
   - **Horror Mode:** Sleek cyber-neon green accents, dark grids, monospace styling, and descriptions detailing their atmospheric performance art.
   - **PLUR Mode:** Dreamy neon pink/violet gradients, rounded sans-serif typography, and descriptions highlighting their community work (e.g., Palisades Wildfire relief), trading kandi, and spreading joy.

2. **Morphing Vector SVG Mask Graphic:**
   - Features a custom vector design of the "Rave Momo" mask. 
   - **Horror Mode:** Pinpoint pupils, glitchy dashed outlines, and a sinister slit smile.
   - **PLUR Mode:** Morphing JavaScript triggers a soft happy curved smile, larger pupils, and a solid glowing contour.

3. **Simulated Cyber Audio Player:**
   - Pre-configured for their official theme track **"THERAVEMOMO"**.
   - Fully interactive play/pause button that activates a live neon visualizer where individual audio frequency bars bounce dynamically.
   - Seekable progress bar allows users to scrub through the track.
   - Collapsible lyrics menu detailing the official track verses.

4. **Integrated Social Grid & Direct Bookings:**
   - Modern, glow-bordered cards linking directly to their verified social handles: **Instagram**, **TikTok**, **SoundCloud**, and **YouTube**.
   - Custom cyber booking form with local validation and a responsive toast alert system that adapts its message/color to the active mode.

---

## 📁 File Structure & Assets

- `index.html` - The complete, self-contained single-page codebase. All CSS styles, vector graphics (SVGs), responsive media queries, and JavaScript animations are embedded directly inside.
- **Why Self-Contained?** 
  - To bypass network-dependency bugs. It ensures that no external CDNs are required, making the site load **instantaneously** with 100% lighthouse performance scores, and making it work perfectly inside offline/sandboxed previews.

---

## 🚀 Deployment Instructions

### Option 1: Quick Hosting (Vercel, Netlify, or GitHub Pages)
Because this is a static single-page application, you can host it for free in seconds:
1. **GitHub Pages:**
   - Create a new repository on GitHub.
   - Upload the `index.html` file.
   - Go to **Settings > Pages**, select the `main` branch, and click Save. Your site is live!
2. **Vercel or Netlify:**
   - Drag and drop the folder containing `index.html` onto [Netlify Drop](https://app.netlify.com/drop) or import the GitHub repo to [Vercel](https://vercel.com).
   - Link a custom domain (e.g., `theravemomo.com`) through their simple DNS settings dashboard.

### Option 2: Connecting Real Audio Streams
To stream their actual SoundCloud audio directly inside the page, you can replace the mockup player with a SoundCloud Embed Widget:
- Go to SoundCloud, click **Share > Embed** on their track.
- Copy the `<iframe>` code.
- Replace the `<div class="audio-player-card">` in `index.html` with the SoundCloud iframe widget, customized with a `#39ff14` (green) or `#ff00aa` (pink) play button color!

---

## 📩 Inquiry & Booking Configuration
The form is currently structured for client-side visual confirmation (displaying custom toast alerts). To connect this form to receive actual emails when managers/ravers submit inquiries, use a free form-backend integration like **Formspree** or **Web3Forms**:
1. Sign up for a free account at [Formspree.io](https://formspree.io/).
2. Create a form and get your unique endpoint URL (e.g., `https://formspree.io/f/xoq...`).
3. Modify the `<form>` tag in `index.html`:
   ```html
   <form class="booking-form" action="YOUR_FORMSPREE_ENDPOINT_URL" method="POST">
   ```
4. Submissions will now be delivered directly to the manager's email inbox!

---

*Curated with Peace, Love, Unity, Respect, and a touch of Horror. 👻🫶🏼*
