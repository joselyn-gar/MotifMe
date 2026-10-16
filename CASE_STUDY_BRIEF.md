# MotifMe · Case Study Brief

Handoff notes for building a portfolio case study about MotifMe. Hand this file to the portfolio session (repo `joselyn-gar/Joselyn-Garcia`). Screenshots live in `case-study/` in this repo.

## The one-liner
MotifMe is a motif and print studio for fashion designers. I took it from a rough idea to a live, shareable web app in one sitting by vibe coding with Claude.

## Links
- **Repo:** https://github.com/joselyn-gar/MotifMe
- **Live site:** Vercel link pending. Add it here once it's deployed.
- **Claude version (full features, private):** https://claude.ai/artifact/RK1BZvLxf3uF9vrixqpdpi

## The problem
- Surface designers bounce between Illustrator (shapes), Photoshop (repeats), mockup templates and Pinterest (inspiration).
- Those tools are heavy for people who just love making prints.
- Nothing ties motif → repeat → product → community together in one place.

**Who it's for:** fashion and print lovers who aren't technical. Students, hobbyists, early print designers.

**Concept:** LinkedIn × Figma × Adobe Illustrator, built for prints.

## My role
Product designer and creative director. I set the idea, the audience, the features and the visual direction. Claude wrote the code. I steered through feedback, references and screenshots.

## Process (the vibe coding story)
1. **First attempt: Google AI Studio.** The result looked busy and generic, and the tools didn't feel like real print design. (`00-before-ai-studio-home.png`, `00-before-ai-studio-editor.png`)
2. **Briefed Claude like a design partner.** I shared screenshots of the failed build, my logo, and a Pinterest board of the end products I wanted, like block-print florals on stripes. (`00-logo.jpg`, `00-inspiration-moodboard.webp`) I asked it to act as a UI/UX designer with fashion people in mind.
3. **Prototype v1.** A full working studio: motifs, freehand drawing, repeats, mockups, mood board, community and exports.
4. **Feedback round: "make it white and modern."** I gave it my logo. Claude switched to a clean white, monochrome interface with a black wordmark, so the prints carry the color.
5. **Feedback round: "add a dashboard."** We added a home screen that greets the user, suggests prompts and picks up the last project.
6. **Shipping.** We put it on GitHub, fixed it for public visitors (downloads, link previews, cropped mockups) and set it up for Vercel so I can share it on Handshake.

**Key takeaway:** the tool wasn't the difference. The brief was. Clear references (logo, Pinterest board, screenshots of what failed) and plain-language feedback got a far better result.

## What it does
- **Home dashboard:** greeting, stats, Ask Mofi with one-tap prompt ideas, quick starts, continue where you left off, saved prints, a daily tip, fresh community work.
- **01 Motif Studio:** layered radial shapes (petals, leaves, scallops, stars, hearts and more). Plain-language dials like "fullness" and "tip shape" replace technical Bézier controls. Drag handles. Figma-style layers. Palettes, plus palette extraction from a photo.
- **Freehand kaleidoscope:** draw once and it mirrors live, 1 to 12 folds.
- **Ask Mofi (AI):** describe a motif ("indigo block-print marigold") and get an editable, layered motif with a palette and repeat suggestion. Mofi also gives one-click design tips grounded in print craft, like "two-tone discipline" from block printing.
- **02 Pattern Repeat:** straight, half-drop, brick, mirror, tossed and placement layouts. Real inches with rulers and 150/300 dpi. Stripe, ticking, gingham, check and polka grounds. Linen and paper finishes.
- **03 Mockups:** dress, tee, tote, pillow, silk scarf and wallpaper, each drawn at true scale so the repeat shows at real size.
- **Mood board:** upload inspiration and pull palettes from pins.
- **Community:** share prints, appreciate them, remix any print.
- **Export:** motif SVG, transparent PNG, seamless repeat tile, full print at size, project file.

## Design decisions worth highlighting
- **Speak the designer's language.** "Fullness" and "tip shape" in place of "Bézier tension". Real units (inches, dpi, fat quarter, yard) in place of pixels.
- **One flow, numbered:** 01 Motif → 02 Repeat → 03 Mockup. Each screen ends with a button to the next step.
- **White, monochrome UI.** The interface steps back so the prints are the only color on screen. The wordmark matches my logo: bold "Motif", italic "Me".
- **True-scale mockups.** A 4″ tile looks different on a 16″ dress than on a 120″ wall. Most mockup tools ignore that.
- **Opens in a working state.** A sample motif, "Dahlia Block", is loaded so no one faces a blank canvas.
- **Remix culture.** The community is built around remixing, not just likes.

## Tech (keep it light in the case study)
- One HTML file with plain JavaScript, no framework. SVG for motifs, Canvas for repeats.
- Built with Claude. Hosted on GitHub and Vercel.
- The public site saves to the visitor's browser. Accounts and a shared database are possible next steps (Supabase), but on purpose they're not in scope for a vibe coding project.

## Visual assets (`case-study/`)
| File | Use |
|---|---|
| `00-before-ai-studio-home.png`, `00-before-ai-studio-editor.png` | "Before": the AI Studio attempt |
| `00-logo.jpg` | My MotifMe logo |
| `00-inspiration-moodboard.webp` | The Pinterest references I briefed with |
| `01-home-dashboard.png` | Hero image |
| `02-motif-studio.png` | Studio and inspector |
| `03-pattern-repeat.png` | Repeat with rulers and tile outline |
| `04-mockups.png` | True-scale mockups |
| `05-community.png` | Community and starter prints |
| `06-phone-studio.png` | Mobile view |

Desktop shots are 2880×1800 (2× of 1440×900).

## Suggested case study outline
1. Hero: name, one-liner, `01-home-dashboard.png`, a "Try it live" button
2. Overview: role, timeline (one session), tools (Claude, GitHub, Vercel)
3. The problem and who it's for
4. Before and after: AI Studio vs. MotifMe
5. How I vibe coded it: the brief, references, feedback rounds
6. The flow: 01 Motif → 02 Repeat → 03 Mockup, one image each
7. Design decisions
8. What's next: accounts, colorways, more mockups, Bézier editing
9. What I learned about directing AI

## Notes for the portfolio build
- It fits the **Playground** section next to Textiles, Design + Social, JDel and Raised on the Blur. Suggested route: `/playground/motifme`.
- Copy images into `public/images/playground/motifme/`, then run `node scripts/optimize-media.mjs`.
- Voice: short, punchy sentences with some variety. No em dashes. Easy on adjectives and superlatives. A rhetorical question here and there is welcome.
- Don't invent metrics. Real numbers can come later, like views from Handshake.
