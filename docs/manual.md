# MythaPrism: The Complete User Manual

> **Pictures.** The figures load from https://mythaprism.com/manual_assets/. The illustrated manual is at https://mythaprism.com/manual.html and as a PDF in each release. This Markdown copy is generated from that manual every build, so the two always say the same thing.

**Build 2026-11-17.635 · MythaPrism LLC**

# Start here

From an idea to a file in your slicer in under a minute, on the desktop Tool or on your phone. This chapter is the whole loop, end to end, and the handful of choices that make a first print look great.

## Idea to slicer in under 60 secondspage 7

The fastest MythaPrism print is five moves: pick your filaments, bring in a picture, press Color match, check the preview, export. With the default engine (V1.3) every one of those moves answers in seconds, so the whole trip, from "that would make a great print" to a file open in your slicer, fits comfortably inside a minute. Here is the minute, second by second.

| Time | You do | MythaPrism does |
|---|---|---|
| 0 to 10 s | **Filament library** → tap the spools you own (only the first time: your library is remembered). | Keeps only the filaments you actually have in play, so the match never plans a color you can't print. |
| 10 to 15 s | **Drop in image**, drag a file onto the page, or tap **Take a photo** on the phone. | Loads the picture at a working resolution of 1200 px (1000 px on Free), up to 2160 px on Plus and 4096 px on Pro, and keeps the original for crops and edits. |
| 15 to 25 s | **Color match** (App: **Colors → Color match**). | Picks the color count, chooses filaments, builds the layer stack and draws the **Synthesized result**, the estimate of the finished print. |
| 25 to 40 s | Glance at the preview. Optional: a preset, a nudge of a Prism Modifier, a crop. | Re-matches live as you change things. **Undo** steps back through anything you try. |
| 40 to 50 s | **Export ▾ → .3mf + shareable PDF.** | Writes the `.3mf` with your printer, filament colors, layer heights and every filament change already inside, plus a one-page-per-part print guide. |
| 50 to 60 s | Double-click the `.3mf`. | Bambu Studio or OrcaSlicer opens with the print on the plate, colors assigned, ready to slice. |

Drop in a picture

Color match

Export

