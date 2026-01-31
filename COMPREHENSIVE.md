# Experiences - Project Documentation

## Quick Reference for Any Agent

This document contains everything needed to understand and work on the **Experiences** project (the main HEARSAY marketing site). Read this first.

---

## CRITICAL: Naming Convention

To avoid confusion between projects, we use these names:

| Project | Folder | GitHub Repo | Railway | What it is |
|---------|--------|-------------|---------|------------|
| **Experiences** | `/Volumes/T7/experiences` | `Experiences` | Experiences | Main marketing site for all HEARSAY experiences |
| **hearsay** | (separate folder) | `hearsay` | hearsay | THE KNOCK app (the first individual experience) |

**ALWAYS refer to THIS project as "Experiences" in all documentation and conversation.**

The brand name shown to users is still "HEARSAY Experiences" - but internally we call this repo/project "Experiences" to distinguish it from the "hearsay" repo which contains THE KNOCK app.

---

## What is HEARSAY?

HEARSAY is an interactive fiction platform where users have real-time voice conversations with AI-driven fictional characters. This is NOT a chatbot product. This is narrative fiction delivered through dialogue.

**Core concept:** Conversation as fiction. Users speak with fictional characters who listen, respond, remember, and sometimes lie. Each experience places you in a specific scenario with a reason to talk to someone through a constrained frame: a peephole, a mirror, a screen, a window.

**Tagline:** "What you hear depends on who you ask."

---

## Project Structure

**This project (Experiences):**
- GitHub: `https://github.com/chweintr/Experiences.git`
- Domain: `hearsayexperiences.com`
- Purpose: Public marketing/landing site

**THE KNOCK app (separate project):**
- Repo: `hearsay`
- Live URL: `https://web-production-607f7.up.railway.app/`
- Purpose: The actual interactive experience

---

## Creator Information

**Creator:** Caleb Weintraub

**Related ventures:**
- `pastpresence.io` - Container brand for all interactive bot experiences (educational, games, art)
- `hearsayexperiences.com` - This project's domain
- `studioeinfuhlung` - AI film outfit (established presence in film festivals)

**Contact:** calebweintraubstudios.com (for now)

---

## Site Architecture

```
hearsayexperiences.com
├── index.html          (Landing page)
├── the-knock.html      (Live experience)
├── the-chair.html      (Coming soon)
├── the-booth.html      (Coming soon)
├── the-fare.html       (Coming soon)
├── the-trail.html      (Coming soon)
├── the-session.html    (Coming soon)
├── about.html          (Statement, contact)
└── ai.html             (AI use statement)
```

---

## Experience Details

### THE KNOCK (LIVE)
- **Status:** Live
- **URL:** https://web-production-607f7.up.railway.app/
- **Genre:** Mystery, theatre, fiction
- **Frame:** Hotel door peephole
- **Premise:** "Someone is at your door. The owner died six months ago. The official story does not match what people whisper."
- **Aesthetic:** Warm golds, deep reds, brass tones. Damask wallpaper, velvet, worn carpet. Fisheye vignette. Tom Waits meets Grand Budapest meets Delicatessen.

### THE CHAIR (Coming Soon)
- **Genre:** Oral history, slice-of-life
- **Frame:** Barbershop mirror
- **Premise:** "Everyone talks to their barber."
- **Aesthetic:** Warm tungsten, Barbicide blue, chrome, worn leather. Studs Terkel energy.

### THE BOOTH (Coming Soon)
- **Genre:** Intimate drama, guilt, unburdening
- **Frame:** Confession booth lattice
- **Premise:** "Bless me, for I have..."
- **Aesthetic:** Dark wood, candlelight, carved lattice, red velvet. Catholic guilt energy.

### THE FARE (Coming Soon)
- **Genre:** Confessional, thriller-adjacent
- **Frame:** Rearview mirror
- **Premise:** "You picked someone up."
- **Aesthetic:** Night city lights, dashboard edge. NYC taxi confessional meets roadside thriller.

### THE TRAIL (Coming Soon)
- **Genre:** Folklore, cryptid studies, found footage
- **Frame:** Trail camera in woods
- **Premise:** "They know you left the camera."
- **Aesthetic:** Black/white or green night vision, timestamp, infrared glow-eyes. Deadpan creature feature.

