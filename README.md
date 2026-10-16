# MotifMe

A motif and print studio for fashion and surface designers. Think Illustrator's shape tools, Figma's layers, and a LinkedIn-style showcase, built for people who love making prints but don't want a steep learning curve.

## What it does

**Home** · A dashboard that greets you by name and shows your stats. Ask Mofi with one-tap prompt ideas, quick starts (new motif, freehand, palette from a photo, remix), pick up your last project, saved prints, mood board preview, a daily tip and fresh community work.

**01 · Motif Studio**
- Build radially symmetric motifs from layers: petals, leaves, circles, rings, dot rings, scallops, stars, hearts, diamonds, triangles, squares and rays.
- Shape each layer with plain-language dials: repeat count, distance from center, length, fullness, tip shape, rotation, fill, outline and opacity.
- Drag the blue handle on the artboard to resize and rotate a layer directly.
- Freehand draw with live kaleidoscope symmetry (1 to 12 folds, optional mirror).
- Palettes, one-click recolor, and palette extraction from any photo.
- **Ask Mofi:** describe a motif ("indigo block-print marigold") and AI builds an editable layered motif, palette and repeat suggestion. Falls back to an offline keyword generator.
- Mofi style assistant with print-design tips you can apply in one click.
- Undo and redo (Ctrl+Z / Ctrl+Shift+Z). Shortcuts: `V` select, `B` brush.

**02 · Pattern Repeat**
- Layouts: straight, half-drop, brick, mirror, tossed, placement.
- Real-world sizing in inches, with rulers, tile outline, and 150 or 300 dpi output.
- Print size presets: swatch, fat quarter, scarf, yard, wallpaper.
- Grounds: plain, stripe, ticking, gingham, check, polka. Filler motifs between repeats.
- Finishes: flat, linen, paper, silk.

**03 · Mockups**
- Slip dress, boxy tee, tote, pillow, silk scarf and wallpaper, each drawn at true scale so the repeat shows at its real size.

**Mood board** · Upload inspiration, pin your own prints, pull a palette from any pin.

**Community** · Share prints, appreciate others' work, and remix any print into your studio.

**Export** · Motif SVG, transparent PNG, seamless repeat tile JPG, full print at size, and a project JSON.

## Run it

Open `index.html` in a browser. No build step.

Running locally, the app saves to your browser and Ask Mofi uses its offline generator. The live version on claude.ai adds AI generation, account sync, the shared community feed and file downloads.

## Roadmap ideas
- Bézier point editing for custom shapes
- Ogee and diamond repeat layouts
- Colorway variants side by side
- Follow designers and comment threads in Community
- Real backend (auth, storage, image AI) for a standalone launch