![The minute on the desktop: the empty Tool, the matched flowers-on-black painting, and the Export menu.](https://mythaprism.com/manual_assets/m6/t_empty_stage.jpg)
![The minute on the desktop: the empty Tool, the matched flowers-on-black painting, and the Export menu.](https://mythaprism.com/manual_assets/m6/t_view_result.jpg)
![The minute on the desktop: the empty Tool, the matched flowers-on-black painting, and the Export menu.](https://mythaprism.com/manual_assets/m6/t_exportdrop.jpg)

*The minute on the desktop: the empty Tool, the matched flowers-on-black painting, and the Export menu.*

Make the first print a good one

Enable a real spread of filaments, from your darkest to your lightest, a black, a white and a handful of saturated colors cover an enormous range. Leave **Layer height** at **0.08 mm (the default)**: finer layers give the color model more steps. And open the `.3mf` fresh in the slicer (File → Open) rather than importing it into a project that is already open, so the colors come from the file.

Where "seconds" applies

The timings above are for a desktop. Every engine runs on your own device, the zoned and layer-match engines take longer on a busy picture, and an older phone can need about 15 seconds for a complex one.

## The 30-second phone printpage 8

The App is built around the camera. Nothing to transfer, nothing to crop on a computer: the photo you take is the print you make.

1. Open the app, tick the consent box on the launch page, and sign in, or tap **Launch the free tool** for the free monochrome edition.
2. Tap **Take a photo** in the middle of the empty workspace. Your phone's own camera opens, shoot, and the photo lands in the workspace.
3. Tap **Colors**, then **Color match**. The matched preview appears on the stage, swipe left and right to see your photo, the relief bands and the layer schedule.
4. Tap **Export → .3MF + shareable PDF**, then **Share** to send the files to your computer (AirDrop, Files, e-mail) or **Download** to keep them on the phone.

![Shoot, match, share: the camera button, the Colors sheet, the result and the Download-or-Share prompt.](https://mythaprism.com/manual_assets/m6/a_empty_camera.jpg)
![Shoot, match, share: the camera button, the Colors sheet, the result and the Download-or-Share prompt.](https://mythaprism.com/manual_assets/m6/a_sheet_colors.jpg)
![Shoot, match, share: the camera button, the Colors sheet, the result and the Download-or-Share prompt.](https://mythaprism.com/manual_assets/m6/a_result_v25.jpg)
![Shoot, match, share: the camera button, the Colors sheet, the result and the Download-or-Share prompt.](https://mythaprism.com/manual_assets/m6/a_share_prompt.jpg)

*Shoot, match, share: the camera button, the Colors sheet, the result and the Download-or-Share prompt.*

## From the file to the printpage 9

The `.3mf` MythaPrism writes is a complete print job, not just a shape. It names a real printer and process preset (for example *0.08 mm High Quality @BBL H2C*), carries every filament color, places the print in the middle of your bed and, for a relief, lists every filament change at the right layer.

1. **Open the file fresh.** In Bambu Studio or OrcaSlicer use **File → Open** and accept the bundled presets when asked.
2. **Load the spools.** Match each filament slot to the spool in your AMS or multi-material unit. The colors arrive already set, and the Filament change schedule in MythaPrism (and in the PDF) lists them in order.
3. **Slice and compare.** Scrub the slicer's layer slider and compare it with MythaPrism's **Layer schedule** view. The changes should land on the same layers.
4. **Print.** 100 % infill and the slower surface speeds are already set in the process for relief prints. Leave them as they are.

The one mistake almost everyone makes once

If you import the model into a project that is already open, the slicer maps filaments by slot number to whatever that project had loaded, MythaPrism's slot-2 gray prints in your project's slot-2 pink. If the sliced colors look wrong while MythaPrism's preview looks right, open the `.3mf` fresh or line your AMS slots up with the Filament change schedule.

**Single-nozzle printer?** A Relief print only ever has one filament loaded at a time: the export's swap guide tells you exactly which layer to pause on and which spool to load next. The one-stack engines (V1.3 to V1.8 and V2 1.0) are designed for exactly that. The flat modes (Slim, Dual, Hybrid, Focus) place colors side by side within a layer and need a multi-material setup. Every mode card says so before you launch it.

**No 3D printer at all?** You can still make the project. The `.3mf` and the shareable PDF are everything a friend, a makerspace or a print service needs to print it for you, Chapter 10 explains how, including ordering many copies at once.

02

# How MythaPrism works

Three ideas explain every control in the product: a color is a height, every filament lets through a different amount of light, and every print is one of six kinds of physical object.

## A color is a heightpage 12

A relief print has a few dozen printable heights. Each height produces exactly one color: the color light makes as it travels down through every filament layer stacked at that point and back out again. Put those heights in order from the plate up and you have the print's real, achievable gradient. The palette your particular stack of spools can produce.

Matching is the job of giving each point of your picture the height whose color is closest. A bright highlight goes to a tall column capped with a light filament. A deep shadow goes to a short column where the dark base shows through. The **Relief bands** view shows those heights as a gray map (brighter = taller), and the **Prism control** card (with the print’s total height and layer count at its top) draws the gradient itself. You can drag its handles to decide by hand where one filament gives way to the next.

Synthesized result

Relief bands

3D

![The same print three ways: the synthesized result, the relief-band height map and a 3D view of the plastic.](https://mythaprism.com/manual_assets/m6/t_view_result.jpg)
![The same print three ways: the synthesized result, the relief-band height map and a 3D view of the plastic.](https://mythaprism.com/manual_assets/m6/t_view_height.jpg)
![The same print three ways: the synthesized result, the relief-band height map and a 3D view of the plastic.](https://mythaprism.com/manual_assets/m6/t_3d_stage.jpg)

*The same print three ways: the synthesized result, the relief-band height map and a 3D view of the plastic.*

The smarter engines go further. The **zoned** engines (the V25 family) split the picture into up to twenty color zones and give each zone its own stack, so a face, a sky and a shirt each get the filaments that suit them. The one-stack engines (V1.3 to V1.8, V2 1.0) do the opposite: every layer is one filament across the whole plate, which is exactly what a single-nozzle printer with pauses wants. Chapter 5 explains all the families.

## Light, filament and LDpage 12

Every filament in the library carries an **LD, Light Depth** figure in millimeters: MythaPrism's own number for how far light travels into that plastic before it is mostly absorbed. (LD is MythaPrism's measure, and it is not the "TD" figure other tools publish, and the two are not interchangeable.) Black PLA stops light within a fraction of a millimeter, a good white lets it through for several. That number is why two filaments with the same swatch color print differently, and it is what the preview is computed from.

**Black is the exception.** One 0.08 mm layer of black hides everything under it in normal light, so black carries an LD of 0.02 mm and every color matcher treats it that way: black can sit *under* other colors to darken them (black under yellow prints olive), or print as black on its own, but black over white is black, never gray. It is the one filament where a single thin layer is enough to cover, the other blacks you add from the catalog follow the same rule.

Library colors for Bambu Lab filaments are Bambu's own published color codes (from Bambu Studio's color-code file), Black and Jade White show their printed look rather than pure #000000 and #FFFFFF. Colors for the other brands in the catalog are approximate, because those makers publish no color codes. Check them against your spool or calibrate. LD values are marked **typ** (typical) or **est** (estimated from the color). They are good enough for a great first print. For the closest match, print MythaPrism's **calibration plate** once and photograph it: the Tool measures how your own spools behave over white and over black, and every engine composites with those measurements instead (Chapter 9).

## The six Prism modes, and 2D image editingpage 13

Everything MythaPrism prints is one of six kinds of object, the **first** place in the mode bar (the top row of the App’s Modes sheet), **2D image editing**, works on the picture alone, and it opens by itself when you add a picture, so you can edit before you color match. The **mode pill** above the stage (Tool) or the **Modes** sheet (App) switches between them. Tapping a mode opens its card, which says what it builds and what your printer needs, and **Launch** switches the print.

| Mode | What it is | Best for | Printer |
|---|---|---|---|
| **Relief Prism** (default) | A sculpted tonal relief: translucent layers stack and thickness paints the image. Back-lit, it glows. | Portraits, photos, landscapes | Any printer: swaps at set heights, or an AMS |
| **Slim Prism** | One picture printed as flat color parts with a glass-smooth face: thin, fast, no swap schedule. | Posters, signs, logos, bookmarks, coasters | Multi-material (AMS) |
| **Dual Prism** | Two flat pictures, one on each face, joined by a thin transition layer. | Keychains, ornaments, two-sided cards | Multi-material |
| **Hybrid Prism** | Your picture as a full relief on top, a second picture as a flat bed underneath. | A sculpted front with a poster back | Multi-material |
| **Focus Prism** | One picture split by who is in it: the background prints flat, the subject rises in relief. | People and pets over a scene | Multi-material |
| **LithoPrism** | A full-color lithophane: hold it to a light and the picture glows in color. | Window pieces, night-lights, back-lit frames | Any printer, or an AMS |
| **2D image editing** | Not a print: the workspace locks to the picture, every edit lands on it, and the print waits until you go back to a Prism mode. | Photo edits, Filters looks, cut-outs from Cut out pieces | , (nothing to print) |

Relief Prism

Slim Prism

Dual Prism

Hybrid Prism

![Four of the modes: Relief (the flowers on black, V25), Slim (the U.S. flag, V1.8 obj), Dual (the flowers on the front on](https://mythaprism.com/manual_assets/m6/t_mode_relief.jpg)
![Four of the modes: Relief (the flowers on black, V25), Slim (the U.S. flag, V1.8 obj), Dual (the flowers on the front on](https://mythaprism.com/manual_assets/m6/t_mode_slim.jpg)
![Four of the modes: Relief (the flowers on black, V25), Slim (the U.S. flag, V1.8 obj), Dual (the flowers on the front on](https://mythaprism.com/manual_assets/m6/t_mode_dual.jpg)
![Four of the modes: Relief (the flowers on black, V25), Slim (the U.S. flag, V1.8 obj), Dual (the flowers on the front on](https://mythaprism.com/manual_assets/m6/t_mode_hybrid.jpg)

*Four of the modes: Relief (the flowers on black, V25), Slim (the U.S. flag, V1.8 obj), Dual (the flowers on the front on Zoned V1.8 obj, the flag on the back on V1.8 obj) and Hybrid (Earth raised as the relief top on Zoned V1.8 obj, over the flag printed flat as the bed on V1.8 obj).*

## Where things livepage 14

The Tool and the App carry the same controls in different places. This table is the map, Chapter 4 tours the Tool and Chapter 11 tours the App.

| You want to… | Tool | App |
|---|---|---|
| Choose your filaments | Header → **Filament library** | **Colors** sheet → Your filaments |
| Bring in a picture | **Drop in image**, or drag a file onto the page | **Take a photo**, or the **Photo** sheet |
| Pick an engine | **Color match ▾** | **Colors** sheet → engine rail → **Color match** |
| Change the print mode | Mode pill above the stage | **Modes** sheet |
| Printer, size, layer height | **Print setup** (left column) | **Export** sheet → Print setup |
| Dither and surface options | **Print setup** (left column) | **Edit** sheet → Processing |
| Edit the picture | **✎ Edit ▾** on the stage | **Edit** sheet → Edit tools |
| Puzzle cut · Multi crop · Filters · Image Simplifier · Image Grading · Mural · Reassign bands | **Add-ons** (left column) | **Edit** sheet → Add-ons |
| Tune tones and colors | **Prism Modifiers** (right column) | **Tune** sheet |
| See the stack and the schedule | **Prism control** · **Filament change schedule** | **Colors** sheet · **Export** sheet → stats |
| Export and save | **Export ▾** · **Save ▾** | **Export** sheet |
| Account, settings, plans | Person icon (top right) | Person icon (top right) |

03

# Photo editing

Every picture you drop into MythaPrism opens as a photo first, with no color match yet. Crop it to any shape, cut out the subject, put it in front of a new background, add a title, grade it with the Prism Modifiers, and save the result as a PNG. You can stop there with a finished picture, or carry every edit into a 3D print.

## A photo editor that also printspage 16

When a picture arrives, MythaPrism doesn't start matching. It waits in **Edit Prime** mode: the Edit menu reads **✎ Edit Prime ▾**, the **Prism Modifiers** card opens, and the **Prime** view shows your photo with every edit and slider applied, live. The **Color match** button pulses a rainbow outline to show the next step is yours. Nothing is planned or printed until you pick a matcher, so you can treat MythaPrism as a photo editor for as long as you like. After a match the Prime view keeps showing the edited photo (filters included). Press and hold the small rainbow **Hold to see original** icon at the bottom left of the picture (its name shows when you point at it, or while you hold it in the App) to compare with the untouched upload (in Dual, Hybrid and Focus each picture shows its own original on its own side). All of it runs on your device: once the Tool or the App is open, photo editing needs no internet connection, and your photos never leave the device.

Everything on this page works on the photo itself:

| You want to… | Use | What lands in the picture |
|---|---|---|
| Frame it, or cut it to a shape | **⬚ Crop** | A new frame or a shaped edge: circle, heart, star, hexagon and more. Outside the shape becomes transparent. |
| Lift the subject off its background | **⧉ Cut out pieces** | The background removed. The cut area is transparent. |
| Swap the background | **▦ Background editor** | A solid color, or another photo behind your subject. |
| Paint an area one color | **◉ Spot color** | The selected area filled with the color you pick. |
| Put words on it | **T Add text** | Text painted in the color you pick: Bold, Mono or Sans, rotated however you like. |
| Add a logo or a QR code | **▣ Add image** | A second picture stamped on top, where you place it. |
| Cut openings | **⌫ Hole punch** | Transparent shapes: circles, stars, hearts, pills, or any outline you draw. |
| Grade the color | **Prism Modifiers** | Exposure, contrast, white balance, vibrance, hue, vignette and more. |
| Turn it into a negative or remix its colors | **◐ Invert · ⟳ Rotate · ⇅ Reverse · 🎲 Randomize** | A photo negative, hue rotations, swapped light and dark. |
| Keep the result | **Save ▾ → Save edited prime image (.png)** | A PNG with every edit and slider baked in. Transparency is kept. |

The photo

New background

Graded

Title added

The saved PNG

![One photo, start to finish, before any color match: (a) the Moon (NASA), cut out with Cut out pieces, (b) Earth’s clouds](https://mythaprism.com/manual_assets/m6/ph_story_0.jpg)
![One photo, start to finish, before any color match: (a) the Moon (NASA), cut out with Cut out pieces, (b) Earth’s clouds](https://mythaprism.com/manual_assets/m6/ph_story_2_bg.jpg)
![One photo, start to finish, before any color match: (a) the Moon (NASA), cut out with Cut out pieces, (b) Earth’s clouds](https://mythaprism.com/manual_assets/m6/ph_story_3_grade.jpg)
![One photo, start to finish, before any color match: (a) the Moon (NASA), cut out with Cut out pieces, (b) Earth’s clouds](https://mythaprism.com/manual_assets/m6/ph_story_4_text.jpg)
![One photo, start to finish, before any color match: (a) the Moon (NASA), cut out with Cut out pieces, (b) Earth’s clouds](https://mythaprism.com/manual_assets/m6/ph_saved_edited_prime.jpg)

*One photo, start to finish, before any color match: (a) the Moon (NASA), cut out with Cut out pieces, (b) Earth’s clouds seen from orbit set behind it (Background editor → Add background behind cut-out), (c) a warmer, punchier grade with a vignette (Prism Modifiers), (d) a title added with Add text, and (e) the PNG that Save edited prime image wrote.*

## The Edit Prime workspacepage 17

![The Tool in Edit Prime mode: the edited, graded photo on the Prime view, the Prism Modifiers card open on the right, and](https://mythaprism.com/manual_assets/m6/ph_workspace.jpg)

*The Tool in Edit Prime mode: the edited, graded photo on the Prime view, the Prism Modifiers card open on the right, and the Edit Prime pill on the stage. No color match has run yet.*

The stage shows the photo at full size: zoom with the wheel or the ＋ / − buttons, drag to pan (in every edit tool the wheel zooms toward the cursor and the picture never slides off its frame), and **⤢** to fit. The **↶ / ↷** buttons above the zoom column (or **Ctrl + Z**, **Ctrl + Shift + Z**) step back and forward through your last changes (10 steps on Free and Plus, 25 on Pro) whether that was a tool's **Apply**, a slider, a crop or a new background. **⊞ Grid S M L** lays a real-millimeter grid over the photo to help you line things up, and it never appears in the saved picture.

**Working resolution** (the first slider in Prism Modifiers) sets how many pixels you edit and save: a new picture starts at 1200 px on the long side (or its own size when it is smaller), Free stays at 1000 px or less, Plus goes up to 2160 px and Pro up to 4096 px. The picture's size in pixels shows under the slider while you drag. Going above the picture's own size enlarges it with MythaPrism's own upscaler, which follows the edges in the picture so lines stay sharp. A bigger working resolution means more detail and slower matching, so 1200 px suits most prints. Changing it reloads the picture from the original at the new size and clears your edits and slider values, so **set it first, then edit.** The zoom and position stay where they were.

Edit first, then match

Make your photo edits before you pick a color matcher. Once a match exists, the same tools start working on the print instead of the photo. A spot color becomes a filament region and text becomes a printed feature. Neither is painted into the photo any more. Everything you did before the match carries into it unchanged.

## The edit tools on a photopage 18

![The Edit Prime menu: the tools that work on a plain photo.](https://mythaprism.com/manual_assets/m6/ph_editmenu.jpg)

*The Edit Prime menu: the tools that work on a plain photo.*

Open **✎ Edit Prime ▾** on the stage. Each tool opens as a large page: the photo on the left, its controls on the right. **Apply** keeps the page open, so you can stack several edits before you close it.

The selection tools are shared: **Tolerance** for auto-detect, **🪣 Fill subject by click**, the three outline tools: **Points**, **Freehand** (one stroke, released to close) and **⌁ Snapper** (each line snaps to the nearest color edge), and the **Brush** (below). The **Smooth lasso** and **Blend lasso** are in the menu too and work on the photo itself. The tools that need a print (**Multi crop**, **Reassign bands**, **Dual backing** and braille text) appear once a match exists.

![The Background editor with the space around the cut-out Moon selected, placing Earth’s clouds behind it, the Add text pa](https://mythaprism.com/manual_assets/m6/ph_tool_bg.jpg)
![The Background editor with the space around the cut-out Moon selected, placing Earth’s clouds behind it, the Add text pa](https://mythaprism.com/manual_assets/m6/ph_tool_bgplace.jpg)
![The Background editor with the space around the cut-out Moon selected, placing Earth’s clouds behind it, the Add text pa](https://mythaprism.com/manual_assets/m6/ph_tool_text.jpg)
![The Background editor with the space around the cut-out Moon selected, placing Earth’s clouds behind it, the Add text pa](https://mythaprism.com/manual_assets/m6/ph_tool_crop.jpg)

*The Background editor with the space around the cut-out Moon selected, placing Earth’s clouds behind it, the Add text page with the title placed, and Crop with the heart shape selected, on Earth.*

### The selection brushpage 19

![The Spot Color window with the Brush, here on the synthesized print: a fine tip tracing the stripes, a thicker tip for a](https://mythaprism.com/manual_assets/m6/ph_tool_brush.jpg)
![The Spot Color window with the Brush, here on the synthesized print: a fine tip tracing the stripes, a thicker tip for a](https://mythaprism.com/manual_assets/m6/ph_brush_row.jpg)

*The Spot Color window with the Brush, here on the synthesized print: a fine tip tracing the stripes, a thicker tip for a broad patch, and the ring that shows the tip under the pointer, the Brush controls under Points, Freehand and Snapper.*

The side panel of every tool folds into numbered sections with a chevron (Select with, Brush, Spot color, Palette, Aspect, Shapes and so on). Tap a section’s name to open or close it. The panel remembers what you left open.

Under Points, Freehand and Snapper, every tool with a selection has a **Brush** row: **🖌 Brush** paints the highlighted selection, **⌫ Erase** takes it away, **↶ Undo stroke** steps back one stroke, and **Size** sets the tip from 1 px to 120 px. The size is measured on the screen, so zoom into the picture (wheel, or ＋) and the same tip covers fewer pixels. That is how you select one eyelash or one letter. A ring shows the tip under the pointer. Brush and erase work with Tolerance and Fill: auto-detect a background, then brush in what it missed and erase what it took by mistake. The brush is in Cut out pieces, the Background editor, Spot color (on the photo before a match and on the synthesized print after one), Crop's selection and the Hole punch, on a phone, paint with one finger (a second finger cancels the stroke).

**⬚ Crop.** Drag the picture under the frame, zoom it, then **Crop**. The presets set a print size at the same time (**200 × 200**, **Bookmark 50 × 150**, **Card 85.6 × 54**, **3:4**, **4:3**, **16:9**, **Free**). **Shapes** cuts the picture itself to a circle, square, triangle, semicircle, trapezoid, diamond, pentagon, hexagon, octagon, star, pill or heart, and **Rounded corners** softens a rectangle. Two fingers rotate the picture under the frame on a touch screen. Turn on **Let the frame go past the picture** in **New border** (it is off by default, so a corner pulled a little too far never jumps the frame). Then pull an edge of the frame past the picture to make the picture bigger, and choose in **New border** how the new border is filled: the picture’s **Edge colors**, or **One color** you pick (a black frame, for example). Until you pull past the picture, nothing is added around it. **Recrop** keeps the whole picture and puts it on a background of the size you pick (1920 × 1080, 1080 × 1920, 1080 × 1080, 4:3, 3:4, 3:2, 2:3, Bookmark or Card), in one color (black to start with) or the picture’s edge colors, so nothing is cut away.

**⧉ Cut out pieces, step 1.** The highlighted area is what MythaPrism thinks is background. Adjust **Tolerance**, click the subject with **Fill subject**, or trace it with Points, Freehand or the Snapper, then **Cut out. Remove background**. **Restore background** puts it back.

**▦ Background editor.** Select the background the same way, then **Apply color** for a solid backdrop, or **Use image** to put another photo behind the subject. The new photo fills the frame. You drag, scale and (on a touch screen) twist the subject into place, then **Apply placement**. **Add background behind cut-out** puts a photo behind a subject you have already cut out.

**◉ Spot color.** Click an area to flood-select it (more clicks add to it), trace it, or brush it, then pick a color and **Apply spot color**. On a photo the area is painted that color. The eyedropper samples a color from the picture itself. **Remove all spot colors** puts the photo back as it was under every spot you painted (after a crop the paint is part of the photo, and use Undo then).

**T Add text.** Up to three texts at a time. Type, choose **Bold**, **Mono** or **Sans**, and pick a color. Drag to move, pull the square handle to resize and the round handle to rotate, or pinch and twist with two fingers. **Apply texts** paints the words into the photo.

**▣ Add image.** Places a second picture on top: a logo, a signature, a QR code. Drag and scale it, rotate it with two fingers on a phone, then **Place image**.

**⌫ Hole punch.** Pick a shape and drag it into place, or **Draw** around any area. The red area becomes transparent.

**↺ Revert all edits** brings back the untouched photo, after a confirmation, and can itself be undone.

The colors for text and spot color come from your **filament library**: the 33 preset colors plus any you add. To use an exact brand color, add it to the library first with **Add filament** and the color square (Chapter 4, *The Filament library*).

Cut out

Heart crop

![Two edits that change the picture's outline: the cut-out from Cut out pieces, and Crop → Shapes → Heart. The checkerboar](https://mythaprism.com/manual_assets/m6/ph_story_1_cut.jpg)
![Two edits that change the picture's outline: the cut-out from Cut out pieces, and Crop → Shapes → Heart. The checkerboar](https://mythaprism.com/manual_assets/m6/ph_crop_heart.jpg)

*Two edits that change the picture's outline: the cut-out from Cut out pieces, and Crop → Shapes → Heart. The checkerboard is transparency, and the saved PNG keeps it.*

## Prism Modifiers on a photo

The **Prism Modifiers** card grades the photo in the Prime view as you drag. Every slider sits at **0** when it is neutral, most run from −100 to +100.

None

Brightness

Contrast

Vibrance

Warm

Cool

![](https://mythaprism.com/manual_assets/m6/ph_mod_none.jpg)
![](https://mythaprism.com/manual_assets/m6/ph_mod_bright.jpg)
![](https://mythaprism.com/manual_assets/m6/ph_mod_contrast.jpg)
![](https://mythaprism.com/manual_assets/m6/ph_mod_vib.jpg)
![](https://mythaprism.com/manual_assets/m6/ph_mod_warm.jpg)
![](https://mythaprism.com/manual_assets/m6/ph_mod_cool.jpg)

Saturation +100

Hue

Vignette

Shadows

Tint

Midtones

![One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balanc](https://mythaprism.com/manual_assets/m6/ph_mod_sat.jpg)
![One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balanc](https://mythaprism.com/manual_assets/m6/ph_mod_hue.jpg)
![One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balanc](https://mythaprism.com/manual_assets/m6/ph_mod_vig.jpg)
![One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balanc](https://mythaprism.com/manual_assets/m6/ph_mod_shad.jpg)
![One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balanc](https://mythaprism.com/manual_assets/m6/ph_mod_tint.jpg)
![One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balanc](https://mythaprism.com/manual_assets/m6/ph_mod_mid.jpg)

*One photo, one slider each, saved as edited prime images: none, Brightness +45, Contrast +60, Vibrance +80, White balance +60 (warm), White balance −60 (cool), Saturation +100, Hue +55, Vignette +80, Shadows +70, Tint +60 and Midtones −50.*

![The Prism Modifiers card in Edit Prime: every slider with its value box and 🔒 lock, and the buttons underneath.](https://mythaprism.com/manual_assets/m6/ph_modcard2.jpg)

*The Prism Modifiers card in Edit Prime: every slider with its value box and 🔒 lock, and the buttons underneath.*

| Slider | What it does to the photo |
|---|---|
| **Tone** | Shifts the whole picture darker or lighter. |
| **Brightness** | Exposure: darker or brighter. |
| **Contrast** | Softer or punchier. |
| **Midtones** | Lowers or lifts only the middle tones. |
| **Highlights · Shadows** | Darkens or brightens only the bright areas, or only the dark ones. |
| **Vibrance** | Boosts muted colors and leaves already-strong ones alone. |
| **Saturation** | All color, evenly. −100 is black and white. |
| **Hue** | Rotates every color around the color wheel. |
| **White balance · Tint** | Cooler or warmer, greener or more magenta. |
| **Vignette** | Darkens (+) or lightens (−) toward the edges. |
| **Skin tones** | Deepens skin toward olive and rich brown, or lightens it toward fair. |
| **Gradients** | Breaks up banding in skies and smooth fades. |

The box beside each slider shows its value. **Sharpness**, **Clarity**, **De-Blotch**, **Skin tones** and **Gradients** show on the photo in 2D image editing (the mode every new picture opens in) and shape the 3D print when you color match. The **Island smoother** merges the print's small specks, so it works on the print only: it is grayed out in 2D image editing and before the first color match.

## The modifier buttonspage 22

Invert

Rotate ×3

Reverse

Randomize

![The color-mixing buttons on the same photo: (a) Invert colors, (b) Rotate colors pressed three times (90° round the whee](https://mythaprism.com/manual_assets/m6/ph_btn_invert.jpg)
![The color-mixing buttons on the same photo: (a) Invert colors, (b) Rotate colors pressed three times (90° round the whee](https://mythaprism.com/manual_assets/m6/ph_btn_rotate.jpg)
![The color-mixing buttons on the same photo: (a) Invert colors, (b) Rotate colors pressed three times (90° round the whee](https://mythaprism.com/manual_assets/m6/ph_btn_reverse.jpg)
![The color-mixing buttons on the same photo: (a) Invert colors, (b) Rotate colors pressed three times (90° round the whee](https://mythaprism.com/manual_assets/m6/ph_btn_shuffle.jpg)

*The color-mixing buttons on the same photo: (a) Invert colors, (b) Rotate colors pressed three times (90° round the wheel), (c) Reverse (light and dark swap, hues kept), and (d) Randomize (a new hue deal).*

Under the sliders:

- **🎲 Randomize modifiers** deals a new, moderate set of values to every grading slider except Hue. It's a quick way to try looks: press it until one fits, then fine-tune.
- **↺ Reset modifiers** returns every slider to 0.
- **🔒** beside a slider locks it, so Randomize and Reset leave it alone. Lock the White balance you like, then randomize everything else.
- **◐ Invert colors** turns the photo into a negative. Press it again to turn it back.
- **⟳ Rotate colors** walks every hue 30° around the color wheel per press. Twelve presses bring it home.
- **⇅ Reverse** swaps light and dark and keeps the hues.
- **🎲 Randomize stack** deals the photo a new hue rotation at random.

**Randomize stack + filaments** needs a matched print. After a match, Invert, Rotate, Reverse and Randomize act on the print's filament stack instead (Chapter 5).

## Filters and Cut out pieces: restyle and split the photopage 23

**Filters** (in Add-ons) puts any of **310 looks** on the photo (flat color fills, cartoon, line art and ink, pencil, halftone, pixel art, neon, blueprint, cosmic, old photo processes, crafts, film grades and more) and shows every one of them on your own photo at once, with Effect, Strength and a before-and-after Compare slider. **Image Grading** (Plus and Pro) grades the photo’s color and light: 53 quick looks, white balance, light, detail and haze, a color mixer, color grading, effects and your own .cube LUT (3D and 1D tables, with or without a shaper, up to 400 MB, read on your device). The **Original** card, first in every group, brings the photo back. **⧉ Cut out pieces** (in the Edit menu) cuts the subject out or splits the photo into pieces (auto, gap, obj, tones, relief or brightness), lets you merge them, put a look on only the pieces you pick, save them as PNGs, a .zip or a layered .psd, and send just those pieces back to the workspace. Apply either before a match and the result is simply part of your edited photo: save it as a PNG, keep editing, or carry it into a print. Undo takes it back. To work on the photo with no print in the way at all, use **2D image editing** in the mode bar (Chapter 7). Chapter 8 covers the add-ons and Chapter 6 covers Cut out pieces. Plus and Pro. Effect, Strength and Compare sit in three equal pills under the picture, next to Compare, and the two see-through arrows on the left and right of the picture (or the arrow keys) step to the previous or next look.

## Saving your picturepage 24

![The Save menu. Save edited prime image writes the photo with every edit and slider applied.](https://mythaprism.com/manual_assets/m6/ph_savemenu.jpg)

*The Save menu. Save edited prime image writes the photo with every edit and slider applied.*

**Save ▾ → Save edited prime image (.png)** writes the photo exactly as the Prime view shows it: every crop, cut-out, background, painted color, text, stamped image and hole, with every Prism Modifier baked in. The file is a **PNG** at your working resolution and keeps its **transparency**, so a cut-out subject or a heart-shaped crop stays see-through. It's named after your picture, ending in `_edited_prime.png`.

The option is there before and after a color match, and it always saves the photo, not the print preview. **Save synthesized image (.png)** saves the print preview instead. **Save project (.mpsm)** keeps everything, edits and slider values included, so you can reopen it and keep editing on the Tool or the App (Chapter 11).

## From photo to printpage 24

When the picture looks right, open **Color match ▾** and pick a matcher. Everything you did carries over: the crop sets the print's outline, transparent areas print as nothing, and the Prism Modifier values stay live, so you can keep grading after the match while the print updates. Chapter 5 covers matching. Chapter 6 covers the tools once a print exists.

## Photo editing on the phonepage 25

![The App with a photo just dropped in, the Edit sheet and the Tune sheet in Prematch 2D editing mode, and the same photo ](https://mythaprism.com/manual_assets/m6/ph_app_photo.jpg)
![The App with a photo just dropped in, the Edit sheet and the Tune sheet in Prematch 2D editing mode, and the same photo ](https://mythaprism.com/manual_assets/m6/ph_app_edit.jpg)
![The App with a photo just dropped in, the Edit sheet and the Tune sheet in Prematch 2D editing mode, and the same photo ](https://mythaprism.com/manual_assets/m6/ph_app_tune.jpg)
![The App with a photo just dropped in, the Edit sheet and the Tune sheet in Prematch 2D editing mode, and the same photo ](https://mythaprism.com/manual_assets/m6/ph_app_graded.jpg)

*The App with a photo just dropped in, the Edit sheet and the Tune sheet in Prematch 2D editing mode, and the same photo with a cooler white balance, more vibrance and contrast, and a vignette.*

On the phone, a picture you take or drop in opens the same way. The **Edit** and **Tune** sheets show a **Prematch 2D editing mode** banner. In Edit, Cut out pieces, Background editor, Crop, Spot color, Add text, Add image, Hole punch and Revert all work on the photo. In Tune, Tone, Brightness, Contrast, Midtones, Highlights, Shadows, Vibrance, Saturation, White balance, Tint, Hue and Vignette work, plus the color-mixing buttons. Controls that only shape a print are grayed out until you match. Tap a slider and it drops onto the picture so you see the change live. Inside the tools, one finger drags whatever you placed and two fingers resize and rotate it. **Export → Save edited prime image** saves the PNG to your phone, and **Share** sends it anywhere.

## What each plan can dopage 26

|  | Free | Plus | Pro |
|---|---|---|---|
| Edit tools on a photo | Crop · Revert | Every tool listed above, with the Brush | Every tool listed above, with the Brush |
| Prism Modifiers | Tone · Brightness · Contrast | Every slider | Every slider |
| Invert · Rotate · Reverse · Randomize stack | - | - | ✓ |
| Save edited prime image (.png) | - | ✓ | ✓ |
| Working resolution | up to 1000 px | up to 2160 px | up to 4096 px |
| Undo / redo history | 10 steps | 10 steps | 25 steps |
| Works offline (on your device) | ✓ | ✓ | ✓ |

What MythaPrism's photo editing is built for

MythaPrism is built to get a picture ready (framed, cut out, cleaned up, titled and graded) whether it ends up on a screen or as a 3D print. Each edit is applied straight to the picture: there is no stack of separate image layers you can hide or rearrange later, so use Undo (10 steps, 25 on Pro) or Revert all edits to step back. It doesn't develop camera RAW files, and it edits and saves at your working resolution (up to 1000 px on the long side on Free, 2160 px on Plus and 4096 px on Pro). For full-resolution retouching, use your usual editor first, then drop the result into MythaPrism.

04

# The Tool, button by button

The desktop Tool runs in any modern browser. Three columns and a stage: the left column sets up the physical print, the stage shows and edits it, and the right column measures and tunes it. This chapter names every control on screen.

## The whole screenpage 28

![The Tool after a V25 match of the flowers-on-black painting: the header across the top, Print setup and Add-ons on the l](https://mythaprism.com/manual_assets/m6/t_hero_flowers_v25.jpg)

*The Tool after a V25 match of the flowers-on-black painting: the header across the top, Print setup and Add-ons on the left, the stage in the middle, Stats, Prism Modifiers and Engine settings on the right.*

**Section headers.** Every card in the side columns (Print setup, Add-ons, Swap order, Stats for nerds, Prism Modifiers, Prism control, Filament change schedule) has a pill header. Click it to fold the card away. Click again to bring it back. The long cards open as a **peek window**: the first rows show, the bottom fades out and a **More ▾** line sits underneath, so the cards below stay on the first screen. The peek window scrolls on its own. **More ▾** grows the card to its full height and becomes **Less ▴**. Stats for nerds is always open when the Tool loads.

## The header barpage 28

![The header: logo, Start here, the Filament library counter, Drop in image, Color match, Save, Export and the account ico](https://mythaprism.com/manual_assets/m6/t_header.jpg)

*The header: logo, Start here, the Filament library counter, Drop in image, Color match, Save, Export and the account icon.*

| Control | What it does |
|---|---|
| **Start here →** | A signpost pointing at the Filament library, the first thing to open on a new device. |
| **Filament library n / 33** | Opens the library. The counter shows enabled filaments / filaments in your library. |
| **Drop in image** | Opens the file picker. You can also drag a file anywhere onto the page, or click *Drop in* on the empty stage. Saved `.mpsm` projects (and older `.mythaprism`, `.sculptraprism` and `.sculptra` files) open the same way. **Save ▾ → Open project (.mpsm)** does the same from the menu. |
| **Color match · V25 ▾** | The engine menu: every engine, in tabs. The button names the engine in use, choosing one re-matches at once (Chapter 5). In the two-picture modes it becomes two buttons, a blue one for Image 1 and a green one for Image 2. On a narrow window they shorten to **Match · V1.3** and then to just the engine (**V1.3**, with the full name when you point at it), and *Start here* steps aside so the header stays on one line. |
| **Save ▾** | Save the edited picture, the synthesized preview, the shareable PDF, or the whole project (Chapter 10). |
| **Export ▾** | Every print file: `.3mf`, `.3mf` + shareable PDF, calibration plates, STL + swaps, the Blender and OBJ files and the package zip (Chapter 10). |
| **Person icon** | The account panel (below). |

The **ticker** under the header scrolls the product's capability strip. It is information only.

### The account panelpage 29

![The account panel, and its MythaPrism Plug-in and Showroom page.](https://mythaprism.com/manual_assets/m6/t_account.jpg)
![The account panel, and its MythaPrism Plug-in and Showroom page.](https://mythaprism.com/manual_assets/m6/t_account_blender.jpg)

*The account panel, and its MythaPrism Plug-in and Showroom page.*

The person icon slides the account panel down. Its header shows **Signed in as** and your first name when you are signed in. **Refresh workspace** starts the workspace fresh: the picture you dropped in comes back as it was, edits, Prism Modifiers and add-ons are cleared, and your plan's default engine is picked again. Your library, presets and settings are kept. **Settings** has two look switches, **Light mode** (on the web Tool a white top bar, white cards and black outlined buttons over the black field, and the App has its own light look) and **Colorful background** (the soft rainbow wash over the black field, on by default, off for plain black) and **Moving background** (the hexagons drift and pulse. Off keeps them still, which saves battery and keeps a phone cooler. Off by default on phones and tablets, on by default on a computer), **Hint pulsing** (Color match pulses gently when it is the next step, and stops the moment you click it. Off: nothing pulses), and manages your **filament preset libraries**, named sets of filaments you recall with one tap: the preset's filaments turn on, every other filament turns off, a filament you deleted since comes back, and the print re-matches on the spot. **Manage devices** lists the devices on your account. Every account works on a few devices at a time: **Free 2, Plus 2, Pro 3**. When your devices are full, the device you are on offers **Use MythaPrism on this device**, which takes the place of the device you used least recently. You can also remove a device by name in Manage devices, or in the Devices tab of your account page at mythaprism.com. That is a **device change**, and you get **2 a month on Free, 4 on Plus and 6 on Pro** (a device you have not used for 30 days drops off by itself and does not count). On the web, up to three MythaPrism tabs can be open at once on an account. A fourth one asks you to close one of the others. These limits keep your account safe. If you need more changes (a new phone, a repair, a lost device) email support@mythaprism.com and we will help. **Manage subscription** opens your plan. **MythaPrism Plug-in and Showroom** hands Studio Bundle members (and $14.99 buyers) the add-on and the Studio starter scene, everyone else sees where to get it. **Send feedback** opens a one-line form, **Tutorials** and **Support** open the guides and the support address, **Sign out** signs you out on this device only and returns to the website. The account page on mythaprism.com also has **Sign out on every device**. The footer shows the build number and the legal links.

**Global height limit.** Every color matcher plans its own height, and **Dynamic**, the default, leaves it that way. Choose **3, 4, 5, 6 or 7 mm** and no print will be taller than that: the classic engines shorten the filament stack so it fits (every color keeps at least one layer), the zoned engines stop every point at the limit, the relief top of a Hybrid or Focus print is planned to fit on top of its bed and transition (the preview shows exactly the shortened top you will print), and the per-pixel V8 and LithoPrism prints, and the flat Slim and Dual faces, are trimmed at it when you export. A limit can cost tones and change the look, so each change asks you to confirm with **I understand**, and the shareable PDF records the limit. It sits in Print setup, right under First layer height, and turns amber while a limit is on. Most prints never need it. Use it for a frame rebate, a slot or a fixed thickness.

![Print setup → Height limit, and the confirmation every change asks for.](https://mythaprism.com/manual_assets/m6/t_settings_hl.jpg)
![Print setup → Height limit, and the confirmation every change asks for.](https://mythaprism.com/manual_assets/m6/t_hl_confirm.jpg)

*Print setup → Height limit, and the confirmation every change asks for.*

## The stage and its controls

| Control | What it does |
|---|---|
| **Preset ▾** | One-tap looks: Family portrait, Family landscape, Monochrome, Single color impression (Chapter 5). |
| **Colors slider · Auto** | How many filaments the print may use. Drag to pin a count. It ends at the number of filaments selected in your library (at most 2 on Free, 6 on Plus, 24 on Pro). Press **Auto** to let the engine decide. |
| **Prime · Synthesized result · Relief bands · Layer schedule** | The four views of the same print (below). |
| **Mode pill** | 2D image editing · Relief · Slim · Dual · Hybrid · Focus · Litho Prism. Tap a mode for its card, then **Launch**. |
| **2D / 3D** | Switches the stage between the flat preview and a true-scale 3D model. |
| **✎ Edit ▾** | The edit tools (Chapter 6). |
| **↶ / ↷** | Undo and Redo, one history (10 steps on Free and Plus, 25 on Pro) for everything you do to the print: an engine pick, an edit, a slider release, a preset, a setup switch, an add-on, a mode launch, a second picture. Each undo restores exactly what you had, with no re-match. **Ctrl/⌘ + Z** and **Ctrl + Shift + Z** (or **Ctrl + Y**) work too. A new picture starts a fresh history. |
| **+ / − / ⤢ and %** | Zoom in, zoom out, fit. The mouse wheel zooms toward the cursor, drag to pan while zoomed. |

![The view tabs, the mode pill and the preset row.](https://mythaprism.com/manual_assets/m6/t_viewtabs.jpg)
![The view tabs, the mode pill and the preset row.](https://mythaprism.com/manual_assets/m6/t_modepill.jpg)

*The view tabs, the mode pill and the preset row.*

### The four viewspage 32

The views never change the print. Only how you look at it.

Prime

Synthesized result

Relief bands

Layer schedule

![Prime, Synthesized result, Relief bands and Layer schedule for the same match of the flowers.](https://mythaprism.com/manual_assets/m6/t_view_source.jpg)
![Prime, Synthesized result, Relief bands and Layer schedule for the same match of the flowers.](https://mythaprism.com/manual_assets/m6/t_view_result.jpg)
![Prime, Synthesized result, Relief bands and Layer schedule for the same match of the flowers.](https://mythaprism.com/manual_assets/m6/t_view_height.jpg)
![Prime, Synthesized result, Relief bands and Layer schedule for the same match of the flowers.](https://mythaprism.com/manual_assets/m6/t_view_layers.jpg)

*Prime, Synthesized result, Relief bands and Layer schedule for the same match of the flowers.*

| View | Shows |
|---|---|
| **Prime** | Your picture with the 2D edits, Filters looks and Cut out pieces changes applied, before and after a match. Press and hold the small rainbow **Hold to see original** icon (bottom left of the picture, its name shows when you point at it) to see the untouched upload. Let go to come back. In the two-picture modes it splits to show both. |
| **Synthesized result** | The close estimate of the finished print, the relief computed from the filament stack, or the flat color regions in the flat modes. |
| **Relief bands** | The height map: brighter is taller. The fastest way to spot lost detail, thin walls and what a dither does to the surface. |
| **Layer schedule** | A build-up view: drag the slider or press ▶ to watch the print grow layer by layer, in the exact filament order. |

### The 3D view

Press **3D** and you go straight in, with no loading wait. A flat plate showing exactly what the 2D view showed stands in at first, while the real print is built a slice at a time behind it. The picture (both pictures in Dual, Hybrid and Focus) dissolves into gray dots where it sits, the dots fly in as particles and settle into the print's dot grid, then the view tips back into an aerial shot over a black ground with a thin rainbow horizon and rings of rainbow dots. The dots rise into the shape of the relief, a rainbow ring grows from the center and the real print appears behind it before the view settles, filling the whole window behind the panels. Touching the view, scrolling, **Reset** or the tilt slider skips to the end, and a device set to reduce motion skips it altogether.

1 · Where the 2D picture was

2 · Tipping back into the dot grid

![](https://mythaprism.com/manual_assets/m6/intro_a.jpg)
![](https://mythaprism.com/manual_assets/m6/intro_b.jpg)

3 · The rainbow front

4 · Settled

![The 3D entrance: the flat picture starts where the 2D picture was and tips back under a rainbow horizon that runs behind](https://mythaprism.com/manual_assets/m6/intro_c.jpg)
![The 3D entrance: the flat picture starts where the 2D picture was and tips back under a rainbow horizon that runs behind](https://mythaprism.com/manual_assets/m6/intro_d.jpg)

*The 3D entrance: the flat picture starts where the 2D picture was and tips back under a rainbow horizon that runs behind the panels, then the rainbow front raises the relief, and the view settles.*

The stage is then a true-scale model of the exact geometry the export will carry: the base plate, every band at its real height, holes and shape crops cut through, puzzle gaps, both faces of a two-sided print. It rebuilds itself whenever the match, an edit or a setup change alters the print, so what you see is what the `.3mf` contains.

| Control | What it does |
|---|---|
| **Drag · right-drag · scroll** | Rotate · move · zoom (pinch on a touch screen). |
| **Reset** | Recenters the model. The 3D view always opens with the whole print in view, on a narrow phone screen it stands back far enough that the turning print never runs off the sides. |
| **Tilt 0 to 180°** | Leans the plate on its turntable: 90° faces you straight on, 0° lays it flat, 180° lays it flat the other way. The turn stays about the vertical axis, so the picture never wobbles. It starts at 85° every time you open the 3D view. |
| **1x** | Turntable speed. Each tap adds 25 % up to 3x, the tap after 3x returns to 1x. A tap also restarts the turn if a drag stopped it. |

Leaving 3D always returns the 2D stage to 100 %, centered.

![The 3D view: the flowers print.](https://mythaprism.com/manual_assets/m6/t_3d_stage.jpg)

*The 3D view: the flowers print.*

### The size visualizer

**📐 Size visualizer** (in Print setup under Print size) draws your print at scale on your printer's bed, with preset sizes: 200 × 200 mm, square 150 and 100 mm, photo 4 × 6 and 5 × 7 in, comic-book and magazine covers, postcard, card, bookmark and the A-series paper sizes, and a scale slider from **Min** to **Max**. The print stays locked to your picture's proportions. **Use this size** applies it. While **Mural** is on, the presets and slider are grayed out and the bed shows one tile at true scale (Chapter 8).

![The size visualizer on the H2C's 300 × 320 mm bed.](https://mythaprism.com/manual_assets/m6/t_sizevis_box.jpg)

*The size visualizer on the H2C's 300 × 320 mm bed.*

## The Filament library

Everything starts here: MythaPrism only plans with filaments you have enabled, so an honest library of what is on your shelf is the foundation of a good match.

![The library: your chips (enabled ones lit), the brand catalog opened underneath, and the calibration block at the bottom](https://mythaprism.com/manual_assets/m6/t_library.jpg)
![The library: your chips (enabled ones lit), the brand catalog opened underneath, and the calibration block at the bottom](https://mythaprism.com/manual_assets/m6/t_library_catalog.jpg)
![The library: your chips (enabled ones lit), the brand catalog opened underneath, and the calibration block at the bottom](https://mythaprism.com/manual_assets/m6/t_library_cal.jpg)

*The library: your chips (enabled ones lit), the brand catalog opened underneath, and the calibration block at the bottom.*

**Chips.** Each chip shows a color dot, the filament's name, its light depth tagged **typ** or **est**, and its **pair** in brackets: how many layers it needs to show its full color over white, then over black (Black is always 1). Click a chip to enable or disable it, the **✕** removes it from your library. **Select all** and **Clear all** flip the whole library, and the search box filters by name. A new library starts with the nine starter filaments, all enabled. Hover a chip to see its brand, product line and color code.

**Add filament.** Type a name, pick the exact color with the color square and press **Add filament**. A calibration plate can measure any filament you add.

**＋ add library.** Opens the brand catalogs: Bambu Lab's PLA Basic, PLA Matte and PLA Pure with Bambu's own color codes, a CMYK set for the CMYK engines (PLA Basic Cyan, Magenta, Yellow and Jade White from Bambu's lithophane bundle, plus PLA Basic Black), and other brands with approximate colors (marked). Tap any swatch to add it to your library. The **Starter set** sits at the top of the catalog: one tap on **＋ Add the starter set** brings back the nine filaments MythaPrism starts with (Jade White, Blue Grey, Black, Red, Pink, Pumpkin Orange, Yellow, Bambu Green, Marine Blue) with their built-in color and light depth, and selects them (Plus and Pro).

**Filament records.** The **▾** on every chip opens that filament's record: the maker's color, a TD value you can type in, the estimated light depth, the calibrated full-strength color, the layer height, the pair (layers to full color over white and over black), the ceiling height, and the color at every layer over white and over black up to the pair, each marked as measured, between two measured squares, or estimated from the light depth. It also keeps when and how it was measured, a batch note, the printer and nozzle, and the measured mixes. **The pair is yours to edit.** Your number wins over the measured one, a note appears when it is above what the light depth allows, and **Reset to measured** brings the measurement back. Records are saved on this device. **Export all records** writes one file with your calibration sets, **Import** reads one back (only plain numbers and short text are taken), and **Copy details** copies a record as text.

**◆ Second image colors only.** In Dual and Hybrid, limits the second picture to its own palette so the two faces don't fight over filaments.

**The calibration block.** Calibration plate, Read calibration photo, Add plate layout, the results table and the Calibration V4 switch, all of Chapter 9.

Specialty filaments

The color matchers print from **PLA Basic and PLA Matte** (and plain PLA such as PLA Pure), and the catalog lists only those lines. Specialty filaments (marble, sparkle, silk, gradient, wood, galaxy, metallic, glow and translucent) are not in the catalog, because their look can't be built from layers the way a plain color can. If you add one by hand with **Add filament** and its name says what it is (for example "Silk Gold"), the matchers never choose it automatically. You can still use it by hand: as a spot color, as the base or transition filament, or by swapping a band in the Prism control.

## Print setuppage 36

Everything about the physical object: which printer, how big, how fine, what it stands on, and which surface options are on.

![Print setup in full (shown in two halves), and the peek window it opens as.](https://mythaprism.com/manual_assets/m6/t_printsetup_p0.jpg)
![Print setup in full (shown in two halves), and the peek window it opens as.](https://mythaprism.com/manual_assets/m6/t_printsetup_p1.jpg)
![Print setup in full (shown in two halves), and the peek window it opens as.](https://mythaprism.com/manual_assets/m6/t_peek.jpg)

*Print setup in full (shown in two halves), and the peek window it opens as.*

| Row | Choices and what they do |
|---|---|
| **Printer (for .3mf)** | Bambu Lab A1, A1 mini, H2C, H2D, H3C, P1P, P1S, X1, X1 Carbon and X2D (the H2C, H2D and H3C are Pro, Free opens on the Generic 256 x 256 bed), Snapmaker U1, FlashForge Creator 5, Prusa XL (5-toolhead) and CORE One, generic 180 to 350 mm beds. Sets the preset names, the bed and, on two-nozzle machines, the window both nozzles can reach. **Import my printer profile** is the first item of the printer menu (like Save at the top of the Preset menu), and the note about any other 3D printer sits at the bottom of the list, so the rows under it (Size visualizer and the rest) stay in view. The print is centered inside it so the slicer never reports a boundary error. |
| **Print size** | Width × depth in millimeters, locked to the picture's proportions. Type either number, use the steppers or open the size visualizer. |
| **Nozzle** | 0.4 mm (default), 0.2 mm (fine detail) or 0.6 mm (speed and strength). The 0.2 and 0.6 mm nozzles are Pro. |
| **Layer height** | 0.08 mm (default) up to 0.28 mm on the 0.4 mm nozzle (0.06 to 0.14 mm on the 0.2 mm, 0.18 to 0.42 mm on the 0.6 mm). Finer layers give the color model more steps. Free prints at 0.08 mm. Plus has every height on the 0.4 mm nozzle, Pro every nozzle and height. |
| **First layer height** | 0.12 to 0.28 mm on the 0.4 mm nozzle, 0.20 mm by default (0.10 mm on the 0.2 mm nozzle, 0.30 mm on the 0.6 mm). Thicker sticks better on a textured plate. Thinner keeps the base slim. The `.3mf` carries it and every swap height follows it. |
| **Base layer: color** | The opaque foundation (three automatic modes, below, or any enabled filament). |
| **Base layer: thickness** | The **[ − ] 0.7 mm [ + ]** row. The hint shows the layer count. 0.2 to 3 mm. |
| **Watermark on print** | Off, Small, Medium or Large (below). |
| **Dither · Relief test** | Surface texture and structural clean-up (Chapter 5). |
| **Smoother surface · Degradient · Force smoother edges · Halftones** | Calmer surfaces, smooth outlines in the exported file, and a comic dot screen on any color print (Chapter 5). |

Rows appear when a mode needs them: **No backing** and **Print face-up** in Slim, the **Transition layer** count and filament in the two-picture modes, the **Litho panel** in LithoPrism. Each is explained with its mode in Chapter 7.

New in builds 551 to 553

**Height limit** now sits in Print setup, right under First layer height (it used to be in Account → Settings). While a limit is on the row turns amber. **＋ Import my printer profile** under the printer list reads a Bambu Studio printer bundle (.bbscfg), an OrcaSlicer bundle or a PrusaSlicer config on your device and adds it as *Manual · your printer*: the export then names your own printer, process and filament presets, and your saved process settings (speed, strength, supports) carry over, with MythaPrism keeping only the color rules. **TIFF** pictures now open on every device (Plus and Pro).

### Base color: three automatic modespage 38

Auto: darkest selected

Auto: lightest selected

Auto: shortest print

![The same match on the three automatic bases: darkest (no plate), lightest (a light plate for back-lighting) and shortest](https://mythaprism.com/manual_assets/m6/s_base_auto.jpg)
![The same match on the three automatic bases: darkest (no plate), lightest (a light plate for back-lighting) and shortest](https://mythaprism.com/manual_assets/m6/s_base_lightest.jpg)
![The same match on the three automatic bases: darkest (no plate), lightest (a light plate for back-lighting) and shortest](https://mythaprism.com/manual_assets/m6/s_base_shortest.jpg)

*The same match on the three automatic bases: darkest (no plate), lightest (a light plate for back-lighting) and shortest print.*

| Mode | What it does |
|---|---|
| **Auto: darkest selected** | No separate plate: the darkest enabled filament is the foundation and the picture rises out of it. The classic look. |
| **Auto: lightest selected** | A plate of the lightest filament under the picture, a brighter relief and a light back that glows when back-lit. |
| **Auto: shortest print** | Tries no plate and every filament as the plate, keeps the combination with the fewest total layers, and names the one it chose. |

Every engine honors the choice: the classic engines put it under the picture as a plate, and the zoned, sectioner and one-color engines build every zone on it. In the flat modes these rows are relabelled **Backing layer** and set the flat construction instead.

### Watermark on print

Puts the word **MYTHAPRISM** on the print: **Off** by default in every plan, or **Small**, **Medium** or **Large** (letters about 4, 6 or 9 mm tall, smaller on a small print). Two more choices appear once a size is set: **where** (the **Back plate**, reading correctly when you turn the print over, or the **front bottom-right** or **bottom-left corner**) and **color**: **White** (the default) or **Black**. **MythaPrism colors** (each letter in the enabled filament closest to the brand rainbow) is offered only on multi-nozzle printers (H2C, H2D, X2D, Snapmaker U1, FlashForge Creator 5, Prusa XL) and grayed out on the rest.

![A rainbow watermark in the front bottom-right corner of the print, on the stage and in 3D.](https://mythaprism.com/manual_assets/m6/t_wm_stage.jpg)
![A rainbow watermark in the front bottom-right corner of the print, on the stage and in 3D.](https://mythaprism.com/manual_assets/m6/t_wm_3d.jpg)

*A rainbow watermark in the front bottom-right corner of the print, on the stage and in 3D.*

On the front the letters print like text and show in the preview and 3D. On the **back plate** they work with every color matcher: the first layer of the print becomes two zones, the letters and the rest of the base, so that one layer prints in two filaments (the letters are their own parts in the `.3mf`, carved out of the first layer, never overlapping it). That needs an AMS or another multi-material setup for the first layer, the hint and the shareable PDF say so, and a classic-engine print that carries a back watermark is exported as one part per filament instead of the layer-change schedule. Turn the 3D view around to see the letters on the underside. Face-down Slim raises them on its flat back instead, Dual and Hybrid put them on the second picture's face. Pick a letter color that differs from the base layer, or the letters won't show, the hint warns you.

## Add-ons

![The Add-ons card.](https://mythaprism.com/manual_assets/m6/t_addons.jpg)

*The Add-ons card.*

Eight switches in plan order, each with a **✎ Edit** pill that opens its own page (Chapter 8). **Puzzle cut** splits the print into interlocking pieces, **Multi crop** prints several crops of one photo as one set, **Filters** puts one of 310 looks on the photo, **Image Simplifier** shows 100 versions of it in fewer colors, made from your own filaments. **Image Grading** grades the photo’s color and light, **Mural** splits a print bigger than your bed into labeled tiles, **Reassign bands** lets you color the picture section by section and works out the layers for you. Free includes Puzzle cut and the black and white Image Simplifier, Plus adds Multi crop, Filters and Image Grading, Pro adds Mural and Reassign bands (the last two in the list). A new picture turns every add-on off.

## The stack cardspage 40

Under the setup cards, the Tool describes the finished stack in plain terms.

![Swap order after a classic match, Colors in this print after a zoned match, and the Filament change schedule.](https://mythaprism.com/manual_assets/m6/t_swaporder.jpg)
![Swap order after a classic match, Colors in this print after a zoned match, and the Filament change schedule.](https://mythaprism.com/manual_assets/m6/t_colors_in_print.jpg)
![Swap order after a classic match, Colors in this print after a zoned match, and the Filament change schedule.](https://mythaprism.com/manual_assets/m6/t_schedule.jpg)

*Swap order after a classic match, Colors in this print after a zoned match, and the Filament change schedule.*

**Swap order: bottom → top** lists the filament bands from the plate up, in the order they print. Each row has the filament (the bottom one tagged BASE), an editable **layer count**, **▲ ▼** to move the band and **×** to remove it, every change re-synthesizes at once. After a zoned or one-color engine the card becomes **Colors in this print**: every filament the print uses and the share of the surface it covers. Colors are assigned per part in the export, so there are no manual swaps.

**Filament change schedule** lists every change with its layer number and height (L0 · 0.00 mm Black start, L7 · 0.56 mm Yellow and so on) exactly the rows the export and the PDF carry.

## Prism controlpage 41

![Prism control after a classic match (drag the handles), after a zoned match (a note) and in Slim Prism (a build diagram)](https://mythaprism.com/manual_assets/m6/t_prism_stack.jpg)
![Prism control after a classic match (drag the handles), after a zoned match (a note) and in Slim Prism (a build diagram)](https://mythaprism.com/manual_assets/m6/t_prism_zoned.jpg)
![Prism control after a classic match (drag the handles), after a zoned match (a note) and in Slim Prism (a build diagram)](https://mythaprism.com/manual_assets/m6/t_prism_slim.jpg)

*Prism control after a classic match (drag the handles), after a zoned match (a note) and in Slim Prism (a build diagram).*

After a color match, the print's total height sits as plain text right above the strip (for example 3.2 mm), the same number as Peak height in Stats for nerds. It changes as you change anything that changes the print. Before a match it is not shown.

The strip is the print's real achievable gradient, from **PLATE (BASE)** at the bottom to **SURFACE (TOP)**. Drag a white handle line to move where one filament gives way to the next, the preview updates live. Each band label shows the filament, its layer count and thickness. **✎ Edit** opens the band editor: swap a band's filament, remove it, add one, or switch to equal-height rows for easy re-ordering.

After a zoned engine each zone prints its own stack, so there is no single gradient to drag. The card says so and points you at the schedule. In the flat modes the strip becomes a build diagram: the face colors sized by their share of the picture, then the transition band, then the second face.

## Stats for nerdspage 42

![Stats for nerds.](https://mythaprism.com/manual_assets/m6/t_stats.jpg)

*Stats for nerds.*

| Field | Meaning |
|---|---|
| **Peak height** | The tallest point of the print in mm: base plus art layers, or slab plus backing in the flat modes. Two small lines under it give the **Average height** over the whole surface and the **Match ΔE** (below). |
| **Largest percent height** | The height that covers the most of the surface, and how much of it (for example 1.20 mm, 45 percent of the surface). The shareable PDF lists the same heights. |
| **Layers** | The layer count, zoned prints name the tallest zone, flat modes break it down. |
| **Swaps** | Filament changes in the schedule, zoned and flat prints read "per-part assignment, no manual swaps". |
| **Match ΔE** (under Peak height) | The average color difference (CIEDE2000) between your picture and the synthesized preview. Lower is better. Under about 10 reads faithful. |

**When MythaPrism is working.** Anything that takes a moment: a color match, an edit you apply, a Prism Modifier you release, a mode, an export, undo, shows a turning rainbow ring over the picture (or over the open tool). A color match shows its percent inside the ring, and the page keeps drawing while it works, because every color matcher works in short steps. The ring goes away when the tool is ready again. Picking another matcher while one is running stops the first one. Quick actions finish before it appears. The phone app shows the same ring.

05

# Color matching

How many filaments the print may use, which engine maps your picture onto them, how to nudge the result until it is yours, and the surface controls that decide how the relief looks and feels in the hand.

## Presets and the Colors sliderpage 44

The **Colors** slider beside it sets how many filaments the print may use (with a CMYK matcher it gives way to the CMYK pills, Chapter 5). The **Preset ▾** pill above the stage holds **＋ Save preset**, **My presets** and MythaPrism’s one-tap recipes.

**Save preset** keeps what you did to a picture so one tap does it again on the next one. Make your edits, open **Preset ▾** and press **＋ Save preset**. A page lists everything the preset can hold: the **picture edits** in the order you made them (the crop with its shape and framing, a Filters look with its amount and strength, Image Grading, the Image Simplifier), the **print size** (a Size visualizer choice fits the next picture into the same box), the **add-ons** (Mural with its grid and size, Puzzle cut), the **Prism Modifiers** and, for a print that was color matched, the **color match** (mode, color matcher, colors, filaments, dither) and the **print setup**. What you changed is ticked and tagged **Edited**. A tag says if it is a **2D picture preset** or a **3D color matched preset**. Untick what you do not want, press **Save preset**, confirm the name (it starts as the date and time) and it is at the top of **My presets**.

A tap on a saved preset applies it to the picture you have open. The **✎ pencil** beside it opens the preset’s details: untick a setting, change a value, move or remove an edit, rename it, then **Save changes** or **Apply now**. **✕** deletes it. Spot colors, texts, lassos and hand-drawn cut lines belong to one picture, so they are listed but not saved. Presets live on this device, on the Tool and in the App.

MythaPrism’s own recipes:

| Preset | What it does |
|---|---|
| **Family portrait · Family landscape** | Pins a Black / Blue Grey / White stack with Dither 3.0 for the classic three-filament look. They always print all three, even on a black-and-white photo. If Blue Grey (or a close color) is in your library but switched off, the preset switches it on for you and says so. |
| **Monochrome** | Exactly two filaments: your darkest and your lightest. |
| **Single color impression** | A one-filament relief where height alone carries the picture. |

Presets that dither work on relief surfaces only (the Relief print and the raised top of Hybrid and Focus). A flat painted face can't carry a dither, and the Tool says so if you try.

The **Colors** slider sets how many filaments the print may use. Drag it to pin a count. Press **Auto** to let the engine decide. For the one-stack engines Auto builds the real stack for every count from two up to your library and keeps the count whose translucent stack matches the picture best. The blends count, not just the pure filaments, so even a black-and-white photo can plan eight or nine spools. Free prints two colors (black and white), Plus up to six, Pro as many as the picture needs. While Auto is on, the count beside the slider shows how many filaments the print actually uses. In Dual and Hybrid the slider is per picture: pick a side first. A pinned count is exact: when a preset holds a filament, the print uses it even where the engine would have left it out.

## The engine menupage 45

![Color match ▾: the launch lineup by kind (One color per layer, Zoned & sectioner, CMYK) each tab sorted by number.](https://mythaprism.com/manual_assets/m6/t5_matchdrop.jpg)

*Color match ▾: the launch lineup by kind (One color per layer, Zoned & sectioner, CMYK) each tab sorted by number.*

**Color match ▾** opens the engine menu. The **Color match** button itself re-runs the engine you are on, the one-click path. On Plus and Pro a new picture starts on **V1.3**. Tabs group the engines by how they print: **One color per layer** (one stack for the whole plate, one filament per layer everywhere, a swap schedule any printer can follow: V1.3, V1.4, V1.5, V1.6, V1.7 and V1.8 auto · gap · obj, V2 1.0), **Zoned & sectioner** (every area or zone prints its own stack, so these need a multi-material system such as an AMS: V1.2, V2 1.2, V3 1.2, Zoned V1.7 / Zoned V1.8 auto · gap · obj, V24, V25, V25.1 to V25.3) and **CMYK** (the twenty CMYK engines, the dither-like front-lit ones in their own Front-lit dots group under them), the LithoPrism engines get their own tab in LithoPrism mode. Inside the first two tabs the engines are listed by kind: **Each color used once** first (every filament prints in one run, the easiest swaps on a single nozzle and up to four colors), then a divider and **Colors may repeat** (a filament can come back higher in the stack for richer color, so more swaps). Only the CMYK engines carry a beta tag. Hover a button for its one-line description. Locked engines show the plan that unlocks them. Picking an engine re-matches immediately. In the App the engines that use each color once are a list of pills in the Colors sheet, then the ones that repeat, and two circles at the end, **Zoned** and **CMYK**, open their engines when you tap them. Tap an engine, then **Color match**.

## The engine familiespage 46

MythaPrism has 56 engines in nine families, plus the B&W engine (smooth or halftones), which every plan has. You only need to know the families. Each has a character. The grid shows the same photo of Earth matched with one engine from each, on the same nine-filament library.

![One photo, the launch lineup. Same picture, same filaments. Only the engine changes.](https://mythaprism.com/manual_assets/m6/t5_engines_lineup.jpg)

*One photo, the launch lineup. Same picture, same filaments. Only the engine changes.*

| Family | Engines | Character | Plan |
|---|---|---|---|
| **Free B&W** | B&W smooth, B&W halftones | The black-and-white engine, on every plan: a black base with white stacked on top. Thicker white where the picture is brighter. **Smooth** uses every clearly different white thickness as a tone (photo-like), **Halftones** is the smooth relief with a printed-comic dot screen in the shadows: black dots 1.6 mm apart, each one bigger where the picture is darker, so the print reads like a newspaper photo or a comic panel from across the room. On Free it is the only engine. On Plus and Pro it sits at the top of the list, and it also prints Slim, Dual and the Hybrid bed in black and white. | Free |
| **Area match, one stack** | V1.3, V1.4, V1.5 | The picture is read as areas of one color, never as noisy pixels. One stack serves the whole plate, one filament per layer, so any printer can follow the swap schedule. Each area takes the run whose color serves it best and each pixel picks its thickness inside that run, so shading and gradients keep their tones. **V1.3** is the default engine on Plus and Pro, with the Colors slider on it uses exactly the number you choose. **V1.4** treats your count as a ceiling (it may use fewer). **V1.5** is V1.4 that honors any count above six. | Plus |
| **Every pixel, one stack** | V1.6, V2 1.0 | No color areas and no smoothing: every pixel takes its own height on one stack, so line art and fine detail stay crisp. Both protect the picture's small colors: a belt, a purple patch, the grey folds of a black cloak. **V1.6** uses every filament once and plans the stack from the picture's own pixels. **V2 1.0** is V1 with the color count read from the real stack. | V1.6 Plus · V2 1.0 Pro |
| **Layer match, one stack** | V1.7 auto · gap · obj, V1.8 auto · gap · obj | The picture is split into layers at its seams, by color boundaries (**auto**), by gaps between tones (**gap**) or into whole objects (**obj**, an on-device grouping of the picture into objects, no cloud). Then one stack is planned for those layers and every layer takes the run that serves it. Boundaries stay crisp and every print stays under 5 mm. **V1.7** uses each filament once. **V1.8** may bring a color back higher up (never twice in a row) and is the most accurate one-stack engine. | V1.7 Plus · V1.8 Pro |
| **Prime** | Prime, Prime V2 | Layer match with better color and cleaner edges than V1.8 auto at about the same number of layers. **Prime** lets a color come back higher up the stack when that serves the picture. **Prime V2** uses every color only once, so the stack is shorter and each filament is loaded one time. | Pro |
| **Zoned area & AMS layer zones** | V1.2, V2 1.2, V3 1.2, Zoned V1.7 / Zoned V1.8 auto · gap · obj | Different parts of the picture get their own stack, so a sky, a face and a shirt can each use their own filaments. These prints need a multi-material system (AMS). **V1.2** gives every color area the single color your filaments print best, composites included, **V2 1.2** never repeats a filament inside a stack, **V3 1.2** adds detail inside each area (a Detail slider). **Zoned V1.7 / V1.8** start from the layer match's one stack and add a handful of extra stacks only where one stack can't reach a color. | Pro |
| **Zoned stacks** | V24, V25, V25.1, V25.2, V25.3 | The picture is divided into coherent color zones (V24 by sections, V25 by color composites) and each zone gets its own layer plan. V25.1 judges color the way the eye does, V25.2 smooths the surface, V25.3 does both. They made many of the photographic pictures in this manual. Need an AMS. | Pro |
| **CMYK** | V2·V8.5, V2·V8.7, V3·V8.4, V4·V8, V4·V8.1, V4·V8.2, V4·V8.3, each with its v2, and V3·V8.4 v2 no repeats, no black, no black and no repeats. Front-lit dots: V3·V8.1, V3·V8.1 v2, V3·V8.6 | Full color mixed per pixel from cyan, magenta, yellow, black and white, printed as a translucent stack, for when you own the five process spools. V4·V8 keeps skies clean and surfaces smooth (V4·V8.1 vivid, V4·V8.2 no black, V4·V8.3 the smoothest), V3·V8.1 (no black) and V3·V8.4 (one filament per layer) use the dense V3·V8 color space, and V3·V8.1 works out its colors as light through the print, so it looks most like its preview held up to a light. V3·V8.1 v2 keeps V3·V8.1's colors and is built to be seen from the front. **V3·V8.6** is built to be seen from the front too: each dot gets the shortest stack of cyan, magenta, yellow, white and black whose color from the front is nearest the picture, in any order, in printed dots (see Dot detail). V2·V8.5 (free mixing) and V2·V8.7 (accents) are the original front-lit set. **The v2s** (V2·V8.5 v2, V2·V8.7 v2, V4·V8 v2 to V4·V8.3 v2) are built to be seen from the front with a smooth surface: each dot gets the front-lit stack nearest its color with no carried error, so there is no dither pattern, small specks join their neighbors and the top is flat. Measured on our test pictures they are about twice as close to the picture as the originals. **The 1-layer v2s** print one filament per layer over the whole plate, so they print on any printer with filament swaps: V3·V8.4 v2 plans the whole schedule at once and uses black at its rule (only to darken what prints over it), **no repeats** prints every filament as one run, **no black** leaves black out. The originals stay in the list to compare. Print the CMYK calibration tile first. | Pro |
| **LithoPrism** | V8 Litho, V8 Litho.1, V8 Litho.2, V2·V8 Litho ×3, V34 Litho, V34.1 Litho | The full-color lithophane, planned for light from behind. They live inside LithoPrism mode (Chapter 7). | Pro |

Retired engines

Before launch the list was cut to the engines that print best and are easiest to choose between. V1, the classic engine, is back as a button on Plus and Pro (since build 585) and still runs the Monochrome preset. V11 still runs the Family portrait and landscape presets, without a button. A project saved with a retired engine opens with its picture and settings and is re-matched with V1.3 (B&W on Free). The Tool says so.

![The B&W engine on Pro: the flowers in black and white, smooth.](https://mythaprism.com/manual_assets/m6/b610_bw_flowers.jpg)

*The B&W engine on Pro: the flowers in black and white, smooth.*

### Practical picks

- **V1.3** for almost anything on any printer, the default.
- **V1.6** or **V2 1.0** for line art, logos and crisp detail, or when a small color (a belt, an eye, a purple patch) must survive.
- **V1.7 gap** for clean tone layers, **V1.8** (Pro) when one stack still misses a color. It may bring a filament back higher up.
- **V25** or **V25.3** for photographs on an AMS, **V25.2** for the smoothest surface.
- **V1.2** or **V3 1.2** for flat art, logos and gradients on an AMS, **Zoned V1.8** for the layer match with a few extra stacks.
- **V4·V8.1** or **V4·V8.3** when you own cyan, magenta, yellow, black and white and want continuous color from five spools.
- **Filters** looks (halftone, posterize, comic, neon and more) for a graphic look, with any engine.

**Two-picture modes.** In Dual and Hybrid every picture has its own engine: pick a side (the Image 1 / Image 2 pills on the stage), then choose an engine, count or preset for that picture alone. The other picture is never re-matched by a choice you make for this one. The add-ons that change the photo (**Filters**, **Image Grading** and the **Image Simplifier**) work the same way: click the picture you want, and the add-on opens on that picture, with its name in the title. In the App, the Image 1 and Image 2 tabs at the top of the edit sheet choose it.

**Every engine in every mode.** On a Hybrid relief top or a Focus subject the engine builds the same stack and the same heights it builds in Relief. On a flat face (Slim, either Dual picture, the Hybrid bed, the Focus background) each pixel prints one filament, so the engine chooses that face's colors: the one-stack engines plan their stack on that picture and use its filaments, and the zoned engines use the filaments their areas pick.

## Engine settingspage 50

![The Engine settings card after a V25 match.](https://mythaprism.com/manual_assets/m6/t_neural.jpg)

*The Engine settings card after a V25 match.*

After a V25-family, V1.2 / V2 1.2 / V3 1.2 or Zoned V1.7 / V1.8 match, the **Engine settings** card appears in the right column with the engine's own settings (the name is historical: these are tuning knobs, not a neural network). For V25: **Vibrance** (push muted colors toward vivid, and 1.0 is off), **Neutral** (colors weaker than this stay gray), **Dark keep** (protects deep shadows from the boost), **Zones** (how many color zones, 2 to 80), **Color bias** (group by color, or by location) and **Max side** (matching resolution). V25.1 to V25.3 add **Unify tolerance**, **Surface smoothing** and **Top layers**, Zoned V1.7 / V1.8 show **Max zones** (1 to 16 stacks) and **Zone threshold** (how much better the print must get before a zone is added). V1.2 (and V2 1.2 / V3 1.2) shows **Color areas** (how many distinct colors it reads, 4 to 64, more = finer gradients), **Smallest area** (mm² below which an area joins its neighbor, and 0 keeps everything), **Max side** (match resolution, up to 3000 px: it can't go past the picture's working resolution) and, since build 546, seven more: **Max zones** (1 to 100: the most separate stacks the print may have. 1 is one stack for the whole plate, 2 means every layer is made of at most two zones, 100 = no limit, the default), **Noise smoothing** (lower keeps fine texture, 0 = off), **Split sensitivity** (lower catches small distinct colors sooner), **Merge distance** (higher = bolder, flatter areas, and lower only matters when the picture has very close shades), **Simplicity** (lower lets a busier composite win when it is closer), **Stack sharing** (higher = look-alike areas share one stack, fewer zones) and **Per-pixel detail** (V1.2 / V2 1.2: inside each zone a pixel may take another height of its own stack. Shading comes back without new stacks). Every one of them at its default prints exactly what V1.2 printed before. On a test photo: Noise smoothing 4 took flat patches from 13 % to 8 % of the picture Split sensitivity 6 the ΔE from 4.3 to 4.0 and Simplicity 0.3 to 4.1. Max zones 3 is a much simpler print (ΔE 9.4) and 1 zone a single stack (ΔE 22).

Change a value, then **Rerun V25** to re-match. **Randomize & run** rolls every setting within its useful range: a fast way to explore looks, **Undo / Redo** step through the rolls, the 🔒 beside a setting holds it during a randomize, and **Reset** restores the engine's tuned defaults.

## Prism Modifierspage 51

The **Prism Modifiers** card adjusts how your picture's colors are judged before matching, and re-matches live as you drag. At zero every slider is exactly neutral. In Dual and Hybrid the sliders are per picture, and they are baked into the exported file, not preview-only tweaks.

No modifiers

Vibrance +70

White balance, warm

Vignette +70

![](https://mythaprism.com/manual_assets/m6/s_mod_none.jpg)
![](https://mythaprism.com/manual_assets/m6/s_mod_vib.jpg)
![](https://mythaprism.com/manual_assets/m6/s_mod_warm.jpg)
![](https://mythaprism.com/manual_assets/m6/s_mod_vignette.jpg)

Contrast +60

Hue +55

Clarity +80

White balance, cool

![One picture of the planets, one engine (V1.3): no modifiers, then Vibrance, warm White balance, Vignette, Contrast, Hue,](https://mythaprism.com/manual_assets/m6/s_mod_contrast.jpg)
![One picture of the planets, one engine (V1.3): no modifiers, then Vibrance, warm White balance, Vignette, Contrast, Hue,](https://mythaprism.com/manual_assets/m6/s_mod_hue.jpg)
![One picture of the planets, one engine (V1.3): no modifiers, then Vibrance, warm White balance, Vignette, Contrast, Hue,](https://mythaprism.com/manual_assets/m6/s_mod_clarity.jpg)
![One picture of the planets, one engine (V1.3): no modifiers, then Vibrance, warm White balance, Vignette, Contrast, Hue,](https://mythaprism.com/manual_assets/m6/s_mod_cool.jpg)

*One picture of the planets, one engine (V1.3): no modifiers, then Vibrance, warm White balance, Vignette, Contrast, Hue, Clarity and cool White balance.*

| Slider | Effect |
|---|---|
| **Working resolution** | The pixel budget the whole Tool runs at: matching, preview and mesh detail. 1200 px for a new picture. Plus goes to 2160 px, Pro to 4096 px for house-scale murals. |
| **Tone · Brightness · Contrast · Midtones** | Overall balance, exposure, tonal punch and the middle tones. |
| **Vibrance · Saturation · Hue** | Boost muted colors, saturate everything evenly, rotate every color around the wheel. |
| **White balance · Tint** | Cooler ↔ warmer, and green ↔ magenta. |
| **Highlights · Shadows** | Lift or lower only the bright or only the dark tones. |
| **Vignette** | Darken (right) or lighten (left) toward the corners. |
| **Sharpness · Clarity** | Crisper edges and text, midtone punch without crushing highlights or shadows. |
| **Gradients** | Smooths banding so skies micro-blend instead of forming hard stripes. |
| **Skin tones** | Left deepens toward olive and rich brown skin, right lightens toward fair skin and drains orange. |
| **De-Blotch · Island smoother** | Merge noisy patches and tiny specks into their surroundings (spot colors and text are protected). |

![Randomize and Reset.](https://mythaprism.com/manual_assets/m6/t_randrow.jpg)

*Randomize and Reset.*

Under the sliders, **🎲 Randomize modifiers** deals a fresh, moderate set of values across every grading slider except Hue and re-matches once. **↺ Reset modifiers** puts them all back to 0. The 🔒 beside a slider locks it, so a randomize or reset leaves it alone. The **Pro** action buttons act on the whole stack: **◐ Invert colors** flips it, **⟳ Rotate colors** cycles the order, **⇅ Reverse stack** reverses it, **🎲 Randomize stack** shuffles it and **🎲 Randomize stack + filaments** also re-deals the filaments from your library.

## Surface: ditherpage 52

A relief has a few dozen printable heights, each producing one color. A photo has millions. Without dither every point snaps to its nearest printable color and smooth gradients break into visible steps. Dithering trades resolution for color: two printable colors alternating in a fine pattern read, from arm's length, as the tone between them, and the translucent plastic itself blends neighboring columns.

Off

1.0

2.0

3.0

4.0

![](https://mythaprism.com/manual_assets/m6/s_dither_off.jpg)
![](https://mythaprism.com/manual_assets/m6/s_dither_d1.jpg)
![](https://mythaprism.com/manual_assets/m6/s_dither_d2.jpg)
![](https://mythaprism.com/manual_assets/m6/s_dither_d3.jpg)
![](https://mythaprism.com/manual_assets/m6/s_dither_d4.jpg)

![A black-and-white Moon (the Monochrome preset, Black + Jade White, Contrast adjusted) with Dither Off, 1.0, 2.0, 3.0 and](https://mythaprism.com/manual_assets/m6/t_dither_3d_off.jpg)
![A black-and-white Moon (the Monochrome preset, Black + Jade White, Contrast adjusted) with Dither Off, 1.0, 2.0, 3.0 and](https://mythaprism.com/manual_assets/m6/t_dither_3d_d1.jpg)
![A black-and-white Moon (the Monochrome preset, Black + Jade White, Contrast adjusted) with Dither Off, 1.0, 2.0, 3.0 and](https://mythaprism.com/manual_assets/m6/t_dither_3d_d2.jpg)
![A black-and-white Moon (the Monochrome preset, Black + Jade White, Contrast adjusted) with Dither Off, 1.0, 2.0, 3.0 and](https://mythaprism.com/manual_assets/m6/t_dither_3d_d3.jpg)
![A black-and-white Moon (the Monochrome preset, Black + Jade White, Contrast adjusted) with Dither Off, 1.0, 2.0, 3.0 and](https://mythaprism.com/manual_assets/m6/t_dither_3d_d4.jpg)

*A black-and-white Moon (the Monochrome preset, Black + Jade White, Contrast adjusted) with Dither Off, 1.0, 2.0, 3.0 and 4.0 (4.5 looks the same as 4.0 on a two-color print), the synthesized result on top, the same print in the 3D view underneath.*

| Setting | What it does | When |
|---|---|---|
| **Off** | Every point snaps to its nearest printable color. Cleanest geometry, visible steps in gradients. | Line art, logos, flat posters. |
| **1.0** | Classic error diffusion: each point prints its nearest color and passes the leftover error to its neighbors. The preview shows the smooth ideal. The print carries the pattern. | Maximum fidelity when you plan to smooth the print. |
| **2.0** | The detail of 1.0 without its checkerboard and without tall peaks: no point stands far above its neighbors. | The everyday texture mode on Plus. |
| **3.0** | The blue-noise blend: an even, irregular texture with no checkerboards and no streaks, and a peak cap measured in color steps so mid-grays survive next to a tall black base. The Family presets use it. | Photographs and portraits. Pro. |
| **4.0** | Dots the size of your nozzle, made only from heights the color matcher already chose next to each other, so there are no tall towers, deep pits or checkerboards, and the picture keeps its detail because the dots follow the matcher's own tone curve and a blue-noise pattern. It works on every color matcher, the zoned and V8 engines included, and turning it off brings back the matcher's own answer. | Any matcher, when the earlier dithers leave peaks or patterns. Pro. |
| **4.5** | 4.0 without its checkerboard: each dot chooses between the two colors nearest it by an even blue-noise pattern instead of passing on its leftover error. On a black and white, Monochrome or one-color print it has its own finer look: dots half the size of 4.0 and the tone sharpened against its neighbors, so stripes, hair and edges stay crisp (the smallest dots blend in the print, so the print looks smoother than the dots on screen). On a color print the checkerboard is gone. | Color prints where 4.0 shows a checkerboard. Pro. |

Dither 1.0 to 3.0 act on relief surfaces. On flat faces they have no effect and the row dims. The V8 per-pixel engines and the zoned engines plan their own texture, and Dither 4.0 and 4.5 are the dithers that also work on top of them. One dither is on at a time, and picking a new color matcher turns the dither off. The B&W engine (smooth or halftones) dithers too on Plus and Pro: its black and white tones blend with every dither your plan has (1.0 and 2.0 on Plus, all of them on Pro). Free prints B&W without dither.

**Dithering is for 2 to 4 colors.** A dither turns on only when the print uses 4 colors or fewer, the base plate counted. With more, the printer turns the surface and the look of the picture into mush, so 2 or 3 colors give the best dithered print and 4 is the most for every dither. Each time you turn a dither on, a card says so: dithering is an advanced process, any printer can print it with a layer by layer color matcher since each color prints in its own layers, and a dithered print can make a large file that is sometimes very slow to slice. **Don't show this again** skips the card on that device. With more than 4 colors the card asks you to lower the Colors slider first, and a dither that is on when the print grows past 4 colors (a new match, a preset or a project) turns off with a note that says why.

The photo

Dither 4.5, up close

![A tiger photo A.R. took at the Virginia Safari Park (used with its permission), printed with Family portrait and Dither ](https://mythaprism.com/manual_assets/m6/b635_tiger_photo.jpg)
![A tiger photo A.R. took at the Virginia Safari Park (used with its permission), printed with Family portrait and Dither ](https://mythaprism.com/manual_assets/m6/b635_tiger_close.jpg)

*A tiger photo A.R. took at the Virginia Safari Park (used with its permission), printed with Family portrait and Dither 4.5 in three filaments. The right picture is a Blender render of the real export up close, a close estimate of the print.*

Off

1.0

2.0

3.0

4.0

![Close-ups of the Moon in the 3D view, Off, 1.0, 2.0, 3.0 and 4.0: Off shows flat bands of gray, 1.0 a fine salt-and-pepp](https://mythaprism.com/manual_assets/m6/t_dither_3dz_off.jpg)
![Close-ups of the Moon in the 3D view, Off, 1.0, 2.0, 3.0 and 4.0: Off shows flat bands of gray, 1.0 a fine salt-and-pepp](https://mythaprism.com/manual_assets/m6/t_dither_3dz_d1.jpg)
![Close-ups of the Moon in the 3D view, Off, 1.0, 2.0, 3.0 and 4.0: Off shows flat bands of gray, 1.0 a fine salt-and-pepp](https://mythaprism.com/manual_assets/m6/t_dither_3dz_d2.jpg)
![Close-ups of the Moon in the 3D view, Off, 1.0, 2.0, 3.0 and 4.0: Off shows flat bands of gray, 1.0 a fine salt-and-pepp](https://mythaprism.com/manual_assets/m6/t_dither_3dz_d3.jpg)
![Close-ups of the Moon in the 3D view, Off, 1.0, 2.0, 3.0 and 4.0: Off shows flat bands of gray, 1.0 a fine salt-and-pepp](https://mythaprism.com/manual_assets/m6/t_dither_3dz_d4.jpg)

*Close-ups of the Moon in the 3D view, Off, 1.0, 2.0, 3.0 and 4.0: Off shows flat bands of gray, 1.0 a fine salt-and-pepper grain, 2.0 the same detail without the tall spikes, 3.0 the even blue-noise texture, and 4.0 dots the size of the nozzle.*

## Surface: relief testspage 54

A thin light outline (a white line around a logo, a highlight on a leaf edge) can only show its color at the top of the stack, so it prints as a tall wall one or two pixels wide: the most brittle geometry there is. The relief tests turn it around: they carve any thin ridge a few layers *below* its surroundings, so the outline becomes an engraved groove and the thick areas become the peaks.

Off

v1

v2

![](https://mythaprism.com/manual_assets/m6/s_relief_off.jpg)
![](https://mythaprism.com/manual_assets/m6/s_relief_v1.jpg)
![](https://mythaprism.com/manual_assets/m6/s_relief_v2.jpg)

![Relief test Off, v1 and v2 on Earth (V1.6), synthesized on top, relief bands below. v1 grooves every thin ridge, and v2 ](https://mythaprism.com/manual_assets/m6/h_relief_off.jpg)
![Relief test Off, v1 and v2 on Earth (V1.6), synthesized on top, relief bands below. v1 grooves every thin ridge, and v2 ](https://mythaprism.com/manual_assets/m6/h_relief_v1.jpg)
![Relief test Off, v1 and v2 on Earth (V1.6), synthesized on top, relief bands below. v1 grooves every thin ridge, and v2 ](https://mythaprism.com/manual_assets/m6/h_relief_v2.jpg)

*Relief test Off, v1 and v2 on Earth (V1.6), synthesized on top, relief bands below. v1 grooves every thin ridge, and v2 keeps compact detail.*

**v1** turns every thin peak into a valley. Maximum clean-up when there is no fine detail to lose. **v2** tells slender walls from compact details by shape (a wall is thin however long it is, and an eye has an inside), keeps the compact ones at full height and grooves only the walls. The groove takes the color of the stack below, which usually reads as a crisp dark outline. The relief tests switch off while a dither is on.

## Surface: Smoother surface, Degradient and smoother edgespage 55

All off

Smoother surface

Degradient

![The surface toggles on the same match.](https://mythaprism.com/manual_assets/m6/s_toggle_none.jpg)
![The surface toggles on the same match.](https://mythaprism.com/manual_assets/m6/s_toggle_smoother.jpg)
![The surface toggles on the same match.](https://mythaprism.com/manual_assets/m6/s_toggle_degradient.jpg)

*The surface toggles on the same match.*

**Smoother surface** gives busy pictures fewer, cleaner color steps at the cost of some variety. **Degradient** turns each smooth gradient into one clean color, fenced by the picture's own lines, a poster-like read with fewer filament changes. **Force smoother edges** (Plus and Pro, off by default) changes only the exported file: off, every edge follows the picture's pixels in small square steps, the smallest and fastest file. On, the edges of color areas, flat faces, backings, the zoned stacks and shaped crops follow smooth outlines along the picture's own lines. On a busy picture the file gets larger and the export slower (a zoned V25 print about three times the size). Dithered prints and the CMYK dot prints always keep their dots.

**Halftones** (Plus and Pro, off by default, right under Force smoother edges) lays the same dot screen as B&W halftones over any color-matched print: in the darker parts of the picture, round dots 1.6 mm apart drop to the base color, bigger where the picture is darker. The colors of the print do not change, only where the dots sit. It works on every color matcher in Relief, Slim, Dual and Hybrid. Turn it off and the print is exactly as before.

![The planets with B&W halftones on Free (left), the same picture matched with V1.3 (middle) and V1.3 with the Halftones s](https://mythaprism.com/manual_assets/m6/t_halftones630.jpg)

*The planets with B&W halftones on Free (left), the same picture matched with V1.3 (middle) and V1.3 with the Halftones switch on (right). Real screen captures, build 630.*

Every row in Print setup has a chevron at its right end that opens what it does.

## The CMYK prints and their dotspage 56

The CMYK color matchers print a picture from **Cyan**, **Magenta**, **Yellow**, **Black** and **White** (Bambu Lab PLA Basic), the way a paper printer works, in tiny dots seen from the front. Pro, and a beta. Print the **V8 calibration tile** from the Export menu first: it grounds the colors in your own cyan, magenta, yellow, black and white spools. The CMYK dither switches of earlier builds are out for now while we work on them.

### Dot detail

**Dot detail** shows in Print setup for V3·V8.6. The 3MF is built from exactly the dots you see. **Small file**: dots about 0.8 to 1 mm, the smallest 3MF and the fastest slicing. **Fine dots**: dots 0.4 to 0.6 mm, each dot its own block, a large 3MF that slices slower. **Fine dots, lean file**: always nozzle-size dots (0.4 mm), built with shared walls and the white base in one piece, so it needs about half the triangles of a block per dot (on a busy picture the 3MF can still be large). Up close every choice shows its dots, like a printed photo in a magazine. From a step back they blend.

### The CMYK pills in place of the Colors slider

A CMYK matcher prints with a fixed set of filaments, so the number of colors is set. While one is picked, the Colors slider next to **Preset** (in the App, the slider in the Colors sheet) is replaced by pills. A smooth-surface v2 shows its **Dot detail**: **Small file** (dots grow only as much as a 1.4 million triangle file needs, the smallest 3MF), **Fine dots** (as fine as a 7 million triangle file allows) and **Every pixel**, the v2 default (every dot is one of the picture's own pixels, neighbors share walls, the most detail and on a busy picture a large 3MF). A tap on a name picks it and matches again. Every other CMYK matcher shows **Fixed colors** with the filaments it prints. The chevron at the right of a pill opens what it does. **Preset** stays live, and picking a preset or a matcher that is not CMYK brings the slider back.

06

# Edit tools

A full photo editor lives inside MythaPrism: built for printing, so every edit follows the picture into the match, the 3D model and the file. Cut out a subject, swap a background, crop to a shape, paint an exact brand color, add text and real braille, punch a hole for a keyring.

## How the tools workpage 58

Open them with **✎ Edit ▾** on the stage (App: the **Edit** sheet). Every tool opens as a page: the picture large on the left, its controls in an **action rail** on the right (beneath the picture on the phone). When a match exists the tools open on the synthesized view, so you see what will print, the **Prime | Synth** pill switches to the untouched source when you want to pick pixels from it. **Apply** doesn't close a tool, lay several spot colors or holes in a row, then close. Every Apply is one step in the Undo history.

![The Edit menu.](https://mythaprism.com/manual_assets/m6/t_editmenu.jpg)

*The Edit menu.*

On a phone or touch screen, anything you place over the picture (a text, a hole-punch shape, an added image, a background, the crop) follows your fingers: **one finger drags, two fingers pinch to resize and twist to rotate.** Rotation clicks into place at 0°, 90°, 180° and 270°. The small resize and rotate pins have a wide touch area.

**The Brush.** Every tool with a selection (Cut out pieces, the Background editor, Spot color, Crop's selection and the Hole punch) has a Brush row under Points, Freehand and Snapper: **🖌 Brush** paints the highlighted selection, **⌫ Erase** removes from it, **↶ Undo stroke** steps back, and **Size** runs from a 1 px tip to 120 px. Size is measured on the screen, so zooming in makes the tip finer on the picture. Pinpoint work is zoom in, small tip. A ring shows the tip under the pointer (Chapter 3 shows it on a photo).

## ✂ Silhouette cutterpage 59

![The Silhouette cutter on the flowers: Sections on Obj and five flowers clicked (they light up), ready to cut out.](https://mythaprism.com/manual_assets/m6/b608_cut_sections.jpg)

*The Silhouette cutter on the flowers: Sections on Obj and five flowers clicked (they light up), ready to cut out.*

**Edit → ✂ Silhouette cutter** cuts the subject out of the picture and takes the background away. It opens as a page: the picture on the left with its views under it (**Picture**, **Pieces**, **Gray + splits** and **Hide**), the steps on the right.

**Background.** The highlighted area is what MythaPrism takes as the background: everything joined to the edge of the picture in colors close to the edge. Raise **Tolerance** to take more away, lower it to keep more. **Fill subject by click** makes the area you click, and everything joined to it in close colors, part of the subject (click more areas to add them). **Restore background** brings the background back. To outline the subject, use **Points**, **Freehand** or the **Snapper** (points that snap onto the subject’s edge), with **Undo point** and **Clear outline**. **Brush** paints the subject and **Erase** paints the background. A circle under the pointer shows the brush size, and **Undo stroke** takes back the last stroke.

**Sections** cut the picture up first: **Auto** (at the color boundaries), **Gap** (gray tone levels), **Obj** (whole objects, up to 500), **Tones** (a few gray tones) or **Relief** (the print’s own bands, after a color match). Click the sections of the subject and they light up (**Invert** and **Clear** help), then press **Cut out: remove background** (the lit sections are the subject, another tool keeps them as its subject). Pick the background for the cut-out, **None** (transparent), **Black**, **White** or **Color**, and press **Cut out: remove background**. **Use the cut-out for workspace** then makes it the workspace picture.

## ⧉ Cut out piecespage 60

**Edit → ⧉ Cut out pieces** splits the picture into pieces you can merge, restyle and save. Cutting the subject out lives in its own tool, **✂ Silhouette cutter**, just above it in the Edit menu. It opens as a window: the picture on the left with its views under it, and numbered steps on the right that fold open one at a time, each with a summary beside it. **Use this for workspace** stays at the bottom, always in reach. It works on the workspace picture, or on a picture you pick with **Open another…**, which never touches the workspace. Everything runs on your device.

**1 · Split** cuts the picture into pieces: **Auto** at the color boundaries (Detail), **Gap** by tone level, **Obj** into whole objects (up to 500), **Tones** into a few gray tones the way the Silhouette cutter’s Tones sections do, **Relief** along the print’s own bands so that every area printing at the same height is one piece (workspace picture only, after a color match), and **Brightness**, the connected areas lighter than a cutoff. **Smallest piece** merges crumbs away.

**2 · Pieces.** Click pieces on the picture or in the list to select them. **All**, **None** and **Invert** change the whole selection. **Merge** joins the selected pieces into one, which goes to the top of the list, and **↶** undoes the last merge. Every piece in the list has its own download button.

**Views.** Under the picture: **Picture**, **Pieces** (each piece in its own color), **Gray + splits** and **Hide** (the picture goes black and only the split lines and the pieces you selected show). After a cut-out, **Cut-out** and **Mask** join them.

![Left: step 2 on Obj (60 pieces) and step 3 open in the Pieces view, two flowers selected and ready to Merge. Right: Cut ](https://mythaprism.com/manual_assets/m6/b608_cut_pieces.jpg)
![Left: step 2 on Obj (60 pieces) and step 3 open in the Pieces view, two flowers selected and ready to Merge. Right: Cut ](https://mythaprism.com/manual_assets/m6/b608_cut_phone.jpg)

*Left: step 2 on Obj (60 pieces) and step 3 open in the Pieces view, two flowers selected and ready to Merge. Right: Cut out pieces in the App, the picture on top and the steps under it.*

**3 · Look on pieces.** A Filters look, with Effect and Strength, on the selected pieces only, or on the whole picture when none are selected. **Apply to selected** bakes it in (**↶ Undo**, **Reset**). To grade color and light, use Image Grading. **5 · Save.** Each piece **Cropped** or **Full size**, with 0 to 4 px of **Edge smoothing**, **All pieces .zip** or **Selected .zip** (with a pieces.json of every position), a **Layered .psd** (one layer per piece, for any image editor) or the **Edited picture .png**.

**Use this for workspace** sends the result back. With pieces selected, only they stay and everything else turns transparent, so only those pieces print. With nothing selected the whole edited picture goes back. The print re-matches (or, before a match and in 2D image editing, it is simply your edited photo), and it is one ↶ Undo step.

## ▦ Background editorpage 61

![The Background editor on Earth: the black of space around the globe is selected as background, ready for a new color or ](https://mythaprism.com/manual_assets/m6/t_edit_bg.jpg)

*The Background editor on Earth: the black of space around the globe is selected as background, ready for a new color or picture.*

Select the background exactly as in the subject picker, then instead of removing it, **fill it with a solid color** (**Apply color**) or **Use image** to put another picture behind your subject. Two tabs choose what you move: **Move subject** drags and scales your picture, **Move background** drags and scales the new background, and **Fit background** fills the frame with the whole background again. Then apply. The editor stays open after each Apply, so you can select another part and change it too, and closing it takes you back to the workspace. **Add background behind cut-out** puts a picture behind a subject you already cut out.

## ⬚ Crop and shape croppage 62

![Crop: the flowers cut to a heart: size presets, shapes and the rounded-corners slider in the rail.](https://mythaprism.com/manual_assets/m6/t_edit_crop.jpg)

*Crop: the flowers cut to a heart: size presets, shapes and the rounded-corners slider in the rail.*

A frame over the picture: drag the picture to position it, zoom with the wheel or the slider (pinch on a phone), then **Crop**. The presets set a real print size at the same time, **200 × 200**, **Bookmark 50 × 150**, **Card 85.6 × 54** and **54 × 85.6**, **3:4**, **4:3**, **16:9** and **Free**. **Shapes** crops the printed object itself (circle, square, triangle, heart, star, diamond, hexagon and more) and **Rounded corners** cuts smooth corners. On a touch screen, two fingers twist to rotate the picture under the frame. Spot colors and texts follow the crop. Anything cropped away is gone from the print. Pulling an edge past the picture makes it bigger, and the **New border** section in the rail fills the new border with the picture’s edge colors or one color you pick. The crop opens on your picture as it is, filling the workspace, and the border appears only while you pull the frame past the picture. Choosing a shape or a size never makes the picture jump.

**Recrop.** When you want the whole picture in a new shape without cutting anything off, open the **Recrop** section and pick a size such as **1920 × 1080**. The picture is fitted inside that shape on a background: **One color** (black to start with, or any color you pick) or **Edge colors** carried out from the picture.

## ◉ Spot colorpage 63

![The Spot Color window on the planets: Jupiter flood-selected on the synthesized print, a filament picked, and the Brush ](https://mythaprism.com/manual_assets/m6/t_edit_spot.jpg)

*The Spot Color window on the planets: Jupiter flood-selected on the synthesized print, a filament picked, and the Brush under Points, Freehand and Snapper.*

Click an area to flood-select it (**Tolerance** controls the spread, more clicks add), or trace it with Points, Freehand or the Snapper. Pick any filament in your library, enabled or not, or use the eyedropper to sample a pixel and let the tool find the closest filament or printable blend, then **Apply spot color**. The color prints only inside the selection. It never leaks to look-alike pixels elsewhere. A circle under the pointer shows the brush size, and the window’s sections (**Select with**, **Spot color** and **Palette**) open and close on their own.

A color the print already makes is *embedded* at the height where it already shows. It adds no layers and no extra filament change. Only a color the stack can't make gets a thin cap on top. **On top of everything** forces an opaque cap so the color reads true even over a dark stack. In the flat modes a spot is simply a flat region. **Remove all spot colors** clears every spot on the picture you are editing (added texts stay). Before a match, it puts the photo back as it was under the paint.

## T Add text, and braillepage 64

![Add text on the flowers, with the Braille (tactile) switch on.](https://mythaprism.com/manual_assets/m6/t_edit_braille.jpg)

*Add text on the flowers, with the Braille (tactile) switch on.*

Up to three texts per picture, kept as live objects: reopen the tool and they come back, fully editable. Click a text to select it, the input box, the font (**Bold**, **Mono**, **Sans**) and the filament chips change the selection. Drag to move, pull the square handle to resize, the round handle to rotate, or pinch and twist with two fingers anywhere in the picture area (on a phone they do not have to land on the picture itself). A new text prints **On top of everything**, with its own cap of its color. In the flat modes text is flat by nature.

**Click to place.** A click on an empty part of the picture puts a text there: the selected text moves there when it is still empty, otherwise a new text starts (up to 3). The **Color** section works like Spot color: **Choose color from image** (click the picture, after a match you get the nearest solid filament or printable mix, before a match the exact color), **Solid filament**, **Colors in your print**, **Composite mixes** (a text in a mix prints exactly like a spot color of that mix), then every plain Bambu Lab PLA Basic and PLA Matte color. Picking a catalog color adds it to your library. **⬒ On top of everything** is a switch on each text, ON for every new text. ON gives the text its own cap above the whole stack, as many layers as its color needs to cover what is under it (white over black takes 8 layers at 0.08 mm), so its color prints true. OFF prints the text flush inside a band that already has its color, with no extra layers (a color the stack does not have still gets a cap), and a note explains that the color can come out tinted by the layers right under it. The zoned engines give a text its full cover either way.

**⠿ Braille (tactile)** turns a text into raised braille. **Braille size** picks the dots: **ADA standard**, the default, with dot sizes and spacing inside the 2010 ADA Standards, Table 703.3.1 (dots 1.5 to 1.6 mm wide at the base and at least 0.64 mm tall, 2.5 mm dot to dot, 6.2 mm cell to cell), or **FBM**, the Filament Braille Method from MythaBraille (smooth dots 2.4 mm wide and 0.56 mm tall on the same spacing), which reads smoothly on filament prints but is not an ADA size. Use ADA standard for public signs. The right sizes alone do not make a sign ADA compliant. Under the button, **Braille code** picks how the text is written: English, Grade 1 (every letter spelled out, the default and the easiest to check), English, Grade 2 (beta, contracted braille), Spanish (beta, with its own signs for á é í ó ú ü ñ, ¿ and ¡) or Arabic (beta, letters, short vowels and shadda, read left to right like all braille). Grade 2, Spanish and Arabic are made by software, so have a braille reader check them before anyone relies on them. It keeps that size, because braille only reads correctly at standard size. Pinching a braille text shows a note instead of resizing it. To change the size of the whole print use the Size visualizer, and the braille keeps its real size.

The braille options sit in labeled rows. **Dot color**: the same color as what is under the dots, or a color of its own. **Raised plate**: a pill-shaped plate under the dots, on by default in Relief and the zoned engines and off on flat tops, with a **Plate color** on flat tops. **Dot shape**: Smooth, Rounded or Flat top. **Dot sides**: Sloped or Cylinder (Smooth has its own sides). FBM picks Smooth for you. Rounded with Sloped sides is the default. In Relief the plate sits one layer above the highest point under it, so the rest of the picture keeps its surface. With the plate off, each dot rises from the picture where it sits.

Braille shows in Add text, the workspace, every synthesized view and in 3D (face-up Slim included). It prints on the Relief front (every engine), on face-up Slim and on the Back side of Dual. It cannot go on a face that prints against the plate: on Slim face down, the Dual side on the bed and both Hybrid sides a note explains why and braille stays off. In Focus and on the V8 per-pixel engines it is skipped, with a message saying why.

## ▣ Add imagepage 66

![Add image: Earth placed in front of the Sun. The same way you would add a QR code, a logo or a label.](https://mythaprism.com/manual_assets/m6/t_edit_addimg.jpg)

*Add image: Earth placed in front of the Sun. The same way you would add a QR code, a logo or a label.*

Places a second picture over the print, baked in where you put it: a QR code, a logo, a signature. Drag and scale it over the preview (two fingers rotate it on a phone). It prints in your filament colors like the rest of the picture. A QR code scans reliably from about 30 mm across.

## ⌫ Hole punchpage 66

![Hole punch on Saturn: pick a shape, drag it into place. Red will be cut.](https://mythaprism.com/manual_assets/m6/t_edit_hole.jpg)

*Hole punch on Saturn: pick a shape, drag it into place. Red will be cut.*

Pick a shape (circle, square, triangle, semicircle, trapezoid, diamond, star, pill, heart) and drag it into place, pull the square handle to resize and the round handle to rotate. Or choose **Draw** and click points around any area. Red is what will be cut. Punch as many holes as you like. Holes go all the way through, backing included in the flat modes, and the shareable PDF lists them under *Edits applied*.

## ◐ Reassign bandspage 67

Reassign bands is now an add-on (Pro). See Chapter 8. It no longer needs a color match first: it colors your picture section by section and works out the layers itself.

## ⧠ Dual backingpage 67

![Placing the second picture against a mirrored ghost of the first.](https://mythaprism.com/manual_assets/m6/t_dual_place.jpg)

*Placing the second picture against a mirrored ghost of the first.*

Opens the second-picture flow that Dual and Hybrid Prism use (Chapter 7): **Choose back picture**, place it against a pale mirrored ghost of the front (the front as seen from behind, so what lines up here lines up on the print) use **⇄ Flip horizontal** if the two should read continuously through the part, then **Place picture**.

Dual backing works before a color match too. With a picture in the workspace it opens Dual Prism straight on the second-picture page.

## Lasso, grid and revertpage 68

![The Smooth lasso armed on the stage, the lasso in Brush mode with its size, and the alignment grid.](https://mythaprism.com/manual_assets/m6/t_lasso.jpg)
![The Smooth lasso armed on the stage, the lasso in Brush mode with its size, and the alignment grid.](https://mythaprism.com/manual_assets/m6/ph_lasso_brush.jpg)
![The Smooth lasso armed on the stage, the lasso in Brush mode with its size, and the alignment grid.](https://mythaprism.com/manual_assets/m6/t_grid.jpg)

*The Smooth lasso armed on the stage, the lasso in Brush mode with its size, and the alignment grid.*

**◠ Smooth lasso** and **⊘ Blend lasso** are drawn straight on the stage, as a **Loop** or with the **Brush**: the bar under the *Lasso on* pill switches between them and sets the brush size. With the Brush, each stroke you paint is smoothed or blended the moment you lift. Smooth re-smooths the inside of the loop so hard specks dissolve into their surroundings. Blend floods the nearest outside colors inward so a blemish is grown over. Before a match, and in 2D image editing, both lassos work on the photo itself (one Undo step each). **⊞ Grid S M L** lays a real-millimeter grid over the picture everywhere, including inside the tools, a placement aid that never prints. **↺ Revert all edits** restores the untouched picture (cuts, backgrounds, crops, lasso strokes, spot colors, texts) after a confirmation, and re-runs the match. It can itself be undone.

## Edit tools on the phonepage 68

In the App every tool opens full-screen from the **Edit** sheet, with its controls under the picture. Pinch to zoom inside a tool, one finger drags whatever you placed, two fingers resize and rotate it. The **Photo** sheet's *Quick edits* row jumps straight to Crop, Silhouette, Spot color, Hole punch and Text.

![The same tools on the App (Cut out pieces opens as its own window): Crop, the cut-out, Spot color, Hole punch and Add te](https://mythaprism.com/manual_assets/m6/a_edit2_crop.jpg)
![The same tools on the App (Cut out pieces opens as its own window): Crop, the cut-out, Spot color, Hole punch and Add te](https://mythaprism.com/manual_assets/m6/a_edit2_sil.jpg)
![The same tools on the App (Cut out pieces opens as its own window): Crop, the cut-out, Spot color, Hole punch and Add te](https://mythaprism.com/manual_assets/m6/a_edit2_spot.jpg)
![The same tools on the App (Cut out pieces opens as its own window): Crop, the cut-out, Spot color, Hole punch and Add te](https://mythaprism.com/manual_assets/m6/a_edit2_hole.jpg)
![The same tools on the App (Cut out pieces opens as its own window): Crop, the cut-out, Spot color, Hole punch and Add te](https://mythaprism.com/manual_assets/m6/a_edit2_text.jpg)

*The same tools on the App (Cut out pieces opens as its own window): Crop, the cut-out, Spot color, Hole punch and Add text.*

07

# The six Prism modes

Each mode builds a different physical object from the same match: a glowing relief, a glass-smooth poster, a two-sided keepsake, a sculpted subject over a flat scene, a full-color lithophane, plus 2D image editing, where the picture waits on its own.

## Choosing and launching a modepage 70

![The Dual Prism mode card.](https://mythaprism.com/manual_assets/m6/t_modecard.jpg)

*The Dual Prism mode card.*

Tap a mode on the mode pill (App: a row in the **Modes** sheet) and its card opens: what it builds, how to use it, and what your printer needs. **Launch** switches the print. Undo takes you back to the mode you came from.

| Mode | Plan | Printer |
|---|---|---|
| Relief Prism | Free (monochrome) · Plus · Pro | Any printer |
| Slim Prism · Dual Prism | Plus · Pro | Multi-material |
| Hybrid · Focus · LithoPrism | Pro | Multi-material (LithoPrism: any printer) |
| 2D image editing | Free · Plus · Pro | , (nothing to print) |

## Relief Prism: the classicpage 71

The whole print is a sculpted tonal relief: translucent layers stack up and thickness paints the image, deep stacks for shadows, thin light-capped columns for highlights. Hold it to a window and it glows. It prints on any printer, single nozzle included: only one filament is ever loaded, and you swap at the heights the export lists (or an AMS swaps for you).

![Relief Prism: the synthesized result and the 3D model.](https://mythaprism.com/manual_assets/m6/t_mode_relief.jpg)
![Relief Prism: the synthesized result and the 3D model.](https://mythaprism.com/manual_assets/m6/t_mode_relief_3d.jpg)

*Relief Prism: the synthesized result and the 3D model.*

## Slim Prism: one flat picturepage 72

The picture printed as flat color parts with a glass-smooth face: razor thin, finished in a fraction of the time, with no swap schedule. Each color is its own part and the printer's material system handles the changes.

![Slim Prism on the U.S. flag (V1.8 obj, the default 9 filaments): the flat color parts, the build diagram in Prism contro](https://mythaprism.com/manual_assets/m6/t_mode_slim.jpg)
![Slim Prism on the U.S. flag (V1.8 obj, the default 9 filaments): the flat color parts, the build diagram in Prism contro](https://mythaprism.com/manual_assets/m6/t_prism_slim.jpg)
![Slim Prism on the U.S. flag (V1.8 obj, the default 9 filaments): the flat color parts, the build diagram in Prism contro](https://mythaprism.com/manual_assets/m6/t_mode_slim_3d.jpg)

*Slim Prism on the U.S. flag (V1.8 obj, the default 9 filaments): the flat color parts, the build diagram in Prism control, and the 3D model.*

**Face-down or face-up.** By default the picture prints face-down, so the bed gives it its smooth face, flip it over to view. **Print face-up** puts a backing on the plate and the picture, unmirrored, on top, which is also the side that can carry braille. **No backing** leaves the backing out so the picture shows from both sides, parts then only hold together where colors touch, so an island surrounded by empty space has nothing to hold it.

**Dots on flat faces.** A switch in Print setup (in the app: with the mode options in the Modes and Edit sheets), shown when a print has a flat painted face: Slim, and the flat sides of Dual, Hybrid and Focus. It is OFF by default, and off means solid color areas. ON mixes your filaments in nozzle-size dots for closer colors. It means more filament changes on every layer, so the print takes longer.

**Surface finish.** Face-down, the picture takes on the plate's texture, mirror-smooth on a smooth plate, patterned on a textured one. Face-up, turn on your slicer's **Ironing** for the top surface.

## Dual Prism: a picture on each sidepage 73

Slim Prism doubled: a thin transition layer bridges the flat face and a second, fully independent flat picture on top. Two pictures, one file, no assembly.

![Dual Prism in the Tool: the flowers (Image 1, Zoned V1.8 obj) │ the U.S. flag (Image 2, V1.8 obj), each side with its ow](https://mythaprism.com/manual_assets/m6/t_mode_dual_full.jpg)

*Dual Prism in the Tool: the flowers (Image 1, Zoned V1.8 obj) │ the U.S. flag (Image 2, V1.8 obj), each side with its own Edit pill.*

**Placing the second picture.** Launch Dual and choose the back picture. The placement view shows your first picture as a pale mirrored ghost, the front seen from behind, so aligning against it aligns the real print. Drag to position, scroll or pinch to zoom, double-click to reset, then **Place picture**. **⇄ Flip horizontal** makes the same picture on both faces line up through the part.

**Second image added.** A prompt then asks whether the second picture should **reuse the first picture's palette** or get **a new palette of its own**. A mostly-dark second picture may plan only a few colors: pick its side and raise the Colors count.

![The two faces in 3D, and Prism control drawing the build: Image 2's colors, the transition, Image 1's colors.](https://mythaprism.com/manual_assets/m6/t_mode_dual_3d.jpg)
![The two faces in 3D, and Prism control drawing the build: Image 2's colors, the transition, Image 1's colors.](https://mythaprism.com/manual_assets/m6/t_prism_dual.jpg)

*The two faces in 3D, and Prism control drawing the build: Image 2's colors, the transition, Image 1's colors.*

**The split workspace.** The **Edit image 1 ▾ / Edit image 2 ▾** pills and the IMAGE 1 / IMAGE 2 tags choose a side, the engine, count, presets, Prism Modifiers, spot colors, lassos and text then act on that picture only. The back only exists where the front has material, so nothing can float. **Transition layer** (count and filament, darkest by default) is the slab that joins the faces: raise it to 2 to 3 layers for a stiffer piece. On Plus and Pro it can be set to **0** for a test or control print with no slab at all. A warning explains what can go wrong (pin holes where light comes through, each picture showing through on the other side, and pieces that can tear apart and stay on the build plate), and you can go straight back to the layers you had.

## Hybrid Prism: poster meets sculpturepage 74

Your picture (Image 1) prints as a full relief on top, exactly as you matched and edited it, and a second picture (Image 2, placed with Dual backing) becomes the flat bed printed face-down underneath. Launching Hybrid never re-matches Image 1: its match, edits, modifiers and spot colors carry over untouched. The transition layer doubles as an opacity barrier so the bed can never glow through into the relief. The row shows the effective count it needs.

![Hybrid Prism: Earth as the relief top (Zoned V1.8 obj) and the U.S. flag as the flat bed (V1.8 obj), and the 3D model.](https://mythaprism.com/manual_assets/m6/t_mode_hybrid.jpg)
![Hybrid Prism: Earth as the relief top (Zoned V1.8 obj) and the U.S. flag as the flat bed (V1.8 obj), and the 3D model.](https://mythaprism.com/manual_assets/m6/t_mode_hybrid_3d.jpg)

*Hybrid Prism: Earth as the relief top (Zoned V1.8 obj) and the U.S. flag as the flat bed (V1.8 obj), and the 3D model.*

## Focus Prism: flat behind, sculpted subjectpage 75

One picture split by who is in it: the background prints flat and face-up while the subject (a person, a pet) rises as a full relief on top. **Launch** takes you straight to the subject picker: press ✨ Auto subject, or outline the subject (Tolerance, 🪣 Fill subject, or the outline tools) and press **Use as subject**. **✂ Choose subject** under the 2D/3D switch changes it any time. Every engine works on the subject, and the flat background follows the same engine.

![Choose Focus Subject on a sunflower: the outline hugs the flower and its leaves, and the rainbow tint marks the backgrou](https://mythaprism.com/manual_assets/m6/t_focus_cutter.jpg)

*Choose Focus Subject on a sunflower: the outline hugs the flower and its leaves, and the rainbow tint marks the background that prints flat.*

![Focus Prism on the flowers (V25): the bouquet picked as the subject in the cutter (everything else is the flat backgroun](https://mythaprism.com/manual_assets/m6/t_focus_freehand.jpg)
![Focus Prism on the flowers (V25): the bouquet picked as the subject in the cutter (everything else is the flat backgroun](https://mythaprism.com/manual_assets/m6/t_focus_launch.jpg)
![Focus Prism on the flowers (V25): the bouquet picked as the subject in the cutter (everything else is the flat backgroun](https://mythaprism.com/manual_assets/m6/t_mode_focus_3d.jpg)

*Focus Prism on the flowers (V25): the bouquet picked as the subject in the cutter (everything else is the flat background), the stage, and the bouquet raised over the flat black in 3D.*

## LithoPrism: the full-color lithophanepage 76

A lithophane that is color-matched automatically. The picture becomes a thin translucent relief on a diffuser base: **thickness paints the tones and thin cyan, magenta and yellow layers paint the color.** Hold it to a window or an LED panel and it glows in full color. Front-lit, it reads as a soft relief. For a **classic white lithophane** (one white filament, the picture in its thickness only), pick **White lithophane**, the first row of the LithoPrism menu. It prints like Relief Prism (any printer, one filament at a time with the swap guide, or with an AMS) at 100 % infill with the process the export names.

![The LithoPrism card lists its eight engines, picking one launches the mode, the result, the 3D model and the Litho panel](https://mythaprism.com/manual_assets/m6/t_litho_card.jpg)
![The LithoPrism card lists its eight engines, picking one launches the mode, the result, the 3D model and the Litho panel](https://mythaprism.com/manual_assets/m6/t_mode_litho.jpg)
![The LithoPrism card lists its eight engines, picking one launches the mode, the result, the 3D model and the Litho panel](https://mythaprism.com/manual_assets/m6/t_mode_litho_3d.jpg)

*The LithoPrism card lists its eight engines, picking one launches the mode, the result, the 3D model and the Litho panel.*

With a picture loaded, tap **Litho** on the mode pill (App: the LithoPrism row). The card lists the eight LithoPrism engines, **V8 Litho** (back-lit, vivid, thin base), **V2·V8 Litho** (back-lit, fine detail, max color) and **V34 Litho** / **V34.1 Litho** (CMYK clean: no dither, clean layers and a smooth surface). Pick one and the mode launches and matches at once. While it's on, the Color match menu shows a **LithoPrism** tab for switching engines and the **Litho panel** appears in Print setup: **Diffuser base** thickness, **Add a border frame**, **Add a hanging hole (top tab)** and **Export calibration tile (.3mf)**. Picking any other engine or mode leaves LithoPrism.

![The Litho panel.](https://mythaprism.com/manual_assets/m6/t_litho_panel.jpg)

*The Litho panel.*

## 2D image editing: just the picturepage 78

The first place in the mode bar (left of Relief, and the top row of the App’s Modes sheet) is not a print, and it is where every new picture lands. **2D image editing** locks the workspace to the picture: the view stays on Prime, the 2D / 3D switch, the other views and the matcher step aside, and every edit tool, Prism Modifier, **Filters** look and **Cut out pieces** change lands on the picture alone. Nothing is re-matched while you are in it, and the print-file exports wait (Save → **Save edited prime image (.png)** keeps the picture).

The card

Tool

App

![The 2D image editing card and the mode on the Tool and on the phone. A bar on the stage says the print waits.](https://mythaprism.com/manual_assets/m6/t5_modecard_2d.jpg)
![The 2D image editing card and the mode on the Tool and on the phone. A bar on the stage says the print waits.](https://mythaprism.com/manual_assets/m6/t5_mode2d_tool.jpg)
![The 2D image editing card and the mode on the Tool and on the phone. A bar on the stage says the print waits.](https://mythaprism.com/manual_assets/m6/a5_mode2d.jpg)

*The 2D image editing card and the mode on the Tool and on the phone. A bar on the stage says the print waits.*

**If you already color matched**, opening the mode takes you straight to the 2D picture. Your print waits exactly as it was. Leave with **Back to the print** on the stage bar, or pick any Prism mode in the bar: if the picture changed while you were editing, the print re-matches once with your engine. If it did not, it comes back untouched. With no match yet, 2D image editing is simply the photo editor (Chapter 3) with nothing else on screen.

**It opens by itself.** When you drop in a picture (or take one with the App’s camera) the workspace opens straight in 2D image editing, because most people edit first and color match second. Opened this way there is no print yet, so there is no *Back to the print* button. The bar just says *color match when you are ready*. Press **Color match** (or pick an engine, or a Prism mode in the bar) and the mode steps aside and matches the edited picture. Open it again after a match and it works as described above: the print waits and **Back to the print** takes you back.

**Every Prism Modifier works here**, including Sharpness, Clarity, De-Blotch and the Island smoother, which used to show only on the print. They run the same filters the color matchers run on their input, so the picture you see is the picture that gets matched, and **Save edited prime image** bakes them in. The **◠ Smooth** and **⊘ Blend** lassos work on the picture too, drawn as a loop or with the brush: Smooth dissolves stray specks into the colors around them, Blend grows the surrounding colors over the selection and smooths the seams.

It is on every plan. On Free the edits are the Free ones, crop and Tone / Brightness / Contrast.

08

# Add-ons

Seven switches that change what one photo becomes: a jigsaw puzzle whose pieces really lock, a set of prints cropped from one photo, Filters looks for the photo, the Image Simplifier, which shows the photo in fewer colors made from your own filaments, Image Grading for the photo’s color and light, a mural bigger than your printer, cut into labeled tiles and sized against real-world objects, and Reassign bands, where you color the picture yourself and MythaPrism works out the layers.

## Puzzle cutpage 80

![The Puzzle cut page, the 4 × 5 cut on the stage, and the same print in 3D.](https://mythaprism.com/manual_assets/m6/t_addon_puzzle.jpg)
![The Puzzle cut page, the 4 × 5 cut on the stage, and the same print in 3D.](https://mythaprism.com/manual_assets/m6/t_puzzle_stage.jpg)
![The Puzzle cut page, the 4 × 5 cut on the stage, and the same print in 3D.](https://mythaprism.com/manual_assets/m6/t_puzzle_3d.jpg)

*The Puzzle cut page, the 4 × 5 cut on the stage, and the same print in 3D.*

Switch **Puzzle cut** on in Add-ons and press **✎ Edit**. **Across** and **Down** set the grid (4 × 5 by default), **Gap** sets the clearance between pieces. The achieved value is reported, and below about 0.3 mm the Tool warns that pieces will fuse. **Tray** adds a snug frame that exports as its own part. The tabs genuinely lock: every tab's neck is narrower than its bulb, and they alternate along every edge. Puzzle cut works in every print mode, and the colors never change, the cut only removes material between pieces. It is included in every plan, Free too.

The shareable PDF of a puzzle adds a labelled piece map with the piece count and size, and short notes on how to print it and how to solve it.

## Multi croppage 80

![Multi crop: three crops of one photo, each with its own framing and corners.](https://mythaprism.com/manual_assets/m6/t_addon_multi.jpg)

*Multi crop: three crops of one photo, each with its own framing and corners.*

**Multi crop** makes three versions of the picture at once (**Original**, **200 × 200** and **Bookmark 50 × 150**) each with its own pan, zoom and corner rounding. **Create 3 crops** and each crop is matched as a print of its own with the engine and settings you are using, in every mode: in Dual and Hybrid the second picture is cropped through the same window, in Focus the subject follows, and texts and spot colors follow too.

The thumbnail bar under the stage switches crops instantly. Each keeps its own result. Change the engine or a setting and the crop you're looking at re-matches at once, the others when you switch to them or export. **Export** writes one `.3mf` with three plates. The one-stack engines share one swap schedule across the plates, the zoned and CMYK engines give each plate its own parts, exactly as you saw them. Multi crop cannot be on together with Mural (see Mural below). Plus and Pro.

## Filterspage 82

![Filters in the Tool (left: Solid Color Fill V2 with the Compare divider) and on the phone (right: Ink Comic Shaded).](https://mythaprism.com/manual_assets/m6/t5_filterlab_tool.jpg)
![Filters in the Tool (left: Solid Color Fill V2 with the Compare divider) and on the phone (right: Ink Comic Shaded).](https://mythaprism.com/manual_assets/m6/a5_filterlab.jpg)

*Filters in the Tool (left: Solid Color Fill V2 with the Compare divider) and on the phone (right: Ink Comic Shaded).*

**Filters** puts a look on the whole photo. Switch it on in Add-ons and its page opens on your picture with **Solid Color Fill** chosen, and **every look shown as a live thumbnail of your own photo**, the Original plus 310 looks, so you choose by eye. On a phone the thumbnails are drawn as you scroll to them, which saves battery.

**Red & Black** turns the photo into black shadows and red tones, the way a picture prints with only a black and a red filament loaded. Use it before a two-filament match (Black + Red): the print reads like the look, and Effect sets how deep the blacks go.

![Filters with Red & Black picked on the flowers: the look a black and a red filament can print.](https://mythaprism.com/manual_assets/m6/b590_filters_redblack.jpg)

*Filters with Red & Black picked on the flowers: the look a black and a red filament can print.*

![All 310 looks and the Original on one photo, in the order the page shows them.](https://mythaprism.com/manual_assets/m6/t5_filterlab_all38.jpg)

*All 310 looks and the Original on one photo, in the order the page shows them.*

**The looks.** All 310, in the order the Filters page shows them (the Original comes first):

| Look | What it does |
|---|---|
| **Solid Color Fill** | Each color area filled with one flat color, the simplest picture to color match. |
| **Solid Color Fill V2** | A smarter flat fill: neighboring areas of the same color merge into clean shapes. |
| **Rotoscope** | Flat painted areas with thin dark outlines, like traced animation. |
| **Cel** | A few flat colors with crisp black ink lines, like a classic animation cel. |
| **Soft Toon** | Smoothed color with lightness in soft steps and gentle gray lines. |
| **Bold Ink** | Six bold colors and thick black outlines. |
| **Two Tone** | Every color area gets one lit tone and one shadow tone, with ink lines. |
| **Painted Toon** | Brushy painted areas with light ink lines. |
| **Pop Dots** | Comic print dots in each area's own color on a pale tint, with ink lines. |
| **Noir Ink** | Black and white only, solid blacks and hatched middle tones. |
| **Color Sketch** | Pencil lines over soft flat color on white paper. |
| **Filament Toon** | Cartoon areas snapped to colors the starter filaments really print, with black outlines. |
| **Polygon Geometric** | The picture rebuilt from flat geometric facets. |
| **Neon Lights** | Glowing neon edges on a dark ground. |
| **Neon Night** | A night-time grade with bright neon outlines. |
| **Crisp Line Art** | Clean dark lines on white, great for a two-color print. |
| **Bold Line Art** | Thicker, confident ink lines. |
| **Ink Outline** | Only the ink lines. Everything else turns transparent. |
| **Graphite Pencil** | A soft pencil sketch in gray tones. |
| **Grayscale** | Plain black-and-white tones. |
| **Monochrome 1-Bit** | Pure black and white, no gray, the boldest two-filament look. |
| **Dithered Mono** | Black and white with an ordered dot pattern for the mid-tones. |
| **High-Contrast B&W** | Hard, punchy black and white. |
| **Red & Black** | Black shadows and red tones, how a picture prints with only a black and a red filament. |
| **Cyanotype Blueprint** | The blue-and-white look of an old blueprint print. |
| **Edge Vignette** | Darkens the corners so the eye goes to the middle. |
| **Acrylic Oil Paint** | Painterly brush patches with soft edges. |
| **Neon Split Tone** | Magenta and cyan split toning. |
| **Retro 4-Color Computer** | The four-color palette of an early home computer. |
| **Solarize Blend** | Bright tones flip over, a darkroom effect. |
| **Thermal Vision** | A heat-camera color ramp. |
| **Teal & Copper Duo** | Two-color film grade: teal shadows, copper highlights. |
| **Posterize Tone** | Hard tone steps like a screen-printed poster. |
| **Cold City Film** | A cold, moody film grade. |
| **Selective Blur** | Softens the picture while keeping the strong edges. |
| **High-Pass Sharpen** | Crisper edges and fine detail. |
| **Interlaced Video Tape** | Scan lines and color bleed of an old tape. |
| **Ink Comic Shaded** | Comic-book inks with flat shaded colors. |
| **Digital Glitch** | Shifted, torn rows of a corrupted signal. |
| **Pro Halftone** | Printed-comic halftone dots. |
| **Clean Sketch** | A clean pencil-sketch drawing. |
| **Pixel Raster** | Big square pixels: retro pixel art. |
| **Flat Toon Shaded** | Cartoon cel shading with flat tones. |
| **Rosey Romantic** | A warm, rosy soft grade. |
| **Vintage Noir** | Old black-and-white film with deep blacks. |
| **Timeless Sepia** | Warm brown antique tones. |
| **Invert Color Phase** | Every color flipped to its opposite. |
| **Anaglyph 3D** | Red / cyan offset like 3D glasses. |
| **Kuwahara Painting** | Smooth painted color patches that keep every edge sharp. |
| **Watercolor Wash** | Soft transparent washes, pigment pooling at the edges and paper grain. |
| **XDoG Ink Drawing** | Clean ink lines and solid ink shadows, like a hand-inked drawing. |
| **Cross-Hatch Pencil** | Layers of crossing pencil strokes, more layers where it is darker. |
| **Stipple Dots** | The picture drawn from thousands of ink dots. |
| **Stained Glass** | Glowing glass panes held together by dark lead lines. |
| **Mosaic Tiles** | Square ceramic tiles with grout lines and bevelled edges. |
| **CMYK Color Halftone** | Four rotated ink-dot screens, like a printed magazine up close. |
| **Pop Art Quad** | The picture four times in bold pop-art palettes. |
| **Pixel Sort** | Glitch-art streaks: runs of pixels sorted by brightness. |
| **Dreamy Glow** | A soft dreamy glow over the sharp picture. |
| **Emboss Relief** | The picture pressed into metal, lit from the top left. |
| **Cinematic Teal & Orange** | Teal shadows and warm highlights, the blockbuster movie grade. |
| **Vintage Film** | Faded film colors, grain, a vignette and a light leak. |
| **Tilt-Shift Miniature** | A sharp band in the middle and blur above and below: a toy-model look. |
| **Charcoal Drawing** | Soft smudged charcoal on textured paper. |
| **Woodcut Print** | Carved wavy lines in black ink on cream paper. |
| **Handheld 4-Shade Green** | Chunky pixels in the four greens of an old handheld game screen. |
| **Infrared Film** | False-color infrared: leaves turn red and pink. |
| **Night Vision** | Green night-vision scope with glow, noise and scan lines. |
| **ASCII Text Art** | The picture redrawn with text characters. |
| **Two-Ink Stencil Print** | Two fluorescent inks, grainy and slightly misaligned. |
| **Low-Poly Triangles** | Triangles that follow the outlines, each in its average color. |
| **Edge-Preserving Smooth** | Flat areas melt smooth while edges stay crisp. |
| **Egyptian Papyrus Painting** | Ancient tomb-painting colors and bold outlines on papyrus, with a painted border. |
| **Pharaoh Gold & Lapis** | A gold-leaf relief with lapis-blue shadows, framed in picture-writing. |
| **Low Poly Fighter** | Chunky smooth-shaded polygons like a late-90s console fighting game. |
| **Retro Polygon Console** | Low resolution, blurry console texture filtering and 15-bit color. |
| **Chromatic Aberration** | Red and blue fringes split apart toward the edges. |
| **Zoom Burst** | Streaks rushing toward the middle, like a zoom pull. |
| **Kaleidoscope** | The picture mirrored round the center. |
| **X-Ray** | Dense areas glow cold blue like an X-ray film. |
| **Bleach Bypass** | Low color, high contrast silver film look. |
| **Cel Shading** | Three flat light bands and clean ink lines, like animation cels. |
| **Colored Pencil** | Colored pencil strokes on white paper. |
| **Chalkboard** | Dusty chalk drawing on a green slate board. |
| **Toy Camera Cross-Process** | Wild cross-processed film colors with dark toy-camera corners. |
| **Auto Enhance** | Fixes dull photos: each color stretched to its full range. |
| **Auto White Balance** | Removes a color cast so whites and grays look neutral. |
| **Red-Filter B&W** | Black and white through a red filter: dark dramatic skies, bright skin. |
| **Bump Relief (Color)** | Keeps the colors and lights every shape like raised plaster. |
| **Clarity Boost** | Local contrast boost: detail and texture pop. |
| **Concentrate** | Crisp colorful middle, softer paler edges, so the eye goes to the center. |
| **Edge Detect** | Bright colored edges on black, the classic edge-detect filter. |
| **Glowing Edges** | Thick edges glowing in the picture’s own colors on black. |
| **Glowing Sun** | Warm sunlight pouring in from the top left with a soft flare. |
| **Grungy** | Gritty: low color, hard contrast, dirt, specks and scratches. |
| **Old Paper** | A faded sepia print on stained, yellowed paper. |
| **Pinhole Camera** | Soft black and white with heavy round vignette and blurred corners. |
| **Instant Photo** | Faded warm instant-camera print in a white frame. |
| **Color Splash Noir** | Hard black and white with only the reds kept in color. |
| **Three-Strip Color** | The rich saturated color of old three-strip film cameras. |
| **Classic Faded** | Muted, faded colors with soft blacks, a quiet literary look. |
| **Retro Slide Film** | Punchy 60s color slide film with deep shadows. |
| **Warm Kelvin** | Strong warm orange 70s cast. |
| **Love Glow** | Warm pink romantic glow. |
| **Nostalgia** | Faded old print with grain and dark corners. |
| **Orange Peel** | Bright juicy orange highlights with teal shadows. |
| **Pleasant Pastel** | Light, airy, gently pastel colors. |
| **Sunrise** | Golden-pink sunrise light with violet shadows. |
| **Muted Green Film** | Low-saturation film look with green-tinted shadows. |
| **Hazy Days** | Soft summer haze: lifted, low contrast, dreamy. |
| **Neon Tube Pink and Blue** | Traces the outlines as glowing pink and blue neon tubes on a dark night. |
| **Neon Sign on Brick** | Turns the picture into a neon sign in its own colors, lighting up a dark brick wall. |
| **Synthwave Sunset Grid** | Paints the picture in sunset neon colors over a glowing retro grid floor. |
| **Plasma Arcs** | Sends crackling blue electric arcs along the shapes of the picture. |
| **Aurora Wash** | Washes the picture with green and blue curtains of northern lights. |
| **Holographic Foil** | Turns the picture into shimmering rainbow foil that shifts with every curve. |
| **Molten Chrome** | Recasts the picture as polished liquid metal reflecting a cool sky. |
| **Bokeh Night Lights** | Melts the picture into a dreamy night of soft out of focus light discs. |
| **Glowing Contour Lines** | Draws the picture as glowing rainbow contour lines like a neon map. |
| **Dual Rim Light** | Lights the picture from both sides with blue and coral stage rim lights. |
| **Anamorphic Flare Bloom** | Blooms the highlights and stretches them into long blue cinema flare streaks. |
| **Star Ray Sparkle** | Adds sparkling star bursts with long rays to the brightest highlights. |
| **Cyber HUD Overlay** | Shows the picture through a glowing teal heads up display with a target ring. |
| **Fluorescent Poster** | Prints the picture in glowing fluorescent poster inks with bold outlines. |
| **Light Web Lines** | Connects the key points of the picture with a glowing web of light lines. |
| **Glowing Ridge Lines** | Redraws the picture as rows of glowing lines that rise with the light. |
| **Classic Blueprint** | Draws the picture as white lines on a deep blue sheet with a faint grid, a frame and a title block. |
| **Architect Sheet** | Turns the picture into blue ink lines and shadow hatching on white drafting paper with a ruled grid. |
| **Reverse Blueprint** | Prints dark ink lines on pale blue paper with ruler ticks along the edges and measuring crosses. |
| **Two Ink Print** | Prints the picture in red and black ink on cream paper with a slight press offset. |
| **Red Ground Ink** | Cuts the picture in bold black ink lines across a red ground, thicker where the picture is darker. |
| **Scratchboard** | Scratches the picture out of solid black as fine white lines that follow the light. |
| **Copper Plate Engraving** | Renders the picture as swelling engraved lines that bend with its forms like an old banknote portrait. |
| **Etching** | Draws the picture with fine wavering hatches in sepia ink on a toned plate with a pressed border. |
| **Topographic Contours** | Reads the picture as a landscape and draws brown contour lines over soft map colors. |
| **Technical Pen** | Builds the picture from crisp ruled hatching, bold outlines and spotted solid blacks in one pen weight. |
| **White Chalk on Black** | Sketches the picture in grainy white chalk lines and hatching on black paper. |
| **Deep Stone Relief** | Carves the picture deep into gray stone lit from the upper left. |
| **Brushed Metal Relief** | Presses the picture into a sheet of brushed steel with a soft sheen. |
| **Gold Foil** | Stamps the picture in raised gold foil with bright glints on the edges. |
| **Copper with Patina** | Raises the picture in warm copper with blue green patina settled into the hollows. |
| **Debossed Paper** | Presses the shapes of the picture into thick white cotton paper with no ink at all. |
| **Thin Clean Edges** | Traces only the true edges of the picture as thin gray lines on white. |
| **Colored Edges** | Outlines the picture in lines colored by the picture itself on pale paper. |
| **Cathedral Glass** | Turns the picture into deep jewel toned glass pieces held in thick dark lead with painted detail. |
| **Sunlit Glass** | Glowing glass with rippled texture and light spilling over thin lead lines as if the sun shines through. |
| **Leaded Panels** | Cuts the picture into flat glass panels whose lead lines follow the shapes in the photo. |
| **Frosted Window** | A pale frosted glass window with soft panes, icy grain and clear water drops. |
| **Two Color Woodcut** | Black carved lines that bend with the shapes over a red tone block on warm paper. |
| **Color Woodblock** | A flat color woodblock print with soft inks, dark outlines and fine wood grain in every color. |
| **Linocut Gouges** | Black ink with white gouge marks carved along the forms, more cuts where the picture is light. |
| **Screen Print** | Three flat inks pulled slightly off register on cream paper, with bright gaps and dark overlaps. |
| **Letterpress** | Navy ink and a red dot plate pressed deep into thick cotton paper with a salty ink texture. |
| **Paper Cut Layers** | Stacks the picture as layers of cut colored paper that cast soft shadows on the sheets below. |
| **Stencil Spray** | A street stencil sprayed on a concrete wall in black and one bold color with grainy edges and drips. |
| **Hexagon Tiles** | Glazed hexagon tiles with a shine in each corner set in pale grout. |
| **Cross Stitch** | Stitches the picture as little colored crosses of thread on light cloth. |
| **Patchwork Quilt** | Sews the picture from patterned fabric patches with puffy seams and running stitches. |
| **Pointillism** | Paints the picture in thousands of pure color dots that mix in the eye. |
| **Impressionist Strokes** | Layers short loaded brush strokes that follow the forms, broad first and then fine. |
| **Oil Pastel** | Waxy oil pastel hatching on dark paper, with the paper tooth showing between the strokes. |
| **Egyptian Sunk Relief** | Your picture cut into pale limestone with faint traces of old paint. |
| **Egyptian Blue Faience** | Glossy turquoise glaze that pools deep blue in the hollows, with fine dark painted lines. |
| **Greek Black-Figure Pottery** | Black slip shapes on orange terracotta with scratched detail lines and a key pattern band. |
| **Greek Red-Figure Pottery** | Terracotta shapes left bare on a black slip ground, shaded with thin brown glaze. |
| **Roman Fresco** | Earth pigments on lime plaster, softly brushed, with fine cracks and worn patches. |
| **Roman Floor Mosaic** | Rows of small cut stone tiles in marble, ochre and slate set in mortar. |
| **Japanese Woodblock Print** | Flat color blocks with crisp black keylines, a soft graded sky and paper grain. |
| **East Asian Ink Wash** | Soft black ink tones bleeding into warm fibrous paper, with open empty space. |
| **Blue-and-White Porcelain** | Cobalt blue brushwork under a glossy white glaze with a ruled ring border. |
| **Persian Miniature Painting** | Jewel bright mineral colors and gold, fine outlines and a gold flecked ruled margin. |
| **Zellige Geometric Tiles** | Hand cut glazed tiles in octagons and squares, each one a single rich color. |
| **Celtic Knotwork Border** | Your picture framed by an over and under woven gold interlace band. |
| **Illuminated Manuscript** | Bright mineral colors on vellum framed by burnished gold leaf and painted bars. |
| **Art Nouveau Poster** | Soft lithograph colors, flowing brown outlines and a rounded double frame. |
| **Art Deco Gold and Black** | Stepped tones of gleaming gold on black with sunburst rays and a geometric frame. |
| **Indian Block Print** | Madder red, indigo and black hand stamped on cotton, with a dotted ground and striped edges. |
| **Andean Woven Textile** | Warp faced weaving in cochineal red, gold, indigo and natural wool with stepped bands. |
| **Woven Strip Cloth Colors** | Narrow handwoven strips in gold, green, red and black, sewn edge to edge. |
| **RGB Tear Glitch** | Rows tear sideways and the red and blue channels slide apart. |
| **Block Smear** | Blocks of the picture drag and smear like a broken video stream. |
| **Pixel Melt** | Bright parts of each column are sorted so the light drips down. |
| **Slit Scan Stretch** | Thin slices of the picture stretch into long streaks of color. |
| **Water Ripple** | Rings spread across the picture like a stone dropped in still water. |
| **Swirl** | The middle of the picture spins into a smooth whirlpool. |
| **Fisheye Lens** | A round wide lens that swells the middle and bends the edges. |
| **Mirror Halves** | The left half folds over the right for a perfect mirror image. |
| **Hex Kaleidoscope Lens** | A honeycomb of little kaleidoscopes, each folding the picture under it. |
| **CRT Phosphor Screen** | An old tube screen with curved glass, scan lines and glowing phosphor stripes. |
| **Tape Tracking Error** | A worn tape with a torn tracking band, static and smeared color. |
| **Dot Matrix Printout** | Printed in ribbon dots on striped tractor feed paper. |
| **Thermal Receipt** | A store receipt print with fine dots, an uneven fade and a dead line. |
| **Photocopy** | A copy of a copy with harsh toner, speckles and dirty streaks. |
| **Broadcast Text Blocks** | Chunky two by three mosaic blocks in bold screen colors. |
| **Falling Code** | Columns of glowing green symbols rain down and draw the picture. |
| **Hologram Scan** | A glowing cyan projection with scan lines and flickering bands. |
| **Impasto Paint** | Thick oil paint with raised brush ridges catching the light. |
| **Ink Splatter** | Bold black ink with splashes and drips over a soft color wash. |
| **Double Exposure** | Your picture blended with a misty pine valley. |
| **Light Leak** | Warm film flare bleeding in from the edges. |
| **Kraft Paper** | Dark ink and white chalk drawn on brown paper. |
| **Sketchbook Page** | Pencil study on a cream page with a coffee ring. |
| **Manga Screentone** | Clean ink lines with flat dot screen shading. |
| **Cubist Facets** | Broken angular planes in earthy tones. |
| **Color Blocks** | Flat rectangles of color that get smaller where the picture is busy. |
| **Folded Paper** | Triangles of folded paper catching the light at different angles. |
| **String Art** | Colored thread strung between nails on a dark wood board. |
| **Satin Stitch** | Embroidered in silky thread with stitches running every way. |
| **Pastel on Dark Paper** | Soft chalk pastel strokes on dark textured paper. |
| **Atlas Map** | Brightness drawn as land, sea and contour lines on an old map. |
| **Dotted Grid Blueprint** | Draws the picture in crisp white ink lines on deep blueprint blue with a dotted grid. |
| **Hidden Line Blueprint** | Draws solid white outlines, dashed hidden lines for the inner shapes and long and short center lines on a mottled blue sheet. |
| **Drafting Dimensions** | Traces the picture in cyan on a navy drafting sheet and measures it with dimension lines, arrowheads and leader balloons. |
| **Faded Old Blueprint** | Ages the blueprint with sun faded blue, worn fold creases, yellowed stains and soft broken white lines. |
| **Isometric Blueprint** | Builds the picture from white hatching along the three isometric directions over a dotted triangle grid on blue. |
| **Patent Drawing** | Draws the picture as clean black outlines with heavier shade lines on the shadow side and stippled dots for the shading. |
| **Isometric Cubes** | Rebuilds the picture from small isometric cubes with a lit top and two shaded sides. |
| **Circuit Board** | Turns the picture into a green circuit board with traces along its edges, gold pads and copper fill in the light areas. |
| **Oscilloscope Trace** | Draws the picture as a glowing green beam trace on a dark scope screen with a measuring graticule. |
| **Radar Sweep** | Shows the picture as blocky radar echoes on a round green scope with range rings and a fading sweep. |
| **Side Scan Sonar** | Paints the picture as a copper sonar scan of the sea floor with speckled ping lines, acoustic shadows and a dark center track. |
| **Weather Map** | Reads the picture as a pressure chart with sweeping isobars, pale coastlines, a front with triangles and half circles and high and low marks. |
| **Microscope Slide** | Shows the picture through a round microscope field as a pink and blue stained tissue sample with cells and nuclei. |
| **Spectrogram** | Shows the picture as a sound spectrogram made of bright frequency bins with axes and a color scale bar. |
| **Streamline Hatching** | Shades the picture with ink strokes that flow along its shapes like a flow field plot. |
| **Section Cutaway** | Cuts the picture into shapes filled with drafting section patterns, cross hatch, slanted lines, gravel dots and open white, with bold outlines. |
| **Technical Illustration** | Redraws the picture like a product manual illustration with stepped warm to cool shading, white highlights and thin dark outlines. |
| **Narrowband Nebula** | Turns the picture into glowing gas clouds in the gold and teal colors of narrowband sky photos. |
| **Dust Pillar Silhouette** | Carves the picture out of dark cosmic dust with glowing rims against a bright nebula. |
| **Spiral Galaxy Swirl** | Winds the picture into a glowing spiral galaxy with a bright core and starry arms. |
| **Blue Reflection Nebula** | Turns the picture into a soft blue starlit haze with feathery dust and bright young stars. |
| **Planetary Nebula Ring** | Sets the picture inside a glowing ring nebula with a teal heart and a red outer rim. |
| **Galactic Star Band** | Turns the picture to night with a glowing band of our galaxy rising behind it. |
| **Nebula Double Exposure** | Fills the bright parts of the picture with a red and teal nebula full of stars. |
| **Supernova Burst** | Blasts the picture outward from a blinding star into a glowing shell of hot gas. |
| **Telescope Starlight** | Grades the picture to deep space and gives its highlights six point telescope star spikes. |
| **Gravity Lens Ring** | Bends the picture around a heavy galaxy into a glowing ring and curved arcs. |
| **Planet Globe** | Wraps the picture onto a lit planet with a glowing blue air rim over a starry sky. |
| **Cratered Moon** | Turns the picture into gray moon dust lit low from the side, pocked with craters. |
| **Red Planet Dust** | Paints the scene in rusty desert reds under drifting butterscotch dust haze. |
| **Planet Rings** | Sweeps a tilted ring system with fine ringlets and gaps across the picture. |
| **Orbit Diagram** | Lays glowing orbit paths, dotted transfer arcs and planet markers over a deep blue picture. |
| **Space Age Poster** | Recasts the picture as a flat color travel poster with a big sun, a ringed planet and sparkles. |
| **Station Monitor** | Shows the picture on a station console screen beside live graphs drawn from its own tones. |
| **Helmet Visor** | Reflects the picture in a curved gold helmet visor framed by a white helmet shell. |
| **Comet Streak** | Dims the scene to night and sends a bright comet across it with blue and gold tails. |
| **Twin Sun Sunset** | Lights the scene with two setting suns, a warm alien sky and doubled soft shadows. |
| **Rain on Glass** | Raindrops on a window bend the picture upside down and leave clear trails through the misted glass. |
| **Snowfall** | Soft snow drifts down in front of a cool winter version of the picture. |
| **Morning Fog** | Low layers of warm morning fog drift through the picture and soften the distance. |
| **Burning Edges** | The picture burns in from its edges with glowing embers and charred paper. |
| **Lake Reflection** | The picture stands on the shore of a still lake and its rippled reflection fills the water below. |
| **Underwater Light** | Sunlight ripples in bright nets over a blue green picture seen through moving water. |
| **Polished Marble** | The picture turns into polished marble with flowing veins, pale where it is light and dark where it is dark. |
| **Wood Burned Art** | The picture is burned into a pale wooden plank in brown and black tones. |
| **Carved Wood Relief** | The picture is carved into warm oak with deep shadows and raised highlights. |
| **Rusted Steel** | The picture shows through a sheet of brushed steel eaten by orange rust. |
| **Cracked Dry Earth** | The picture dries into curled clay plates split by deep cracks. |
| **Crystal Facets** | The picture is seen through a cut crystal that shifts each facet and splits light at the edges. |
| **Autumn Leaves** | Greens turn red and gold in warm autumn light while leaves drift across the picture. |
| **Lightning Storm** | A dark storm grade with forked lightning that lights up the picture. |
| **Sunbeams and Dust** | Golden beams of light stream through the picture with dust floating in them. |
| **Soap Bubbles** | Floating soap bubbles shimmer with swirling film colors and bend the picture inside them. |
| **Tintype** | Turns the picture into a silver gray tintype on black iron with dark collodion flow marks around the edges. |
| **Daguerreotype** | Shows the picture on a cool silver mirror plate with a colored tarnish halo inside a brass oval mat. |
| **Salt Print** | Prints the picture in soft reddish brown sunk into matte paper fibers with faded edges. |
| **Gum Pigment Print** | Builds the picture from three brushy pigment layers of blue, red and ochre printed slightly out of register. |
| **Lith Print** | Gives the picture grainy warm peach highlights and deep hard black shadows like a lith darkroom print. |
| **Color Screen Plate** | Rebuilds the picture from tiny orange, green and blue grains like an early color glass plate. |
| **Hand Tinted Print** | Makes a warm black and white print and brushes soft pastel tints over it a little off the lines. |
| **Darkroom Print** | Prints the picture in rich black and white with a dodged center, burned edges and a ragged black rim on white paper. |
| **Sabattier Reversal** | Partly reverses the tones like a print flashed in the darkroom and draws thin bright lines along every border. |
| **Contact Sheet Frame** | Places the picture in a frame of a film strip with sprocket holes and a red grease pencil mark around it. |
| **Prism Refraction** | Shoots the picture through a glass prism with a rainbow ghost of the bright parts and a spectrum over one corner. |
| **Panning Blur** | Keeps the middle of the picture sharp while the rest streaks sideways like a camera panning with a moving subject. |
| **Soft Focus Pictorial** | Paints the picture in glowing soft focus with gentle green gray tones that fade to paper at the edges. |
| **Glass Plate Negative** | Shows the picture as an old amber glass negative with silvered edges, a crack and a chipped corner on a light box. |
| **Photogravure** | Prints the picture in velvety warm black aquatint grain inside a pressed plate mark on cream paper. |
| **Swiss Grid Poster** | Splits the picture into a strict grid of flat gray modules with one bold red field and a black rule. |
| **Modernist Shapes** | Rebuilds the picture from circles, squares and triangles in red, yellow, blue and black on cream. |
| **Op Art Rings** | Draws the picture with black and white rings that swell and bend with its light and dark. |
| **Memphis Pattern Poster** | Flat candy colors with black outlines, polka dots, stripes and confetti squiggles filling the shapes. |
| **Flat Long Shadow** | Flat vector colors where every lighter shape throws a long diagonal shadow. |
| **Coloring Book Page** | Bold, clean, closed outlines on white paper, ready to color in. |
| **Die Cut Sticker** | Turns the picture into a glossy sticker with a white border, a soft shadow and a peeling corner. |
| **Three Tone Halftone** | Prints the shadows as black dots and the light as white dots on one bold flat color. |
| **Squiggle Line Portrait** | Draws the picture with rows of a wavy pen line that wiggles faster and wider in the dark parts. |
| **Triangle Grid Poster** | Flat colored triangles on a regular grid that split smaller where the picture has detail. |
| **Split Complementary Poster** | Recolors the picture in five flat poster tones built from its main hue and the two hues beside its opposite. |
| **Seventies Stripes** | Warm retro stripes in brown, rust, orange, mustard and cream that bend around the shapes. |
| **Crayon Drawing** | Colors the picture in waxy crayon scribbles with white paper peeking through and dark crayon outlines. |
| **Tattoo Flash** | Thick black outlines and a few bold classic colors with dotted black shading on aged paper. |
| **Stamp Pattern Repeat** | Cuts the picture into a one color block stamp and prints it in a repeating pattern in two inks. |
| **Sketchnote Marker** | Black pen lines, two gray markers and a bright highlighter on dotted notebook paper. |
| **Stud Bricks** | Builds the picture from toy bricks with round studs in bright plastic colors. |
| **Glass Marbles** | Packs the picture into shiny glass marbles that each show a tiny flipped view. |
| **Air Bubble Sheet** | Lays a sheet of shiny air bubbles over the picture with each bubble magnifying it. |
| **Modeling Clay** | Sculpts the picture in soft rounded modeling clay with thumbprints and deep creases. |
| **Felt Applique** | Cuts the picture from fuzzy wool felt shapes sewn down with a running stitch. |
| **Sidewalk Chalk** | Draws the picture in bright pastel chalk on rough gray pavement. |
| **Flow Field Lines** | Redraws the picture as flowing pen lines that follow its shapes like a plotter drawing. |
| **Truchet Tiles** | Weaves the picture from random quarter circle tiles whose lines thicken in the shadows. |
| **Maze Drawing** | Turns the picture into one big solvable maze whose walls grow thick in dark areas. |
| **Woven Photo Strips** | Cuts the picture into paper strips and weaves a color copy over and under a sepia copy. |
| **Circle Packing** | Fills the picture with snug flat circles, big in calm areas and tiny on the details. |
| **Jigsaw Puzzle** | Cuts the picture into raised jigsaw puzzle pieces with one piece still missing. |
| **Crackle Glaze** | Glazes the picture like glossy pottery with a fine web of stained crackle lines. |
| **Gummy Candy** | Casts the picture in glowing see-through gummy candy with glossy rounded edges. |
| **Candy Sprinkles** | Rebuilds the picture from thousands of shiny candy sprinkles scattered on top. |
| **Numbered Paint Sheet** | Turns the picture into a numbered painting sheet with outlined areas and tiny color numbers. |

![The rail: the looks, Adjust, Filaments and the result colors. (Older screenshot: the Color grading sliders shown here no](https://mythaprism.com/manual_assets/m6/t5_filterlab_grading.jpg)

*The rail: the looks, Adjust, Filaments and the result colors. (Older screenshot: the Color grading sliders shown here now live in Image Grading.)*

**Adjust.** **Effect** (0 to 200 %) is the look's own strength setting, **Strength** (0 to 100 %) blends the look back toward the photo.

**Color and light.** Grading the photo (temperature, saturation, contrast, highlights and the rest) has its own add-on, **Image Grading**, below. Filters is just the looks.

**Filaments.** **Use only my loaded filament colors** snaps every pixel of the result to the nearest filament you have selected. What you see is what the matcher gets.

**Compare** moves a Before | After divider (drag on the picture too). **Apply filter** writes the look into your picture as an ordinary edit at your working resolution, keeping any cut-out or shape crop, the preview and the Apply give the same picture.

Pick another look later and it is applied to the photo as it was *before* the first one, so looks never pile up. **Undo** (↶) steps back. **Remove filter** (or the switch) puts the photo back exactly, unless you have made other edits on top since, in which case MythaPrism asks you to use Undo so none of them are lost. If the print is matched it re-matches. Before a match the look is simply part of your edited photo. Flat, few-color looks (Solid Color Fill V2, Posterize Tone, Flat Toon Shaded, Monochrome) give the color matchers the calmest pictures. Compare the matched preview with and without. A test print is the judge. The shareable PDF and the swap guide note the look under *Edits applied*.

Filters runs on your device, offline, in a background worker. It took over from the old 23-style Filters page in build 558 and was called Filter Lab until build 561. **Plus** and **Pro** include every look, Free shows the switch with the upgrade message.

## Image Simplifierpage 97

![The Image Simplifier on the flowers: versions in 4 colors, one of them on the picture. Tool and App.](https://mythaprism.com/manual_assets/m6/b597_simplifier.jpg)
![The Image Simplifier on the flowers: versions in 4 colors, one of them on the picture. Tool and App.](https://mythaprism.com/manual_assets/m6/b597_simplifier_app.jpg)

*The Image Simplifier on the flowers: versions in 4 colors, one of them on the picture. Tool and App.*

For a printer with one nozzle and one AMS, fewer colors means fewer swaps and a faster, cleaner print. Open **Image Simplifier** in Add-ons, choose how many colors the picture should use with **−** and **+**, and MythaPrism shows 100 versions of your photo in that many colors. Every color is a filament in your library, with its maker's published color, so what you pick is what prints. Specialty filaments are never used, and black only ever prints as black.

**Pick the colors you want.** Tap filaments under **Use these colors** (for example Red and Black) and every version is rebuilt to hold them. **New set** makes 100 versions you have not seen yet, the color sets shown least so far first, with new tone curves and a new order. When every color is one you picked, the set is filled with new tone curves, shifts and detail so it still holds 100. Tap a version to see it on the picture, drag **Compare** (or the picture) to see it beside the original, and step through the versions with the arrows. **Apply to the photo** puts it on the photo, and the filaments it really uses become your selection, so the color match that follows prints with them. If a picture has fewer tones than the colors you asked for, a version can use fewer, and the page says so (for example 3 of 4). Undo (↶) brings the photo back. The Image Simplifier switch stays on after Apply: turn it off to bring the photo and your filaments back as they were.

**Tones.** **Solid** shows each color as one filament at full strength, like a poster. **Layered** adds the in-between shades that thin layers of the same filaments make when they are stacked dark to light, the way a color match prints them, so the sky and the shadows blend instead of stepping. These shades come from each filament's light depth, so the preview is an estimate, and one layer of black still hides everything under it. With Layered, Apply selects every filament up to the lightest one the picture uses, because a stack prints each one under it. **Mixed** is a cross between Solid and Layered, for the look of a poster. Each version picks at random which of its filaments are layered (at least two, so there are in-between shades) and which print solid on top. The picture is split into parts along its own shapes, and each part prints solid or in layered shades at random, so a solid yellow can sit in a black, gray and white picture even where the photo has no yellow. The small version, the big preview and the applied photo show the same parts, and the color match prints the same stack. **Dots** makes the in-between shades from tiny dots of the solid colors side by side, so every spot is still one filament, good for flat prints.

**Plans.** Free makes 2-color versions in black and white. Plus goes from 1 to 6 colors, Pro from 1 to 24.

After **Apply**, the Image Simplifier row shows **✎ Edit** (in the App, a round pencil). It opens the page again without undoing the simplified picture. Every add-on that is on has the same Edit.

**Image Cuts** is no longer an add-on. Its splitting, merging and saving now live in **⧉ Cut out pieces** in the Edit menu (Chapter 6).

## Image Gradingpage 98

![Image Grading on the flowers: the Golden hour look, the Compare divider at 55 %, the arrows to step through the looks an](https://mythaprism.com/manual_assets/m6/t_imagegrading.jpg)

*Image Grading on the flowers: the Golden hour look, the Compare divider at 55 %, the arrows to step through the looks and the workspace buttons on the picture.*

**Image Grading** grades the color and light of the photo itself. The Prism Modifiers stay the controls for the print, Image Grading is for the photo. It opens on the edit-tool layout: the picture with a Before | After divider (the **Compare** slider under it, or drag on the picture), a **Strength** slider beside Compare (100 % is the full grade, lower blends it back toward your photo, 0 % is the photo unchanged, and Apply keeps the strength you chose), and numbered sections on the right:

**1 · Quick looks.** 53 one-tap grades shown as thumbnails of your own picture, in seven groups you pick from the chips above them: Everyday (Natural, Warm, Cool, Punchy, Soft, Vivid, Bright and airy, Crisp, Muted, Clean portrait, Food pop), Film (Faded, Golden hour, Vintage, Instant film, Seventies, Cross process, Bleach bypass, Film fade, Toy camera, Old photo), Cinematic (Teal and orange, Big Screen, Cinematic, Day for night, Noir, Western, Neon night), HDR (natural, dramatic, gritty, soft, landscape), Black and white (plain, hard, soft, Sepia, Cyanotype, Silver), Seasons and places (Autumn, Spring, Winter, Tropical, Forest, Ocean, Sunset, Morning mist, Candlelight) and Creative (Dreamy glow, Pastel, Infrared, Blue duotone, Landscape pop). Every look is MythaPrism’s own recipe of the sliders below, named after the general style, so you can start from one and fine-tune.

**2 · White balance.** Temperature and Tint. **3 · Color.** Hue, Saturation and Vibrance (strengthens the quieter colors more than the strong ones). **4 · Light.** Exposure (in camera stops), Contrast, Highlights, Shadows, Whites, Blacks and Midtones. **5 · Detail and haze.** Clarity (local contrast in the mid-tones), Texture (fine detail, or smoother skin when lowered) and Dehaze. **6 · Color mixer.** Pick one of eight color bands (Red, Orange, Yellow, Green, Aqua, Blue, Purple, Magenta) and change only those colors: their hue, saturation and luminance. A dot marks a band you changed. **7 · Color grading.** A tint and an amount for the shadows, the midtones and the highlights, and a Balance between them. **8 · Effects.** Fade, Vignette and its size, Grain and its size, and Glow.

**9 · Your LUT.** **Load a .cube LUT** reads a standard .cube file (3D or 1D, up to 40 MB) and applies it after the sliders, with a **Strength** slider from 0 to 100 %. The file is read and applied on your device and is never uploaded. A file that cannot be read says why. **Remove LUT** takes it off. Use LUTs you have the right to use. A LUT is not kept in a saved preset, so load it again when you need it.

**On the picture.** The round arrows on both sides (or the left and right arrow keys) step through the looks of the group you picked. The buttons in the corner work like the workspace’s: **Undo** and **Redo** step back and forward through your grade changes on this page (Ctrl+Z and Ctrl+Shift+Z too, they never touch the picture underneath), **Zoom in**, **Zoom out** and **Fit** (drag to move the picture while zoomed, or use the mouse wheel), and the rainbow button bottom left is **Hold to see original**. Double-click any slider, its name or its number to put it back to its default (on a phone, tap the number twice). **⚄ Randomize** deals a random grade and **↺ Reset** clears them all.

**Apply grading** writes the grade into the picture as an ordinary edit (transparent areas stay transparent), then re-matches the print if there is one. Undo (↶) steps back, grades never stack. A second Apply grades the photo as it was before the first, and switching the add-on off (**Remove grading**) puts the photo back. If you change the working resolution later, the same grade is applied again to the new picture, so it stays on. Everything runs on your device. Plus and Pro.

![Image Grading on the phone: the picture with the arrows and the buttons, Compare, then the look groups and the numbered ](https://mythaprism.com/manual_assets/m6/a_imagegrading.jpg)

*Image Grading on the phone: the picture with the arrows and the buttons, Compare, then the look groups and the numbered sections as you scroll.*

## Muralpage 101

![The Mural page: finished size and unit, tile shape, tile size, and the labeled tiles over the picture.](https://mythaprism.com/manual_assets/m6/t_addon_mural.jpg)

*The Mural page: finished size and unit, tile shape, tile size, and the labeled tiles over the picture.*

**Mural** splits a print bigger than your bed into labeled tiles (A1, A2, B1 …) that you print one at a time and reassemble by label. Mural and **Multi crop** are never on at the same time, because a mural would make every crop as big as the mural. If one is on and you turn on the other, a message asks you to keep the one you have or switch.

| Control | What it does |
|---|---|
| **Finished width · height** | Type either. The other follows the picture. |
| **Unit** | **mm, cm, m, in** or **ft**, the readouts follow, with the millimeter figure alongside. |
| **Shape** | Grid, brick or hex tiles, or draw them yourself in **Manual**. |
| **Tile size** | **100 × 100**, **200 × 200**, **300 × 300** mm, or **% of bed**. The line names your printer and its bed. |
| **Auto-fit** | Cuts the mural into tiles of that size. |

Each tile exports as its own closed plate with every color part it contains, so the slicer's filament list for a tile matches the whole print. Pair Mural with the **4096 px** working resolution (Pro) for crisp house-scale tiles. The shareable PDF of a mural carries the tile map with labels, a table of every tile's size and position, and step-by-step assembly. Pro.

### Size it up

![Size it up: the print at its finished size beside a 6 ft person, on a meter grid.](https://mythaprism.com/manual_assets/m6/t_addon_sizeitup.jpg)

*Size it up: the print at its finished size beside a 6 ft person, on a meter grid.*

Not sure how big to go? **Size it up** on the Mural page swaps the tiles for a size workspace: your print, drawn at its finished size, stands beside a reference object at the same scale: a golf ball, a tennis ball, a soccer ball, a basketball, a credit card, a phone, a letter or A4 sheet, a laptop, a 5′9″ or 6 ft person, an interior door or an average car. Drag the blue corner of the print to resize it (the finished width updates as you drag), drag either item to rearrange them, scroll or pinch to zoom, **⤢ Fit** to refit, **⇄** to swap sides, and **Back to tiles** to return.

While Mural is on, the Size visualizer shows one tile on your bed at true scale, with the total size and tile count above it.

The tile grid shows on the **Synthesized result** only, never on Prime, Relief bands, Schedule or the 3D model. The **Mural grid** switch at the top left of the workspace hides the grid and shows it again.

## Reassign bandspage 103

![The Reassign bands window on the flowers: the Detail slider breaks the picture into sections (their edges pulse slowly).](https://mythaprism.com/manual_assets/m6/t_reassign.jpg)

*The Reassign bands window on the flowers: the Detail slider breaks the picture into sections (their edges pulse slowly). Every tone band has a color and one section is selected (rainbow). On the right, the same palette and tools as Spot Color, and the two ways to build.*

**Reassign bands** (Pro) is for coloring a picture yourself instead of letting a color matcher decide. Switch it on in Add-ons (no color match is needed first, it works straight from the photo) and the window opens on the **Bands** view: your picture in gray, cut into **sections** whose edges pulse slowly. Choose how it is cut: **Auto split** (at color boundaries), **Gap split** (gray tone levels, the default), **Obj split** (whole objects), **Tones** (bands of brightness) or **Relief split** (the areas of the print's own heights, once there is a color match). The slider sets how fine the cut is. **Prime · Bands · Hide** switches between the photo with your colors laid over it, the gray picture, and a black view where only your colors and the pulsing split lines show. Press and hold the small rainbow **Hold to see original** icon to see the untouched photo.

![Reassign bands with Relief split: the Bands view (left) and the Hide view, where only the split lines pulse (right).](https://mythaprism.com/manual_assets/m6/b590_reassign_relief.jpg)
![Reassign bands with Relief split: the Bands view (left) and the Hide view, where only the split lines pulse (right).](https://mythaprism.com/manual_assets/m6/b590_reassign_hide.jpg)

*Reassign bands with Relief split: the Bands view (left) and the Hide view, where only the split lines pulse (right).*

Click a section to select it (click it again to let it go, **Whole band** selects every section of that brightness at once). For a shape the sections don't follow, trace it with **Points**, **Freehand** or **Snapper**, or paint it with the **Brush** (**Erase** takes pixels back out, and **Size** sets the tip, so zooming in gives a finer one). Then pick a color. The same choices the Spot Color window offers: every solid filament, the colors already in your print and the two-filament composite mixes, or **Choose color from image** to eyedrop one. Picking a color with a selection colors it at once, **Color the selection** uses the current color again. **Uncolor selection** and **Clear all colors** undo coloring, **Undo selection** steps the selection back.

![The built print in the Synthesized result. The match button now reads Color match · Manual.](https://mythaprism.com/manual_assets/m6/t_reassign_result.jpg)

*The built print in the Synthesized result. The match button now reads Color match · Manual.*

**Build print** works out the layers that make your colors real. **One stack · any printer** plans a single stack of layers for the whole plate (the same planner as V1.3, run on your colored picture). It prints on any printer with filament swaps or an AMS. **Exact zones · AMS** gives every colored area its own stack (the V1.2 zones), so each color lands exactly. It needs a multi-material system. **The parts you did not color** decides the rest of the picture. **Auto** (the default) runs the color matcher you used last (or your plan’s default) on the picture and keeps its result wherever you did not color, so you can color the background and let the matcher do the subject. **Pick a matcher** lets you choose that matcher from a list. **My colors** gives each uncolored section the closest of the colors you used. The filaments your colors and the matcher need are added to your selection. Selection, Build the layers as and The parts you did not color fold open and shut like the sections of the other tools, and Build print stays in view. The color matcher reads **Manual**, you chose the colors, and the Synthesized result, 3D preview, Prism control, export and shareable PDF all follow your plan. The Prime view still shows your photo.

To change something, press **✎ Edit**: the window reopens with your colors. Picking any color matcher leaves Manual. Switching Reassign bands off goes back to the engine you had before.

![Reassign bands on the phone: the same window, full screen, with the palette below the picture.](https://mythaprism.com/manual_assets/m6/a_reassign.jpg)

*Reassign bands on the phone: the same window, full screen, with the palette below the picture.*

On the phone, Reassign bands sits in **Edit → Add-ons**, after Mural. Tap a section to select it, tap a color to fill it, and press **Build print**. The match pill then reads **Manual**.

09

# Filament calibration

The library values get you a great first print. Your own spools are the ground truth, and one printed plate and a phone photo are enough for MythaPrism to measure them.

## Why calibratepage 107

Two spools sold as "yellow" can let through very different amounts of light, and the difference shows most in thin layers. Exactly the layers skin tones and mid-tones are built from. A calibration plate prints every filament you select at known thicknesses over a white slab and over a black slab. You photograph it, the Tool reads the photo in your browser, and from then on every engine composites with what your spools actually do.

![The calibration block at the bottom of the Filament library, and the App's collapsed Filament calibration section.](https://mythaprism.com/manual_assets/m6/t_library_cal.jpg)
![The calibration block at the bottom of the Filament library, and the App's collapsed Filament calibration section.](https://mythaprism.com/manual_assets/m6/a_sheet_colors_cal.jpg)

*The calibration block at the bottom of the Filament library, and the App's collapsed Filament calibration section.*

## Step by steppage 107

1. **Select the filaments** you want measured in the library. Every enabled filament goes on the plate.
2. **Export the plate:** **⌗ Calibration plate (.3mf)** in the library (or *Filament calibration plate* in the Export menu). It prints squares of each filament at 1, 2, 3, 4, 5, 6, 8, 10, 12 and 16 layers plus a 20-layer reference, over a white slab and over a black slab, with a color-over-color check row and an orientation mark. Print it at 0.08 mm and 100 % infill, exactly as exported.
3. **Photograph it** straight down in even daylight, HDR off, a touch under-exposed (about −0.7 EV) so reds and yellows don't clip. Several photos are better than one.
4. **📷 Read calibration photo** and pick the photos (the phone's album picker allows several at once). The reader finds the plate, straightens it, measures every square and lists each filament's opacity over white and over black, plus the color-over-color check. It skips any photo it can't read and says why, and warns when a color channel hit the camera's ceiling. On a different device from the one that exported the plate, add its `_layout.json` first with **📄 Add plate layout (.json)**.
5. **Calibration V4** is on as soon as a plate has been read (one switch, **Calibration V4: real colors and layer limits**, in the same panel). Your measurements are stored on this device, one set per layer height.

## Calibration V4: your filaments' real colorspage 108

What the plate shows: over a **white** backing one layer of a color is already most of the way to that color, while over a **black** backing colors build up slowly. Calibration V4 plans with what your plate measured. Each filament uses the **full-strength color** your plate photographed, and a **light depth** fitted so that it reaches that color in the number of layers your plate showed. That number is the **pair** on the library chips: how many layers the filament needs to show its full color over white, then over black.

![The calibration results in the Filament library, read from a developer plate set, with the Calibration V4 switch on.](https://mythaprism.com/manual_assets/m6/b608_cal_v4.jpg)

*The calibration results in the Filament library, read from a developer plate set, with the Calibration V4 switch on.*

**Layer limits.** No band in the print ever gets more layers than its filament needs to be pure over what is under it, and no calibration can push a filament past what its light depth allows. Black is always 1 and only ever goes under other colors to darken them.

**The results table.** One row per filament: the measured and the library color, **Pure after** (the pair, over white and over black), **1 layer on white** and **1 layer on black** (how much one layer covers), **fit ΔE**, the **LD** and **Hides at** (the thickness where white and black backings look the same), with the squares from 1 to 20 layers over white, then over black. ⚠ marks a filament whose measured color is far from the library color.

**Where it applies.** Relief Prism and the stacked modes. Prints with a flat painted face (Slim, and the flat sides of Dual, Hybrid and Focus) keep the maker’s colors, because measured colors matched worse there.

**Developer builds only.** The older calibration tools, Calibration V3 and its print estimate, the measured profiles, Calibration V2, Measured stacks only, the Pairs, Spectrum and Mixes plates and the trained color model, are in developer builds only and are not part of this release.

Plans

Calibration is included with Plus and Pro. The companion *Filament Calibration Guide* covers the details: lighting set-ups, reading the results table, and one calibration set per layer height.

10

# Export, share and print

One click gives you a complete print job and a print guide anyone can follow. This chapter covers every file MythaPrism writes, how to slice it, and how to get a print made (by a friend, a makerspace or a print farm) when you don't own the printer.

## The Export menupage 111

![The Export menu.](https://mythaprism.com/manual_assets/m6/t_exportdrop.jpg)

*The Export menu.*

| Option | What you get | Plan |
|---|---|---|
| **.3mf file** | The complete job for Bambu Studio and OrcaSlicer: geometry, printer and process presets, filament colors, and the swap schedule (relief) or per-part colors (flat and zoned). | All |
| **.3mf + shareable PDF** | The `.3mf` plus the Print Guide & Share Sheet. The recommended export. | All |
| **Filament calibration plate** | The calibration plates for the selected filaments (Chapter 9). | Plus · Pro |
| **V8 calibration tile** | The C/M/Y/K/White swatch tile for the V8 engines. | Pro |
| **STL + swaps (.txt)** | The mesh as STL plus a text guide listing every filament change, for any other slicer. You add the pauses. | All |
| **Blender file (.glb, colors included)** | The finished print as a 3D object with its colors: one object and one material per filament, real size, upright (Chapter 12). | Pro |
| **OBJ + MTL for CAD (.zip)** | The same colored objects as `.obj` + `.mtl`, in millimeters, Z up. | Pro |
| **Shareable PDF (.pdf)** | The Print Guide & Share Sheet on its own. | All (Free is watermarked) |
| **Package: everything (.zip)** | The `.3mf`, the guide, the preview, the settings, and on Pro the `.glb` plus a `blender/README.txt` saying where to download the Blender add-on (your account on mythaprism.com). | Plus · Pro |

**Save ▾** keeps your work rather than printing it: **Save edited prime image (.png)** (your picture with the edits baked in), **Save synthesized image (.png)** (the preview, for listings and mock-ups), **Shareable PDF**, and **Save project (.mpsm), full save state**: a `.mpsm` (MythaPrism project) file holding the pictures (including the untouched original, so *Revert all edits* still works), the color match itself (every engine's stack, zones or per-pixel plan, both sides in the two-picture modes), every edit, spot color and text, the mode, the add-ons (Puzzle cut, Mural), the engine settings and every control. Open it with **Save ▾ → Open project (.mpsm)** or drop it in like a picture: the workspace comes back exactly as it was, with no re-match. The file is kept bare bones. Only what the current print needs, never program code, and it is compressed and encoded, so it opens only in MythaPrism (a file that was changed or damaged is refused rather than opened wrong). Expect a few MB for a phone-size picture, more at Pro working resolutions. Older `.mythaprism`, `.sculptraprism` and `.sculptra` projects still open (the saved engine re-matches the picture, since those files did not store the match). A project made with an engine or mode your plan does not include opens with its picture and settings and is re-matched with your plan's engine.

### What the .3mf carriespage 112

Real preset names for your printer and layer height (for example *0.08 mm High Quality @BBL H2C*) so nothing resets when the slicer opens it, a process tuned for translucent color, 100 % infill, monotonic surfaces and slow speeds that keep thin layers even on relief surfaces (the flat modes run stock speeds), the print centered in your printer's printable area, a free spot kept for a prime tower. The tower itself is off, because most prints come out clean without it (turn it on in the slicer if you see colors mixing), and several plates in one file for Multi crop and Mural.

## The shareable PDF

![The Print Guide & Share Sheet for the Sun print (V2 1.0): the cover with both pictures and the settings, the filament st](https://mythaprism.com/manual_assets/m6/pdf_relief_1.jpg)
![The Print Guide & Share Sheet for the Sun print (V2 1.0): the cover with both pictures and the settings, the filament st](https://mythaprism.com/manual_assets/m6/pdf_relief_2.jpg)
![The Print Guide & Share Sheet for the Sun print (V2 1.0): the cover with both pictures and the settings, the filament st](https://mythaprism.com/manual_assets/m6/pdf_relief_3.jpg)

*The Print Guide & Share Sheet for the Sun print (V2 1.0): the cover with both pictures and the settings, the filament stack and schedule, and the slicer walkthrough.*

The shareable PDF is one page set per physical part: your picture and the synthesized result, every setting needed to recreate the print (mode, engine, dither, printer, nozzle, layer heights, calibration), the edits applied, the filament stack (or the swatch grid of a zoned print), the swap schedule with layer numbers that match your slicer's layer slider, purge guidance, a slicer walkthrough, a troubleshooting table and a printer-requirement note: *any printer*, *AMS recommended* or *AMS required*. The **Size** line reports the real height of the exported geometry. When the back-plate watermark is on, the guide says the first layer prints in two filaments and marks the job as needing an AMS or multi-material setup. A Global height limit is listed with the settings. With an add-on on, an **Add-ons in this print** section follows: the puzzle's piece map, the multi-crop plates or the mural's tile map and assembly steps.

![The Add-ons section of a puzzle print: the labelled piece map, the piece table, and how to print and solve it.](https://mythaprism.com/manual_assets/m6/pdf_puzzle_add.jpg)

*The Add-ons section of a puzzle print: the labelled piece map, the piece table, and how to print and solve it.*

## No printer? Share the projectpage 113

You don't need to own a color 3D printer to make something with MythaPrism. The `.3mf` and the shareable PDF together are a complete, self-explaining print job. Everything a person with the right printer needs, and nothing they have to guess.

A friend

Send the two files to anyone with a multi-color printer. The .3mf opens with your colors assigned. The PDF shows what it should look like and which spools to load.

A makerspace

Libraries, schools and makerspaces often have multi-material printers. Bring the files on a phone or a USB stick. The PDF is the job ticket.

A print service

Online 3D-print services and print farms take a .3mf directly. The PDF is your spec sheet: filaments, layer height, infill, and a picture of the result.

**Send it from the App.** Every export on the phone ends in the **Download or Share** prompt. **Share** opens the system share sheet (AirDrop, Messages, e-mail, Drive, Files, or the app of a print service) so a photo you took a minute ago can be on its way to a printer before you put the phone down.

![The App's Export sheet and the Download-or-Share prompt.](https://mythaprism.com/manual_assets/m6/a_sheet_export_files.jpg)
![The App's Export sheet and the Download-or-Share prompt.](https://mythaprism.com/manual_assets/m6/a_share_prompt.jpg)

*The App's Export sheet and the Download-or-Share prompt.*

**Order in bulk.** A print farm prints the same job many times over. Because the `.3mf` already carries the printer, the process, the layer height and every filament change, each copy comes out the same. The PDF tells the farm which filaments to load and what the finished piece looks like, so there is nothing to interpret. Keychains for a whole team, coasters for an event, badges for a club, ornaments for a family: one match, one file, as many copies as you order. Multi crop and Mural files arrive with every plate already laid out.

Before you order many copies

Order one first and compare it with the PDF's synthesized picture. Ask the service to use the filaments the PDF lists (or tell you what they substituted), and to print at the layer height and 100 % infill in the file. If you plan to *sell* what you make, you need the commercial license (Creator or Studio) and the rights to the picture. See Chapter 14.

## Slicing, step by steppage 114

1. **Open the `.3mf` fresh**, File → Open in Bambu Studio or OrcaSlicer, and accept the bundled presets when asked.
2. **Map the filament slots** to the spools in your AMS, the colors arrive preset. The **Filament change schedule** lists them in order.
3. **Slice and compare** the filament-change list with MythaPrism's **Layer schedule** view and the PDF.
4. **Print** without changing infill or surface speeds on relief prints.

**Single-nozzle printers.** Print a Relief with the swap schedule (pause at each listed layer, change the spool, purge), every one-stack engine (V1.3 to V1.8, V2 1.0) prints one filament per layer. The flat and zoned prints need a multi-material setup. For other slicers, use **STL + swaps (.txt)** and add a pause at each layer the text lists.

11

# The MythaPrism app

The whole engine in your pocket, built around the camera. See something worth printing, shoot it, edit it, color-match it and send a print-ready file to your printer, all without leaving the app, in seconds.

## Built around the camerapage 117

Most 3D-print tools start at a computer with a file you already have. The MythaPrism app starts where pictures actually happen. **Take a photo** sits in the middle of the empty workspace. One tap opens your phone's own camera, and the shot lands in the workspace ready to match: full resolution, no cropping on a computer, no transferring files.

![The launch page with the consent box ticked, the empty workspace with Take a photo, and the Photo sheet.](https://mythaprism.com/manual_assets/m6/a_launch_consented.jpg)
![The launch page with the consent box ticked, the empty workspace with Take a photo, and the Photo sheet.](https://mythaprism.com/manual_assets/m6/a_empty_camera.jpg)
![The launch page with the consent box ticked, the empty workspace with Take a photo, and the Photo sheet.](https://mythaprism.com/manual_assets/m6/a_sheet_photo.jpg)

*The launch page with the consent box ticked, the empty workspace with Take a photo, and the Photo sheet.*

What makes the phone special:

- **Camera to print file in seconds.** The match, the preview and the export all happen on the phone. A photo you take can be a `.3mf` before you've walked away from the subject.
- **Your phone's own camera.** The app opens the real camera app (every lens, zoom and setting you're used to) rather than a cut-down in-app viewfinder. iPhone photos in HEIC format open directly, and so do the Android camera's.
- **Private by default.** Your photos stay on the phone for the free edition and every on-device engine (Chapter 14).
- **Phones and tablets.** The app works on iPhone, iPad and Android phones and tablets. On a tablet the sheets stop at a comfortable reading width and the app turns with the screen. On a phone it stays upright. In a phone's web browser, the web tool itself opens: the same tool as on a computer, laid out in one column that fits the screen (picture first, then every card under it).
- **Edit with your fingers.** Pinch to zoom the picture, swipe between views, and in the edit tools drag with one finger and pinch-and-twist with two to resize and rotate whatever you place.
- **Share straight to a printer.** Every export ends in **Download or Share**: AirDrop or Files to your computer, e-mail, Messages, a print service's app (Chapter 10).
- **The same projects as the desktop.** Save a `.mpsm` project on the phone (Export sheet → Save project) and open it in the Tool, or the other way round. On the phone, **Open a saved project (.mpsm)** under *Tap to drop in a photo* in the Photo sheet opens the file picker (Files on Android and iPhone).

Taking a photo worth printing

Shoot in even, soft light. Open shade or an overcast day beats harsh sun, which bakes black shadows into the print. Fill the frame with the subject. A plain background makes Cut out pieces and Focus Prism effortless. Hold the phone square to flat artwork to keep it rectangular. And shoot a little wider than you need: crop presets (bookmark, card, square) can then frame it exactly.

## The launch pagepage 118

Tick **I have read and agree to the Terms of Service, the EULA and the Privacy Policy**. Every button stays dimmed until you do, and a newer Terms version asks again. Then **Launch the free tool** (no sign-in needed to use it, and sign in with a free account to download your print), or sign in to a paid plan with **Continue with Google**, **Continue with Apple** or your e-mail. With e-mail you can use your password, or a short page opens to send you an 8-digit code that you type or paste in the app (the Paste button reads only the digits). Before the code is sent, the app shows your address in large letters and points out common typos such as .con for .com. The app keeps you signed in in the phone's secure storage. One account works everywhere: a plan bought on the website unlocks the app, and a plan bought in the app unlocks the website. **Buying in the app:** Plus and Pro (monthly or yearly) and the pack of 10 black-and-white downloads are App Store / Google Play purchases, billed by Apple or Google at the price the store shows, manage or cancel them in the store's subscription settings (**Manage subscription** in the account menu takes you there). **Restore purchases** finds them again on a new phone. The Creator / Studio bundles and the Plug-in and Showroom are sold on the website only. **Delete my account** is in the account menu too (cancel a store subscription first, deleting the account does not stop the store billing).

## The workspacepage 119

![The stage after a V25 match (Prime, Synthesized result, Relief bands and Schedule) and the 3D model.](https://mythaprism.com/manual_assets/m6/a_view_prime.jpg)
![The stage after a V25 match (Prime, Synthesized result, Relief bands and Schedule) and the 3D model.](https://mythaprism.com/manual_assets/m6/a_result_v25.jpg)
![The stage after a V25 match (Prime, Synthesized result, Relief bands and Schedule) and the 3D model.](https://mythaprism.com/manual_assets/m6/a_view_height.jpg)
![The stage after a V25 match (Prime, Synthesized result, Relief bands and Schedule) and the 3D model.](https://mythaprism.com/manual_assets/m6/a_view_schedule.jpg)
![The stage after a V25 match (Prime, Synthesized result, Relief bands and Schedule) and the 3D model.](https://mythaprism.com/manual_assets/m6/a_3d.jpg)

*The stage after a V25 match (Prime, Synthesized result, Relief bands and Schedule) and the 3D model.*

The top bar carries the logo, the name of the view you are on (Prime · Synthesized result · Relief bands · Schedule) with four dots beneath it, the plan badge and the person icon.

| Gesture or control | What it does |
|---|---|
| **Swipe left / right** | Moves between the four views. |
| **Pinch** | Zooms the picture: zoomed in, it runs edge to edge behind the frosted bars. One finger pans, dragging hard into an edge turns the page. |
| **▶ and the slider** (Schedule) | Builds the print up layer by layer. With the 3D model on, the model builds up with it, cut at each layer's true height in the colors that layer shows. |
| **↶ / ↷** | Undo and redo: everything, 10 steps (25 on Pro). |
| **2D / 3D** | The 3D model: one finger rotates, two fingers move, pinch zooms, **Reset**, the **Tilt** slider and the **1x** speed pill work as on the desktop. |
| **Engine pill** | Names the engine in use. |
| **Back button** | Closes the top layer (a tool page, the plans, the account panel, a sheet) one at a time. It never quits the app while something is open. |

## The six sheetspage 119

The bottom bar holds six sheets: **Photo · Colors · Modes · Edit · Tune · Export**. Tap one and it slides up over the stage. Tap outside it or swipe it down to close.

### Photopage 119

**Take a photo** (camera) and **Tap to drop in a photo** (your library). **Working resolution**: the pixel budget the whole app runs at (Plus goes to 2160 px, Pro to 4096 px). **Quick edits**: shortcuts to Crop, Silhouette, Spot color, Hole punch and Text.

### Colors

![The Colors sheet: your filaments, the count and Auto, the engine rail and Color match, and the Filament calibration sect](https://mythaprism.com/manual_assets/m6/a_sheet_colors.jpg)
![The Colors sheet: your filaments, the count and Auto, the engine rail and Color match, and the Filament calibration sect](https://mythaprism.com/manual_assets/m6/a_sheet_colors_cal.jpg)

*The Colors sheet: your filaments, the count and Auto, the engine rail and Color match, and the Filament calibration section opened.*

**Your filaments** are the enabled chips, **+** opens the library, the red ✕ removes a chip. **Colors in the print** is the count slider with **Auto**. **Filament calibration** is a collapsed section holding the plates, the reader and the switches (Chapter 9). **Match engine** is a scrolling rail of chips grouped by family. Tap one, then **Color match**. After a zoned match the sheet shows **Colors in this print**.

### Modes

![The Modes sheet, a mode card, and the LithoPrism card with its six engines.](https://mythaprism.com/manual_assets/m6/a_sheet_modes.jpg)
![The Modes sheet, a mode card, and the LithoPrism card with its six engines.](https://mythaprism.com/manual_assets/m6/a_mode_card.jpg)
![The Modes sheet, a mode card, and the LithoPrism card with its six engines.](https://mythaprism.com/manual_assets/m6/a_litho_card.jpg)

*The Modes sheet, a mode card, and the LithoPrism card with its six engines.*

Seven rows (2D image editing (on top), Relief, Slim, Dual, Hybrid, Focus and LithoPrism) each with a one-line description. Tap a row for its card and **Launch**. Options for the active mode appear under the list. Once a launched mode has finished loading, after the match, and for the two-picture modes after the second picture is placed. The sheet slides down by itself so the result is in view.

### Edit

![The Edit sheet: the edit tools, then the Add-ons and Processing further down.](https://mythaprism.com/manual_assets/m6/a_sheet_edit.jpg)
![The Edit sheet: the edit tools, then the Add-ons and Processing further down.](https://mythaprism.com/manual_assets/m6/a_sheet_edit_addons.jpg)

*The Edit sheet: the edit tools, then the Add-ons and Processing further down.*

**Edit tools** (Chapter 6) each open full-screen. **Add-ons** (Puzzle cut, Multi crop, Filters, Image Simplifier, Image Grading, Mural and Reassign bands) are switches that open their pages (Chapter 8). **Processing** holds Dither Off to 4.5, Relief test, Smoother surface, Degradient and the CMYK switches (Chapter 5).

### Tune

![The Tune sheet, a live slider over the picture, locks and the Randomize panel, and the Engine settings.](https://mythaprism.com/manual_assets/m6/a_sheet_tune.jpg)
![The Tune sheet, a live slider over the picture, locks and the Randomize panel, and the Engine settings.](https://mythaprism.com/manual_assets/m6/a_tune_live.jpg)
![The Tune sheet, a live slider over the picture, locks and the Randomize panel, and the Engine settings.](https://mythaprism.com/manual_assets/m6/a_sheet_tune_locks.jpg)
![The Tune sheet, a live slider over the picture, locks and the Randomize panel, and the Engine settings.](https://mythaprism.com/manual_assets/m6/a_mod_rand_panel.jpg)
![The Tune sheet, a live slider over the picture, locks and the Randomize panel, and the Engine settings.](https://mythaprism.com/manual_assets/m6/a_sheet_tune_neural.jpg)

*The Tune sheet, a live slider over the picture, locks and the Randomize panel, and the Engine settings.*

Every Prism Modifier is a row showing its current value. Tap a row and a live slider drops onto the picture so you see the change as you drag. **Confirm** keeps it, **Cancel** puts it back, and **Reset** puts that one modifier back to 0. The 🔒 on a row locks that slider. **Randomize modifiers** opens a panel under the workspace with **Randomize**, **Reset** and **Done**, randomize never touches Hue or a locked slider. After a V25-family match the **Engine settings** rows follow the same pattern.

### Export

![The Export sheet: Print setup, stats, and the Save and Export buttons.](https://mythaprism.com/manual_assets/m6/a_sheet_export.jpg)
![The Export sheet: Print setup, stats, and the Save and Export buttons.](https://mythaprism.com/manual_assets/m6/a_sheet_export_setup2.jpg)
![The Export sheet: Print setup, stats, and the Save and Export buttons.](https://mythaprism.com/manual_assets/m6/a_sheet_export_bottom.jpg)

*The Export sheet: Print setup, stats, and the Save and Export buttons.*

**Print setup**: printer, size with the size visualizer, nozzle, layer height, first layer height, base color, base thickness and watermark. **Print stats**: height, layers, swaps and match ΔE. **Save**: project, synthesized image, edited picture. **Export**: every file from Chapter 10. Each export ends in the **Download or Share** prompt, both keep a copy on the phone.

The **Edit** and **Export** sheets lay their buttons out in two even columns, and the filament library lists your filaments the same way. Signed out, the account panel offers **Sign in** and **Back to the sign-in screen** (your picture and work stay). Signing in or out, and Refresh workspace, restart the app cleanly, and Refresh reopens the picture you dropped in. The Android Back button closes whatever is open, one layer at a time.

![The Edit and Export sheets on the phone.](https://mythaprism.com/manual_assets/m6/b590_app_edit.jpg)
![The Edit and Export sheets on the phone.](https://mythaprism.com/manual_assets/m6/b590_app_export.jpg)

*The Edit and Export sheets on the phone.*

**Sign-in and security** (in the account panel) holds two optional protections. **Two-step sign-in** adds a 6-digit code from an authenticator app to your usual sign-in, so someone who gets into your e-mail still cannot open your account. Turn it on there or in the Two-step sign-in tab of your account page at mythaprism.com: add MythaPrism to your authenticator app (tap Open in my authenticator app on the phone, scan the code from another device, or type the key), then type the code it shows. Add a backup authenticator if you can. From then on, every sign-in asks for the code after the e-mail code (or Apple / Google). Lost every authenticator? Write to support@mythaprism.com from your account e-mail. **App lock** (iPhone, iPad and Android) asks for Face ID, Touch ID, your face or fingerprint, or your screen lock when the app opens and when you come back after five minutes away. Your face or fingerprint never leaves the phone. Purchases still use the store's own confirmation.

## Account and plans

![The account panel, and Plans & licenses.](https://mythaprism.com/manual_assets/m6/a_account.jpg)
![The account panel, and Plans & licenses.](https://mythaprism.com/manual_assets/m6/a_plans.jpg)

*The account panel, and Plans & licenses.*

The person icon opens the same account panel as the Tool, plus **Restore purchases**. **Settings** switches the app between its dark look and a **light mode**, soft light grey surfaces with dark text. Your pictures, the filament swatches and the preview colors never change.

**Paid plans in the app.** The app you install from the App Store or Google Play holds the free tool. When you have Plus or Pro, bought in the app or on mythaprism.com, sign in (with your two-step code if it is on) and the app downloads your plan's tool once, a few megabytes, checks it and restarts into it. From then on it opens straight from the phone. The app checks your plan whenever it connects, at least once every 31 days, so a paid tool needs a connection now and then. Moving to a lower plan swaps in that plan's tool, an ended plan goes back to the free tool, and after an app update the tool is downloaded again the next time the app connects. Your pictures never leave the phone.

![Light mode: the Colors and Export sheets.](https://mythaprism.com/manual_assets/m6/a_light_colors.jpg)
![Light mode: the Colors and Export sheets.](https://mythaprism.com/manual_assets/m6/a_light_export.jpg)

*Light mode: the Colors and Export sheets.*

## The free edition on the phonepage 126

![The Free edition: locked controls carry a plan badge and explain themselves when tapped.](https://mythaprism.com/manual_assets/m6/a_free_colors.jpg)
![The Free edition: locked controls carry a plan badge and explain themselves when tapped.](https://mythaprism.com/manual_assets/m6/a_free_modes.jpg)

*The Free edition: locked controls carry a plan badge and explain themselves when tapped.*

Free is monochrome: black and white filaments, two colors, the B&W engine (smooth or halftones), 0.08 mm layers and Relief Prism. Everything else shows a **Plus** or **Pro** badge. Tap it to see what it does and which plan unlocks it. The camera, Crop, Puzzle cut and the `.3mf` and PDF exports all work on Free. You can open and use all of it without signing in, downloading a print file on Free asks you to sign in to a free account (10 print downloads a month, and a pack of 10 more is $1.99). Signed in, a small round counter next to **Hold to see original** shows how many print downloads you have left (this month's free ones plus any from packs). Hover or tap it to see when the free ones reset and to buy 10 more. Your photo still stays on your phone. Tap a 🔒 message's **See plans ›** for the upgrade card (a black card with your picture in slanted panes that swap between black and white and color), and after a black-and-white match tap **See it in color** for a rough color preview of your photo.

**Previews of what a plan adds.** On Free and Plus, tapping something your plan does not include also plays a short clip above the message: real MythaPrism output of that feature (a Hybrid print turning in 3D, the dithers on one photo, a Mural drawn to scale beside a person, Spot color fixing a spot up close). Each one plays once per feature while the app is open, closes after a few seconds or when you tap anywhere else, and the X closes it at once. The clips are part of the app, so nothing is downloaded and nothing about you is sent. Pro never shows them.

**Tutorials.** The first time the app opens with no picture, it offers a short walkthrough. You can start it again at any time from the account menu, **Tutorials**: **Make your first print** walks you through a whole print on your plan with a painting of flowers on black that comes with the app: crop it, raise the contrast a little, add or take out filaments in the library, pick V1 in the Colors sheet (B&W smooth on Free), then V1.6 (B&W crisp on Free) in the matcher bubble on the workspace, so you see that one matcher can suit a picture better than another, ease the contrast back, choose a size in the Size visualizer, then export the .3mf and the shareable PDF. It also points to Spot color and Reassign bands for choosing colors yourself. **Tour of the app** points out every part of the app: the workspace buttons, presets and Save preset, Prism control, the matcher bubble, every print mode, every edit tool and add-on, processing, every Tune row, every Export setting and the account menu, and names the plan a part needs. A ring shows where to tap, a bubble says what happens, and you can skip any step. **Family portrait** takes your own photo of a person, a family or a pet through the Family portrait preset: three filaments (Black, Jade White and Blue Grey) and Dither 3.0 blend into soft skin, hair and shadows, then 3D on Pro and the export (Plus and Pro, on Free it shows where the preset is). Both end on **More from MythaPrism**: the Plug-in and Showroom, MythaBraille, what is on the way, and where to follow us.

**Slicing a detailed print takes time.** The first time you export a print file (3MF, STL or the export package), a note says that a busy picture, a dithered or CMYK print or a big print can have millions of triangles, so your slicer can take many minutes to open and slice it. That is not a bug, it is how slicers handle very complex shapes today. A lower Working resolution, fewer colors, no dither, a smaller size or Small file in Dot detail make a lighter file. Tap **I understand** once and it does not ask again on that device.

**Your printer setup and the cheat sheets.** The first time the app or the tool opens, it asks what kind of printer you have: one nozzle where you change filament by hand, one nozzle with an AMS or another filament changer, two nozzles (H2D, X2D), a tool changer with up to 6 toolheads (Snapmaker U1, FlashForge Creator 5, Prusa XL), or 7 or more nozzles (Bambu Lab H2C or H3C, or a Prusa CORE One with the 8-tool INDX). It then shows a cheat sheet of what to stick to and what to avoid on that setup. For example, by hand: the matchers under Each color used once and few colors, because every color is a stop at the printer. With a tool changer: the Zoned and CMYK matchers, with as many colors as toolheads. Every plan can read every cheat sheet, and each tip names the plan it needs. Find them again in the account menu, **Tutorials**: Your printer setup, Cheat sheets and More from MythaPrism.

12

# MythaPrism Plug-in and Showroom

A plug-in made for Blender and compatible with Blender 4.2 and newer (it was called MythaPrism for Blender until build 561). Take a finished print, any mode, into Blender with its real colors, layer by layer. Check it against your printer, add geometry of your own, send it back to the slicer with every color still assigned, or stand it in a showroom and render product shots that look like photographs.

## What it doespage 129

MythaPrism does the part no 3D app does: it turns a flat picture into a filament-accurate stack of colored layers. **Export → Blender file (.glb, colors included)** hands that result to Blender as real geometry: one object per filament, real size, colors on. The **MythaPrism Plug-in and Showroom** add-on turns the file into a workspace:

- **One-click import, every mode** (Relief, Slim face-down or face-up, Dual and Hybrid (both faces), LithoPrism and CMYK) at true millimeter size, with the colors MythaPrism shows on the faces you look at (a face printed face-down carries its own picture on the underside) and each filament's color on the walls, one collection per filament, transforms locked so nothing drifts.
- **The filament stack, layer by layer**, every filament with its real layer count. Open one and pick any of its layers to see the print cut at that layer.
- **Printer constraints**. Your printer drawn around the print at true scale, with a Fits / Too big check.
- **1.6.0**: the sidebar is numbered sections that fold (1 Colors and light, 2 Filaments and layers, 3 Zones, 4 Printer, 5 Showroom, 6 Backlight, 7 Turntable video, 8 Export and settings) and **Help**. **Real light** in section 1 makes every filament real plastic that light crosses by MythaPrism’s light depth: one 0.08 mm layer of black stops the light, one layer of white still glows, so a one-layer white barrier in a Dual print lets the back picture bleed through under the backlight. It renders in Cycles. **Zones** lists each zone of a zoned print with its own stack, and shows a zone alone. The **Stage logo** switch takes the MythaPrism logo off the stage for clean product shots.
- **Showroom**: a black showroom with rainbow accents, a turntable, seven ready-made camera angles, switches for Stand at 90°, Side mirrors and the Stage logo, a Backlight with its own section (the light box and its light switch separately), Real light (light crosses every layer by its light depth), a Zones section for the zoned engines and a Help section for every button, and a one-click turntable video, rendered in Cycles.
- **Export for the slicer**. Your edited model back out as `.obj` + `.mtl` with one group per filament.

![Rendered in the Showroom: a Slim print turned to show its face-down face, a LithoPrism Moon with the Backlight on, and a](https://mythaprism.com/manual_assets/m6/bl5_slim_down_0.jpg)
![Rendered in the Showroom: a Slim print turned to show its face-down face, a LithoPrism Moon with the Backlight on, and a](https://mythaprism.com/manual_assets/m6/bl5_litho_1_backlight.jpg)
![Rendered in the Showroom: a Slim print turned to show its face-down face, a LithoPrism Moon with the Backlight on, and a](https://mythaprism.com/manual_assets/m6/bl5_dual_0_mirrors.jpg)

*Rendered in the Showroom: a Slim print turned to show its face-down face, a LithoPrism Moon with the Backlight on, and a Dual print between the Side mirrors.*

**Getting it.** The add-on is included with the **Studio Bundle**, and anyone else (Free, Plus, Pro or the Creator Bundle) can buy it on its own for a one-time $14.99. Sign in at **mythaprism.com → Account → Download MythaPrism Plug-in and Showroom** (the Tool's and App's **account panel → MythaPrism Plug-in and Showroom → Download from my account** opens that page). One download is a zip with the add-on and the Studio scene. You can download each add-on version up to **3 times** (enough to reinstall on a new computer), and every new version gives 3 more. Lost all three? E-mail support@mythaprism.com. It needs Blender 4.2 or newer and a MythaPrism `.glb`: export your own with Pro or the Studio Bundle, on Free, Plus or the Creator Bundle it opens MythaPrism .glb files other people share with you. The add-on's code is open source under the GPL. The MythaPrism name, logo and the Studio scene are not.

## Install and importpage 130

1. In Blender: **Edit → Preferences → Get Extensions → ▾ → Install from Disk**, and pick the add-on zip. (To update later, remove the old version first, then install the new one.)
2. In a new scene press **N** in the 3D viewport and open the **MythaPrism** tab.
3. **Import MythaPrism print (.glb)** and pick your file. (It is also under **File → Import → MythaPrism print (.glb)**.)

![A print imported with the add-on: the flowers at 120 mm, the MythaPrism panel on the right listing the file, the color m](https://mythaprism.com/manual_assets/m6/bl_ui_import_c.jpg)

*A print imported with the add-on: the flowers at 120 mm, the MythaPrism panel on the right listing the file, the color mode and the filaments bottom → top.*

The import sets millimeter units, switches Blender's color management to *Standard* (Blender's default look desaturates filament colors), removes the default cube and light, places the print at its true size with the top showing the colors MythaPrism synthesized, puts one collection per filament in the outliner, locks the transforms and frames the view. The panel's header names the file, its size, the layer heights and the MythaPrism build that made it.

**Colors.** **Translucent** (on by default) lets thin top layers show the stack beneath them, like the real plastic, off, every part shows its plain filament color, the slicer's view. **Exact** turns lighting off the colors so they match the MythaPrism preview pixel for pixel. The ⟳ button rebuilds the materials.

## The stack, layer by layerpage 131

![The Filaments list with Pink opened on layer 6, and the print cut at that layer with the layer selected on its own.](https://mythaprism.com/manual_assets/m6/bl_panel_layer.jpg)
![The Filaments list with Pink opened on layer 6, and the print cut at that layer with the layer selected on its own.](https://mythaprism.com/manual_assets/m6/bl_ui_layer_c.jpg)

*The Filaments list with Pink opened on layer 6, and the print cut at that layer with the layer selected on its own.*

The **Filaments · bottom → top** list shows every filament as a swatch with its real layer count, *Black, 17 layers*, *Pink, 14 layers*. Click a name to select that filament's parts. Open one with ▸ and it lists the print layers it occupies and a button for each of its layers: pick one and every filament is cut at the top of that layer, with the layer itself selected as its own object and its height shown (*Pink · layer 6 of 14 · print layer 13 · z 1.08 to 1.16 mm*). The toggle beside the list switches between showing the stack below the layer and the layer alone. **Show the whole print** puts everything back.

## Printer constraintspage 132

![Printer constraints: the Bambu Lab H2C drawn around the print at true scale, with its build volume glowing in rainbow ed](https://mythaprism.com/manual_assets/m6/bl_ui_printer_c.jpg)

*Printer constraints: the Bambu Lab H2C drawn around the print at true scale, with its build volume glowing in rainbow edges.*

Pick your printer (Bambu Lab H2C, H2D, X1C / P1S, A1 and A1 mini, Prusa CORE One and MK4 / MK4S, Creality Ender 3 and K1 / K1C, or a **Custom** build volume) and switch on **Show the printer**. The plate, a 10/50 mm grid, the build volume and the printer’s cage are drawn around the print at true size (since 1.6.0 no print head or rods hang over it), with a label naming the printer and its volume. The panel reads **Fits · 120 × 74 × 2 mm**, or turns red with **Too big on X** (or Y, or Z), useful the moment you start adding geometry.

## The Showroompage 133

![The showroom's hero shot: a plinth with the glowing MythaPrism logo and a rainbow light ring, a rainbow line on the back](https://mythaprism.com/manual_assets/m6/bl5_solar_0.jpg)

*The showroom's hero shot: a plinth with the glowing MythaPrism logo and a rainbow light ring, a rainbow line on the back wall, neutral white lights.*

**Open the showroom** stands the print on a low black slotted display stand on a turntable plinth in a black showroom: a curved backdrop, a glossy plinth with the MythaPrism logo and a rainbow light ring, a rainbow LED line on the back wall, softbox key, fill and rim lights, an 85 mm camera with depth of field, Cycles on your graphics card, and a full turn of the turntable. The show face always turns to the camera: a Slim print made face-down, or Dual's Image 1, is turned round first, the way you would pick it off the plate. Leaving the showroom (**✕**) restores the view and colors you had before.

Three switches sit under the showroom button, each off until you turn it on. **Stand at 90°** stands the print straight up instead of leaning it back 8°, so a full turn shows both faces evenly. **Side mirrors** puts a tall, wide mirror either side of the stage, angled to the camera, so the whole back of a two-sided print (Dual, Hybrid) shows in the same shot. **Backlight** opens its own box (Brightness, Warm, Neutral or Cool) and puts a light box right behind the print, inside its edges: the light shines through a LithoPrism print like a real lithophane and the studio lights dim. Any other print gets a glowing halo round its edges. In Plug-in and Showroom 1.5.5 the layer view shows every layer solid, big layers too.

**Turntable video: one full turn.** Pick the length (2 to 30 seconds), the size (1920 × 1080, 1280 × 720, square 1080 × 1080, or vertical 1080 × 1920 for Reels, Shorts and TikTok) and the quality (Draft, Good, Best), then press **Render turntable video**: Blender renders the print making one full turn and saves an .mp4 (H.264) next to your .blend file, or in your Videos folder. A Best-quality minute on a graphics card takes a while. Try Draft first to check the framing.

![The showroom panel (camera flipper, Clean full view and Render shot, version 1.5 adds three switches and the Turntable v](https://mythaprism.com/manual_assets/m6/bl_panel_showroom.jpg)
![The showroom panel (camera flipper, Clean full view and Render shot, version 1.5 adds three switches and the Turntable v](https://mythaprism.com/manual_assets/m6/bl_ui_showroom_c.jpg)

*The showroom panel (camera flipper, Clean full view and Render shot, version 1.5 adds three switches and the Turntable video box) and the showroom it builds. Here the flowers print.*

Side mirrors · Dual

Backlight · LithoPrism

Stand at 90° · Hybrid

![The 1.5 switches: a Dual print between the Side mirrors, a LithoPrism Moon with the Backlight on, a Hybrid print standin](https://mythaprism.com/manual_assets/m6/bl5_dual_0_mirrors.jpg)
![The 1.5 switches: a Dual print between the Side mirrors, a LithoPrism Moon with the Backlight on, a Hybrid print standin](https://mythaprism.com/manual_assets/m6/bl5_litho_1_backlight.jpg)
![The 1.5 switches: a Dual print between the Side mirrors, a LithoPrism Moon with the Backlight on, a Hybrid print standin](https://mythaprism.com/manual_assets/m6/bl5_hybrid_1_upright.jpg)

*The 1.5 switches: a Dual print between the Side mirrors, a LithoPrism Moon with the Backlight on, a Hybrid print standing straight up.*

Under the showroom button, **◀ Camera n/7 ▶** flips through seven ready-made shots (**Ctrl + Shift + ← / →** in the viewport), each shown clean. No grid, no gizmos, no menus. **Clean full view** fills the window with the shot, **Render shot** renders it (F12 works too). The seven angles:

1 · Hero

2 · Straight on

3 · Low hero

4 · High three-quarter

![](https://mythaprism.com/manual_assets/m6/bl5_solar_0.jpg)
![](https://mythaprism.com/manual_assets/m6/bl5_solar_1.jpg)
![](https://mythaprism.com/manual_assets/m6/bl5_solar_2.jpg)
![](https://mythaprism.com/manual_assets/m6/bl5_solar_3.jpg)

5 · Side profile

6 · Close-up

7 · Wide room

![The seven camera angles on the planets print (the curved planets montage, V1.2): hero, straight on, low hero, high three](https://mythaprism.com/manual_assets/m6/bl5_solar_4.jpg)
![The seven camera angles on the planets print (the curved planets montage, V1.2): hero, straight on, low hero, high three](https://mythaprism.com/manual_assets/m6/bl5_solar_5.jpg)
![The seven camera angles on the planets print (the curved planets montage, V1.2): hero, straight on, low hero, high three](https://mythaprism.com/manual_assets/m6/bl5_solar_6.jpg)

*The seven camera angles on the planets print (the curved planets montage, V1.2): hero, straight on, low hero, high three-quarter, side profile, close-up and wide room.*

These are product photos without a camera: a print you haven't made yet can have a listing picture, a thumbnail for a video or a mock-up for a customer. Render the turntable for a short loop.

## Add your own geometrypage 135

Blender can add anything to a print: a sculpted mountain on a map, a raised rim on a coaster, a frame, 3D lettering. The rule is simple, **whatever you join into a filament's object prints in that filament.**

![Olympus Mons (a NASA/JPL Viking picture of Mars, public domain) color-matched in MythaPrism (V1.3) and imported, the vol](https://mythaprism.com/manual_assets/m6/proj_mars_blender_import.jpg)
![Olympus Mons (a NASA/JPL Viking picture of Mars, public domain) color-matched in MythaPrism (V1.3) and imported, the vol](https://mythaprism.com/manual_assets/m6/bl_render_mars_bed.jpg)
![Olympus Mons (a NASA/JPL Viking picture of Mars, public domain) color-matched in MythaPrism (V1.3) and imported, the vol](https://mythaprism.com/manual_assets/m6/bl_render_mars_close.jpg)

*Olympus Mons (a NASA/JPL Viking picture of Mars, public domain) color-matched in MythaPrism (V1.3) and imported, the volcano built as a real mesh printing in Latte Brown, the print laid flat in the Showroom, close up.*

1. **Add → Mesh → Cone** (or any shape). **S** scales it, **G** moves it. Sink its base a millimeter into the print so it doesn't float. Sculpt mode works too.
2. Select the new shape, then Shift-select the filament object it should print in, and press **Ctrl + J** to join them. The shape now belongs to that filament.
3. Switch on **Show the printer** to check it still fits.

## Back to the slicerpage 135

**Export for the slicer (.obj + .mtl)** writes the model in millimeters, Z up, one group per filament (`Black`, `Jade_White`, `Cocoa_Brown` …), the `.mtl` with the filament colors and a `_README.txt` naming which part prints in which filament. In Bambu Studio or OrcaSlicer: **File → Import** the `.obj`; when asked whether to load it **as a single object with multiple parts, answer Yes**, right-click each part and set its filament. The parts are named after the filaments, so it is a one-to-one pick. Slice at the layer height you exported with and print.

Without the add-on

Set **Scene Properties → Units → Length: Millimeters, Unit Scale 0.001**, then **File → Import → glTF 2.0**. The objects arrive named by filament but loose, and the colors look dull until you set the view transform to *Standard*. To export by hand: **File → Export → Wavefront (.obj)** with Forward **Y**, Up **Z**, Scale **1**, Grouping **Object Groups**.

**The MythaPrism theme.** **MythaPrism theme** gives Blender a dark interface with MythaPrism's accents, **Blender default** restores yours. **Apply MythaPrism scene settings** re-applies millimeters, the Standard look and the preview lighting if you've changed them.

13

# What you can make

Fourteen things people actually make, each as a click path through the Tool, the App's sheets carry the same controls. Every project starts the same way: enable the filaments you own, bring in the picture, pick an engine.

## A product line from your camera rollpage 137

Bookmark

Two-sided coaster

Pendant

Jigsaw puzzle

![](https://mythaprism.com/manual_assets/m6/proj_bookmark_3d.jpg)
![](https://mythaprism.com/manual_assets/m6/proj_coaster_3d.jpg)
![](https://mythaprism.com/manual_assets/m6/proj_earring_3d.jpg)
![](https://mythaprism.com/manual_assets/m6/proj_puzzle_3d.jpg)

Card with braille

Olympus Mons

Glowing landscape

Gallery piece

![A few of the objects in this chapter: a bookmark, a two-sided coaster, a pendant, a puzzle, a card, Olympus Mons built i](https://mythaprism.com/manual_assets/m6/proj_idcard_3d.jpg)
![A few of the objects in this chapter: a bookmark, a two-sided coaster, a pendant, a puzzle, a card, Olympus Mons built i](https://mythaprism.com/manual_assets/m6/bl_render_mars_close.jpg)
![A few of the objects in this chapter: a bookmark, a two-sided coaster, a pendant, a puzzle, a card, Olympus Mons built i](https://mythaprism.com/manual_assets/m6/bl5_valley_5.jpg)
![A few of the objects in this chapter: a bookmark, a two-sided coaster, a pendant, a puzzle, a card, Olympus Mons built i](https://mythaprism.com/manual_assets/m6/bl5_solar_3.jpg)

*A few of the objects in this chapter: a bookmark, a two-sided coaster, a pendant, a puzzle, a card, Olympus Mons built in Blender, a glowing landscape and a gallery piece.*

| Idea | Mode and tools | Plan |
|---|---|---|
| Glowing portraits, pets, landscapes | Relief Prism + V25 · Dither 3.0 Pro (Plus: V1.3 / V1.6) |  |
| Posters, signs, logos, menus | Slim Prism · spot color · Mural for big ones | Plus · Pro |
| Keychains, ornaments, coasters, cards | Dual Prism · shape crop · hole punch | Plus |
| A sculpted front with a poster back | Hybrid Prism | Pro |
| A person or pet raised over a scene | Focus Prism | Pro |
| Night-lights and window pieces | LithoPrism | Pro |
| A restyled photo or a cut-out | 2D image editing · Filters · Cut out pieces | Free · Plus · Pro |
| Puzzles, sets, walls | Puzzle cut · Multi crop · Mural | Free · Plus · Pro |
| Tactile pieces and signage | Add text → Braille | Plus · Pro |
| Maps, dioramas, awards with modelled parts | Blender round trip | Pro |

## 1. Bookmarkpage 138

![A 50 × 150 mm bookmark: the crop preset and a tassel hole, and the 3D preview.](https://mythaprism.com/manual_assets/m6/proj_bookmark_2d.jpg)
![A 50 × 150 mm bookmark: the crop preset and a tassel hole, and the 3D preview.](https://mythaprism.com/manual_assets/m6/proj_bookmark_3d.jpg)

*A 50 × 150 mm bookmark: the crop preset and a tassel hole, and the 3D preview.*

1. Bring in a tall photo. **✎ Edit → ⬚ Crop → Bookmark 50 × 150**. The preset frames the picture and sets the print size at once. Position the picture, then **Crop**.
2. **Color match → V25 (Plus: V1.3). Stay in **Relief Prism** for a bookmark that glows against a window, or launch **Slim Prism** for a thin, fast, glass-flat one.
3. **⌫ Hole punch → circle**, drag it near the top for the tassel.
4. **T Add text** for a name or a line of poetry, a filament already in the stack prints flush.
5. **Export → .3mf + shareable PDF.** Slice at 0.08 mm, print, thread the tassel.

## 2. Two-sided coasterpage 139

![A round Dual Prism coaster, the flowers on one face (Zoned V1.8 obj), the U.S. flag on the other (V1.8 obj), and its 3D ](https://mythaprism.com/manual_assets/m6/proj_coaster_2d.jpg)
![A round Dual Prism coaster, the flowers on one face (Zoned V1.8 obj), the U.S. flag on the other (V1.8 obj), and its 3D ](https://mythaprism.com/manual_assets/m6/proj_coaster_3d.jpg)

*A round Dual Prism coaster, the flowers on one face (Zoned V1.8 obj), the U.S. flag on the other (V1.8 obj), and its 3D preview.*

1. Bring in the top picture. **⬚ Crop → Shapes → Circle**. Set Print size to about **95 × 95 mm**. Match it (V1.3 or V1.7 give the cleanest flat parts).
2. Mode pill → **Dual Prism → Launch**. Choose the back picture, place it against the mirrored ghost, **Place picture**, and answer **new palette**.
3. Pick **Image 2** and set its own engine and count (6 to 9 colors).
4. Raise the **Transition layer** to 2 to 3 layers for a stiffer coaster. Turn on your slicer's Ironing for the top face.
5. **Export.** Make a set by exporting again with the next pictures, or with **Multi crop**.

## 3. Pendant or earrings with a jump-ring holepage 140

![A small round cut-out with a jump-ring hole, flat Slim version in 2D and 3D.](https://mythaprism.com/manual_assets/m6/proj_earring_2d.jpg)
![A small round cut-out with a jump-ring hole, flat Slim version in 2D and 3D.](https://mythaprism.com/manual_assets/m6/proj_earring_3d.jpg)

*A small round cut-out with a jump-ring hole, flat Slim version in 2D and 3D.*

1. Bring in a picture with a clear subject. Cut it out with **⧉ Cut out pieces** (the print's edge becomes the outline) or **⬚ Crop → Shapes → Circle / Heart / Star** at **22 to 30 mm**.
2. **Slim Prism**, **V1.3 or V1.7 with 3 to 5 bold colors, tiny parts want few colors.
3. **⌫ Hole punch → circle**, shrink it to about 2 mm, drag it to the top edge.
4. **Nozzle 0.2 mm** (Pro) for the finest detail, **0.08 mm** layers. Print a pair from one plate.

## 4. A jigsaw puzzle giftpage 141

![A 4 × 5 puzzle of a painted solar-system chart (V25), the interlocking tabs are real, and the 3D preview.](https://mythaprism.com/manual_assets/m6/proj_puzzle_2d.jpg)
![A 4 × 5 puzzle of a painted solar-system chart (V25), the interlocking tabs are real, and the 3D preview.](https://mythaprism.com/manual_assets/m6/proj_puzzle_3d.jpg)

*A 4 × 5 puzzle of a painted solar-system chart (V25), the interlocking tabs are real, and the 3D preview.*

1. Bring in the photo. **V25.3**, or the **Family portrait** preset for a classic three-filament look.
2. **Relief** for a glowing gift, **Slim** for a flat puzzle. A 200 × 150 mm puzzle fits any 256 mm bed.
3. **Add-ons → Puzzle cut → ✎ Edit**: **Across 5, Down 4** for twenty pieces, **Gap 0.4 to 0.5 mm**, **Tray** on for a framed set.
4. Want a message on the back? Launch **Dual Prism** and place a plain card with **Add text** as Image 2.
5. **Export → .3mf + shareable PDF.** The PDF's piece map doubles as the gift card.

## 5. A card, badge or luggage tag with braillepage 142

![A card-size Slim print with a name and its braille, in 3D, and the Add text tool with Braille on.](https://mythaprism.com/manual_assets/m6/proj_idcard_3d.jpg)
![A card-size Slim print with a name and its braille, in 3D, and the Add text tool with Braille on.](https://mythaprism.com/manual_assets/m6/proj_idcard_text.jpg)

*A card-size Slim print with a name and its braille, in 3D, and the Add text tool with Braille on.*

1. **⬚ Crop → Card 85.6 × 54**, real credit-card size.
2. **Slim Prism** with **Print face-up**, so the picture and the braille sit on the open top.
3. **T Add text → + New text**: type the name. Add a second text with the same words and tap **⠿ Braille (tactile)**, Grade 1 braille at true ADA size.
4. Line them up with the **⊞ Grid**. Add a **Hole punch** for a lanyard. **Export**, print at 0.08 mm.

## 6. A portrait or landscape that glowspage 142

![A painted solar-system chart printed on V25, in the showroom from two camera angles. The steps below are the same for a ](https://mythaprism.com/manual_assets/m6/bl5_valley_1.jpg)
![A painted solar-system chart printed on V25, in the showroom from two camera angles. The steps below are the same for a ](https://mythaprism.com/manual_assets/m6/bl5_valley_5.jpg)

*A painted solar-system chart printed on V25, in the showroom from two camera angles. The steps below are the same for a portrait.*

1. Enable a wide range of filaments including a good black and white. Bring in the photo.
2. **V25 (Plus: V1.6, which keeps small accents). Nudge **Skin tones** to suit the subject. A little **Contrast** lifts the eyes.
3. **Dither 3.0** (Pro) or 2.0 for the smooth gradients of a face. **Relief test v2** if a thin bright rim around the hair would print as a wall.
4. Base **Auto: lightest selected** for a print that glows when back-lit. For the person raised over a flat scene, use **Focus Prism** instead.
5. Display it in front of a window or an LED panel.

## 7. A wall-sized poster (Mural)page 143

1. **Working resolution → 4096 px** (Pro), then bring in a high-resolution picture.
2. **V25.2 or V1.7 for a clean surface, **Slim Prism** for a flat, glass-smooth face.
3. **Add-ons → Mural → ✎ Edit**: set the **Finished width** (say 2 ft), a **Tile size** that fits your bed, **Auto-fit**. **Size it up** to see it beside a person or a door.
4. **Export**: one file, one plate per tile. Print, then mount the tiles by label on a board.

## 8. A night-light lithophanepage 143

1. Bring in a photo with strong light and shade. Mode pill → **Litho** → **V8 Litho (backlit)**, **V2·V8 Litho (fine detail)** or **V34 Litho** for clean layers with no dither.
2. The first time, **Export → V8 calibration tile** and print it with your cyan, magenta, yellow, black and white spools.
3. **Export → .3mf**. Print at 100 % infill exactly as set. Mount it in a frame with an LED strip behind.

## 9. A restyled photo to frame (no print needed)page 143

1. Bring in the photo. It opens in **2D image editing** by itself.
2. Add-ons → **Filters**: pick a look on the thumbnails (Solid Color Fill V2, Posterize Tone or Pro Halftone), grade the color, **Apply filter**.
3. Edit → **⧉ Cut out pieces** → **Cut out subject**, fix the edge with Fill subject by click or the Brush, then **Cut out: remove background** and **Use the cut-out for workspace**.
4. Save → **Save edited prime image (.png)**. To print it after all, pick a Prism mode. The print matches the edited picture.

## 10. A keychain for everyonepage 143

1. Bring in the group photo. **Add-ons → Multi crop → Create 3 crops**: frame a different person in each and round the corners.
2. **Slim Prism**, **V1.3 with 6 colors so the set shares one palette. **Hole punch** each crop (switch crops with the thumbnail bar).
3. **Export**: one file, three plates. Order more copies from a print service with the same file (Chapter 10).

## 11. A business card nobody throws awaypage 144

1. Bring in the logo. **⬚ Crop → Card 85.6 × 54**. **V1.3 with 2 to 4 colors, Spot color** the exact brand color if needed.
2. **Dual Prism → Launch**. For Image 2 use a plain light picture, then **▣ Add image** for a QR code (30 mm or larger) and **T Add text** for the name and number.
3. **Transition 1 layer** to keep the card thin. **Export.**

## 12. A tactile photo with a braille captionpage 144

1. **V25**, Relief Prism: the zoned engines give strong, touchable height differences.
2. **Relief test v2** so thin lines become grooves, which read well under a fingertip.
3. **Add text → ⠿ Braille** along the bottom edge on a flat part of the picture.
4. **Auto: lightest selected** base, 0.08 mm layers.

## 13. Olympus Mons on Mars, built in Blender, the round trippage 144

![Olympus Mons on Mars (NASA/JPL, public domain) color-matched with V1.3 in the Tool, in 3D, and with the volcano built as](https://mythaprism.com/manual_assets/m6/proj_mars_2d.jpg)
![Olympus Mons on Mars (NASA/JPL, public domain) color-matched with V1.3 in the Tool, in 3D, and with the volcano built as](https://mythaprism.com/manual_assets/m6/proj_mars_3d.jpg)
![Olympus Mons on Mars (NASA/JPL, public domain) color-matched with V1.3 in the Tool, in 3D, and with the volcano built as](https://mythaprism.com/manual_assets/m6/proj_mars_blender_mons.jpg)

*Olympus Mons on Mars (NASA/JPL, public domain) color-matched with V1.3 in the Tool, in 3D, and with the volcano built as a mesh in Blender, seen from the side.*

1. Bring in a **terrain picture you have the rights to**. Your own photo or drawing, or a public-domain picture. Never a game or film map. (This one is Olympus Mons on Mars from NASA’s Viking Orbiter, NASA/JPL, public domain. NASA does not endorse MythaPrism.) Seven Mars colors from the Bambu PLA Basic and Matte lines: Black, Dark Chocolate, Cocoa Brown, Caramel, Terracotta, Latte Brown and Desert Tan. **Print size 180 mm**, **0.08 mm layers, V1.3 or V25.
2. **Export → Blender file (.glb, colors included).**
3. In Blender, **Import MythaPrism print (.glb)** from the MythaPrism tab (Chapter 12).
4. Build the volcano where the picture shows it. A circle grid (**Add → Mesh → Circle** with **Fill Type: Triangle Fan**, then **Subdivide**), shaped in **Sculpt mode** or with **Proportional Editing**: a broad, gentle shield, the steep cliff ring around its base, and the caldera pits at the top (the **Draw** brush with **Ctrl** digs them). Sink its edge a millimeter into the print and give it the filament it should print in as its material (or **Ctrl + J** it into that filament). **Export 3MF for the slicer** then sends it with the print, and in the Showroom **Lay flat** shows its height from the side. Smaller jobs need less: a cone for a peak, four bevelled cubes for a frame.
5. **Export for the slicer (.obj + .mtl)**, in the slicer import it as one object with multiple parts and set each part's filament.

## 14. Product shots before you printpage 145

1. Match and export any print as a **.glb**.
2. In Blender: import it, press **Product showcase**, flip the **Camera** until the angle is right, **Render shot**.
3. Use the render as a listing picture, a mock-up for a customer or a thumbnail for your video, then print the one they choose.

## More ideas on the same pathspage 145

Realtor closing gifts (the listing photo as a Focus Prism relief) · recipe cards (dish on one side, steps on the other) · plant markers with a photo and care notes · magnet sets from a month of photos (Multi crop + Slim) · holiday ornaments with a different picture per side · classroom maps in touchable relief · window sun-catchers (LithoPrism) · shop signage (Slim + Mural + spot color) · award plaques with a modelled frame (Blender) · board-game tiles and terrain (Blender). Every one of them is a mode, a crop, an edit tool and an export you have already seen.

Other people's pictures

Print what you own or have permission to use. Fan art, characters, logos and other people's photos belong to their owners. A MythaPrism plan or license doesn't grant rights in them, and selling prints of them needs the owner's permission (Chapter 14).

14

# Plans, privacy and your rights

What each plan includes, what happens to your photos, what you may do with what you make, and how MythaPrism's own name and inventions are protected.

## Planspage 147

|  | Free | Plus | Pro |
|---|---|---|---|
| **Colors in a print** | 2: black and white | up to 6 | as many as the picture needs |
| **Nozzle and layer height** | 0.4 mm nozzle at 0.08 mm | 0.4 mm nozzle, every layer height (0.08 to 0.28 mm) | + the 0.2 mm and 0.6 mm nozzles, every layer height (0.06 to 0.14 · 0.18 to 0.42 mm) |
| **Engines** | the B&W engine (smooth or halftones) | the B&W engine, V1, V1.3, V1.4, V1.5, V1.6, V1.7 auto · gap · obj (one stack, any printer) | every engine: + V1.8 auto · gap · obj, V2 1.0, the zoned engines, twenty CMYK engines and LithoPrism |
| **Print modes** | Relief | + Slim, Dual | + Hybrid, Focus, LithoPrism |
| **Dither and surface** | - | Dither 1.0, 2.0 | + 3.0, 4.0, relief tests, CMYK switches |
| **Prism Modifiers** | Tone, Brightness, Contrast | every slider | + the stack action buttons |
| **Edit tools** | Crop | the whole toolkit, text and braille | the same |
| **Add-ons** | Puzzle cut | + Multi crop, Filters, Image Grading | + Mural, Reassign bands |
| **2D image editing** | ✓ (crop + 3 sliders) | ✓ | ✓ |
| **Pictures** | PNG, JPG, WebP up to 3 MB | every format your device opens, up to 15 MB | every format, no size limit, up to 4096 px working resolution |
| **Filament calibration** | - | ✓ | ✓ |
| **Save project, PNGs, Package zip** | - | ✓ | ✓ |
| **Blender .glb, OBJ + MTL** | - | - | ✓ |
| **MythaPrism Plug-in and Showroom** | $14.99 one-time | $14.99 one-time | $14.99 one-time · included in the Studio Bundle |
| **Shareable PDF** | watermarked | ✓ | ✓ |
| **Print downloads a month** | 10 with a free account · 10 more for $1.99 (never expire) | unlimited | unlimited |
| **See your photo in color** | rough preview (on your device, watermarked) | full-color prints | full-color prints |
| **Devices signed in** | 1 | 2 | 3 |

**Creator** and **Studio** are Plus and Pro with the **commercial license** to sell the prints and files you make. Current prices, early-bird pricing and the bundles are on **mythaprism.com/pricing**. Every purchase on mythaprism.com carries a **14-day money-back guarantee**. Purchases made in the Apple App Store or Google Play are refunded through Apple or Google.

**Changing plans.** On a plan from mythaprism.com, open your account page, **Subscription**, **Change plan** to switch between Plus and Pro, monthly and yearly, or a bundle, on the same subscription. Before you confirm it shows the numbers from Paddle: what you pay now (the new plan for the rest of your billing period, minus the unused part of the old one), or the credit you get when you move down, and your next payment. If the payment does not go through, nothing changes. Moving from monthly to yearly starts the new cycle on the day you switch. The 14-day money-back guarantee covers a plan-change payment too, and a refund of it puts you back on the plan you had. A plan bought in the App Store or Google Play is changed there.

**Signing in.** You can open and use the free edition without signing in. Downloading a print file (.3mf or STL) on Free needs a free account. The photo stays on your device either way. A free account downloads **10 print files each calendar month** (they come back on the 1st). Downloading the same print again in the same month does not count. If you need more black-and-white prints, a **download pack** adds 10 for $1.99: one time, never expire, used after the monthly 10. Plus and Pro have no download limit.

**Upgrading from inside the tool.** The Free tool shows every Plus and Pro button, switch and menu row too. Locked, with nothing behind them. Tap one to see what it is, which plan has it and the plans card (where a pack of 10 more black-and-white downloads is always offered). Every 🔒 message has a **See plans ›** button: tap it for a card with the plan, yearly or monthly billing, the early-bird price and the standard price, and one button to checkout (Plus users see Pro). On Free, after a black-and-white match, **See it in color** shows a rough, watermarked idea of your photo in color, painted on your device from common filament colors, not a print plan, a real Plus or Pro color print looks different. Paid plans sign in without a password: Google, Apple or an e-mail link. Signing in on one device more than your plan allows signs the oldest one out.

![The upgrade card from a tapped 🔒 message (left) and, on Free, the rough color preview of the photo with the 10-download ](https://mythaprism.com/manual_assets/m6/t_upcard_plus.jpg)
![The upgrade card from a tapped 🔒 message (left) and, on Free, the rough color preview of the photo with the 10-download ](https://mythaprism.com/manual_assets/m6/t_upcard_preview.jpg)

*The upgrade card from a tapped 🔒 message (left) and, on Free, the rough color preview of the photo with the 10-download pack (right).*

## Your photos and your privacypage 149

**Your photos stay on your device** on every plan: every engine, the preview and the export run in your browser or on your phone, and the Tool keeps working offline once it has loaded. If any planning ever moves to MythaPrism's servers, the Privacy Policy is updated first and says exactly what is sent. Nothing you export is stored anywhere except where you save it. The full details are in the Privacy Policy at mythaprism.com/privacy.

## What you may make and sellpage 149

- **You own your prints.** What you make from your own pictures is yours.
- **Other people's work stays theirs.** A MythaPrism plan or license gives you no rights in anyone else's photos, artwork, characters, logos or likeness. Fan art of a film or game character is still that character's owner's. Printing someone else's photo needs their permission.
- **Selling needs two things:** the commercial license (Creator or Studio) and the rights to the picture. When you sell, you are the seller. MythaPrism is not a party to the sale.
- **Some things are off limits** whatever the picture: parts for firearms or weapons, and anything the Terms of Service list as prohibited. Printed parts are decorative. Don't use them where a failure could hurt someone.

The Terms of Service, the End-User License Agreement and the Refund Policy at mythaprism.com set out the details.

## MythaPrism's name, code and inventionspage 150

**Trademark.** MYTHAPRISM™ and the MythaPrism hexagon logo are trademarks of MythaPrism LLC (U.S. trademark application serial no. 50131240).

**Copyright.** The MythaPrism Tool, the MythaPrism app, this manual and the MythaPrism website are © 2026 MythaPrism LLC. All rights reserved. The code of the MythaPrism Plug-in and Showroom is free software under the GNU General Public License. The MythaPrism name, logo and the Studio scene that ship with it are not.

**Patents.** Several constructions and methods in this manual were invented at MythaPrism. U.S. provisional patent applications on them are being prepared. We will say “patent pending” only once they are on file.

**Trade secrets.** The engines' internal methods and parameters are confidential. The End-User License Agreement doesn't permit reverse-engineering, probing or scraping them.

**Other people's names.** Bambu Lab, Bambu Studio, AMS, OrcaSlicer, PrusaSlicer, Prusa, Snapmaker, FlashForge, Creality, Elegoo, Polymaker, Blender, Apple, iPhone, Safari, Google, Android and the other product names in this manual are trademarks of their owners. They are used only to say what MythaPrism works with. MythaPrism is not affiliated with or endorsed by any of them.

**Fonts and pictures.** This manual is set in Anton, Inter and Space Mono, each © its project authors and used under the SIL Open Font License 1.1 (openfontlicense.org). Every example picture in this manual is a real photograph or painting. None is AI-generated. The space pictures are NASA images in the public domain (credits: NASA/JPL, NASA/SDO, NASA Goddard Space Flight Center, NASA/JPL-Caltech/Space Science Institute, NASA Scientific Visualization Studio). NASA does not endorse MythaPrism or its products. The flowers on black is a commissioned painting used with the artist’s permission, the U.S. flag is in the public domain.

15

# Reference

The cheat-sheet, the keyboard shortcuts, answers to the questions people ask most, and the words this manual uses.

## Cheat-sheetpage 152

| You want… | Reach for |
|---|---|
| Select one exact detail (a single stripe, one letter) | Zoom in, then the Brush in the tool with a small Size, Chapter 3 |
| Edit a photo and save it as a picture (no print) | Edit Prime: the edit tools + Prism Modifiers, then Save ▾ → Save edited prime image (.png), Chapter 3 |
| Glowing photographic art on any printer | Relief Prism + the V25 family (Plus: V1.3 / V1.6) + Dither 2.0 or 3.0 |
| Flat, fast, no swaps | Slim Prism + a small color count |
| A different picture on each face | Dual Prism + Dual backing (+ Flip horizontal) |
| A relief with a poster back | Hybrid Prism |
| A subject raised over a flat scene | Focus Prism |
| A full-color lithophane | LithoPrism → a V8 Litho or V2·V8 Litho engine |
| Just edit the picture, no print | 2D image editing (mode bar) |
| A print that must stay under a set height | Print setup → Height limit |
| Snap-apart pieces | Puzzle cut (every print mode) |
| An exact brand color in one area | Spot color |
| A specific outline | Crop → Shapes, or Cut out pieces |
| A hanging hole | Hole punch (it cuts through the backing too) |
| Continuous color from five spools | V4·V8.1 or V3·V8.1 (print the CMYK calibration tile first) |
| Five CMYK spools, clean smooth layers | V4·V8.3 (the smoothest CMYK surface) |
| Several products from one picture | Multi crop: one file, three plates |
| A wall-sized print | Mural + 4096 px working resolution |
| A busy photo that matches and prints calmly | Filters → Solid Color Fill V2 or Posterize Tone, then match, Chapter 8 |
| Print only part of the picture | Cut out pieces → Split → select the pieces → Use this for workspace, Chapter 6 |
| Color the picture myself, section by section | Add-ons → Reassign bands → select sections, pick colors → Build print (the match reads Manual), Chapter 8 |
| See the untouched photo | Press and hold the rainbow **Hold to see original** icon, bottom left of the picture |
| Colors that match your real spools | The calibration plate + Calibration V4 |
| A print on a single-nozzle printer | Relief with the swap guide on a one-stack engine (V1.3 to V1.8, V2 1.0) |
| Someone else to print it | .3mf + shareable PDF → a friend, a makerspace or a print service |
| Product photos before printing | Blender file → MythaPrism Plug-in and Showroom → Product showcase |
| To try something and go back | ↶ Undo / ↷ Redo |

**These don't combine:** a dither and the relief tests (a dither turns the tests off) · relief test v1 and v2 · Relief and the flat modes.

## Keyboard shortcutspage 153

| Keys | Where | What |
|---|---|---|
| Ctrl/⌘ + Z | Tool | Undo |
| Ctrl + Shift + Z or Ctrl + Y | Tool | Redo |
| Mouse wheel | Tool stage, edit tools | Zoom toward the cursor |
| Shift + drag | Edit tools | Pan |
| Drag · right-drag · wheel | 3D view | Rotate · move · zoom |
| N | Blender 3D viewport | Open the sidebar with the MythaPrism tab |
| Ctrl + Shift + ← / → | Blender showroom | Previous / next camera angle |
| Ctrl + J | Blender | Join a shape into a filament's object |
| F12 | Blender | Render the current shot |

## Troubleshootingpage 154

| What you see | What to do |
|---|---|
| The sliced colors are wrong, but MythaPrism's preview is right | Slot mapping: you imported into a project that was already open. Open the `.3mf` fresh (File → Open), or line your AMS slots up with the Filament change schedule. |
| The previous color streaks into the next one right after a change | Turn on the prime tower in your slicer (MythaPrism leaves it off) and slice again, raise the flush volumes if it persists. |
| The print is darker or duller than the preview | Thin color-over-color layers print duller than the library values predict. Print and read a calibration plate (Chapter 9) and leave Calibration V4 on. |
| Skin prints too orange | Use the V25 family (Plus: V1.6) and nudge **Skin tones**. |
| The dithered surface is spiky | Use Dither 2.0 or 3.0, the same detail without tall peaks. |
| Grays vanished next to black on a Family preset | Use Dither 3.0, whose cap is measured in color steps. |
| Thin outlines print as tall, fragile walls | Relief test v2 (v1 for maximum clean-up). |
| The relief test removed small details | Switch from v1 to v2. |
| Fine details vanish | Raise the color count, turn off Smoother surface, or switch the relief test to v2. |
| The second picture in Dual or Hybrid has only two colors | Pick that picture's side and raise its Colors count. |
| The two faces don't line up | Use **⇄ Flip horizontal** when placing the second picture. |
| An edit changed the wrong picture | In the two-picture modes, pick Image 1 or Image 2 first, the tools follow the selected side. |
| Text prints raised | Pick a text color already in the stack for flush text. |
| A no-backing print fell apart | Islands surrounded by empty space have nothing holding them. Turn the backing on. |
| Puzzle pieces fused | The gap was below about 0.3 mm, raise **Gap**. |
| The projected shadow is blurry | Use one bright point light, not a room lamp, with the wall a few feet away. |
| A HEIC photo won't open in the browser | Chrome and Windows can't read HEIC. Use JPG or PNG, open it in Safari or the MythaPrism app, or set the iPhone camera to *Most Compatible*. |
| Blender shows loose objects and a dull picture | You used File → Import → glTF. Use the MythaPrism tab's **Import MythaPrism print (.glb)** instead. |
| The slicer shows different colors than MythaPrism's preview | Normal: a slicer draws each part in its filament's solid color. The thin translucent layers only blend on the real print, the MythaPrism preview and the Blender add-on's import show that blended look. |
| The print came out shorter than usual, with fewer tones | Print setup → **Height limit** is set. Choose **Dynamic** to let the engine plan its own height again. |
| The page feels slow after a long session | **Refresh workspace** in the account panel. Your library, presets and settings are kept. |

## Glossarypage 156

| Term | Meaning |
|---|---|
| **Prime** | Your picture with the 2D edits applied, what the engine matches. |
| **Manual** | What the color matcher reads after Reassign bands builds a print: you chose the colors, MythaPrism worked out the layers (Chapter 8). |
| **Edit Prime** | The state a picture opens in before any color match: the edit tools and Prism Modifiers work on the photo itself, and Save edited prime image writes it out as a PNG (Chapter 3). |
| **Synthesized result** | The close estimate of the finished print, computed from the filament stack. |
| **Band** | A run of layers printed in one filament. |
| **Stack** | The sequence of bands from the plate to the top. |
| **Stop** | The height a point's column ends at. The color at that height is what shows. |
| **Zone** | A region of the picture that a zoned engine gives its own stack. |
| **Composite** | A stop made of thin layers of several filaments. How the V25 family reaches colors no single filament has. |
| **Swap** | A filament change at a specific layer, listed in the schedule and the PDF. |
| **Spot color** | A region you choose, printed in one exact filament. |
| **Filter** | An add-on style (Rotoscope, Flat Poster …) that restyles the photo into flat color shapes before matching. |
| **Transition layer** | The slab joining the two faces of a Dual or Hybrid print. |
| **Light Depth (LD)** | MythaPrism's per-filament number (mm) for how far light travels into a filament, **typ** = typical, **est** = estimated. Not the same as the "TD" other tools publish. |
| **Hiding thickness** | Measured from your calibration plate: the front-lit thickness at which a filament hides a white-vs-black backing (ΔE00 ≤ 3). Shown as Hides at in the calibration results. |
| **Measured profile** | A filament's opacity over white and over black, read from your calibration plate. |
| **ΔE** | A measure of color difference. About 2 is barely visible, about 10 a clear but acceptable shift. |
| **Dither** | A fine pattern of two printable colors that reads as the tone between them. |
| **Peak cap** | The rule that no point may stand more than a set amount above its tallest neighbor. |
| **Engraved valley** | A thin ridge carved below its surroundings by a relief test. |
| **2D image editing** | The mode for the picture alone, edits never re-match the print until you go back to a Prism mode. |
| **Cut out pieces** | The edit tool that cuts the subject out or splits the picture into pieces to merge, edit, save or print on their own. |
| **Height limit** | The optional global cap (3 to 7 mm) on how tall any print may be. Dynamic lets each engine decide. |
| **Action rail** | The column of controls beside every edit tool (beneath the picture on a phone). |
| **.3mf** | The print-job file slicers open, with geometry, presets and colors inside. |
| **.glb** | The 3D file Blender and other 3D apps open, with the colors on the model. |

## Supportpage 157

In the account panel, the gray **Help** box under **Support** searches this manual: type a few words and pick the part you need, it opens here on mythaprism.com. **Support** holds **Send feedback**, **Report a bug** (a short form: write what went wrong and how to make it happen. It is posted as a public report in the MythaPrism community on GitHub, with your build and setup if you leave that ticked and a short code instead of your name or e-mail, and never with your pictures. You can send one report a day. If the report service cannot be reached, it opens an e-mail to support instead), **Build notes and updates** (what changed in each update, on mythaprism.com and on GitHub) and **Email support**. Or write to **support@mythaprism.com**. The website has the tutorials, this manual and the Filament Calibration Guide. MythaPrism LLC · PO Box 47373, Windsor Mill, MD 21244 · (410) 929-6308.

MYTHAPRISM USER MANUAL · BUILD 635 · © 2026 MYTHAPRISM LLC