### THE SESSION (Coming Soon)
- **Genre:** Philosophy, absurdist comedy
- **Frame:** Altered state / trance
- **Premise:** "Whatever Sammy gave you is kicking in."
- **Aesthetic:** Heat shimmer, faces from static, geometric patterns. Deadpan absurdist meets genuine philosophy.

---

## AI Use Statement (Full Text)

### On Making HEARSAY

I have wanted to build something like this for twenty years. Interactive fiction where the characters actually listen. Conversations that become literature. The problem was always resources. A project like this would have required a team — programmers, voice actors, animators, writers — and funding to support them, and years of development, and people willing to believe in something that didn't exist yet.

I didn't have any of that. So the idea stayed an idea.

Generative AI changed what one person can attempt. Not because it does the work for me, but because it lets me work at a scale I couldn't reach alone. I have spent thousands of hours on this project over the past several months. The codebase runs to around 15,000 lines across frontend, backend, and documentation. The character prompts alone are thousands of words each. This is not prompt-and-accept. This is not a vending machine.

What I actually do: I write, I design, I direct. The models generate raw material — images, sounds, video, dialogue possibilities — and I edit, composite, rework, and reject until the output matches what I'm trying to make. When a character's voice isn't right, I rewrite the constraints and try again. When a generated image is close but wrong, I paint over it, cut it apart, combine it with something else. The iteration is constant.

I think of the models as collaborators, not tools. We consult each other. We debug each other. I praise them when something lands and tease them when it doesn't. This is a working relationship, not a button I press.

The characters in HEARSAY have bounded autonomy. I wrote their voices, their knowledge, their secrets, their relationships. The AI performs within those constraints, improvising in ways I didn't script. That emergence is the point. I am the author of the possibility space. The AI and the user together author each instance.

On the ethics of training data: I know the models learned from work by artists who didn't consent. I don't have a clean answer. What I can say is that this project has not displaced anyone. I would not have hired a team to build this — I couldn't have. Without these tools, HEARSAY would still be an idea I mentioned at parties. The choice was not "human artists or AI." The choice was "this exists or it doesn't."

If the project moves to commercial release, I would replace generated assets with work by human artists and musicians. The generative approach let me build a proof of concept in months instead of years. It is scaffolding. The structure it supports — the characters, the system, the narrative architecture — that is mine.

I am working in a moment when the implications of these tools are unresolved. I have tried to use them thoughtfully. I do not claim to have all the answers. I claim only to have made something that could not exist without both human authorship and machine collaboration, and to have done the work to make it mine.

---

## Design Guidelines

### Landing Page
- Full-viewport looping video background (ethereal vapor with "HEARSAY EXPERIENCES" forming)
- Video: autoplay, muted, loop, with static fallback
- Centered content over video
- Minimal nav: About, AI Statement
- Experience grid: 2x3 or 3x2 responsive

### Typography
- DO NOT use thin, wispy fonts
- Use display serif or distinctive sans-serif with good weight
- Suggestions: Playfair Display, EB Garamond, DM Sans medium weight
- Consider text shadow or blur behind text for contrast against video

### Color (Landing)
- Background: Video provides color (soft whites, iridescent pastels)
- Text: Dark gray (#1a1a1a) or near-black
- Accent: Muted gold or warm highlight
- Avoid pure white text, neon, saturated colors

### What NOT to Do
- Don't make it look like a SaaS product page
- No startup clichés (gradient blobs, "powered by AI" badges)
- No excessive animation or parallax
- No stock photography
- Aesthetic is theatrical and literary, NOT tech-forward

---

## Deployment

- **Platform:** Railway (connected to GitHub)
- **Process:** Push to GitHub, Railway auto-deploys
- **Domain:** hearsayexperiences.com

---

## Technical Stack

Simple static site:
- HTML/CSS/JavaScript
- No framework required
- Optimized for performance (video loading is critical)
- Mobile responsive (static image fallback for video on mobile)

---

## Assets

- `assets/landing-bg.mp4` - Landing page vapor video (~25MB)
- Individual experience teaser assets: TBD (using CSS-generated placeholders for now)

---

## Future Work

- Teaser videos/stills for each experience page
- Email signup integration (Formspree or Buttondown)
- Replace generated assets with human artist work for commercial release
- Corner decorative elements for landing page (user will provide)
