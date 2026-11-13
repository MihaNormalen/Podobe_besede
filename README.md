Type a word or a sentence, and images tagged with it fly across the screen. A browser-based VJ tool in a single HTML file: no install, no build step, no API key.

It is a remake of an old Flash (SWF) piece that played on the link between words and the images the internet attaches to them.
https://app.assembla.com/spaces/dominik-mahnic/wiki/Besede_Podobe_(2010)

Run it

Open wordspace.html in a current browser (Chrome, Edge, Firefox or Safari). It needs an internet connection to fetch images.

To host it on GitHub Pages, rename the file to index.html (or link to wordspace.html), then turn on Pages for the repository under Settings → Pages.

A search can be put in the address, which is handy for bookmarks and links:

wordspace.html#ocean
wordspace.html#red%20house%20by%20the%20sea
How it works
You type a word or a sentence and press Enter.
The page searches two open image libraries, Wikimedia Commons and Openverse. Neither needs an account or a key.
A phrase is searched whole and also word by word (up to five meaningful words, skipping filler such as “the” and “by”), and the results are mixed.
The images are drawn on a canvas and animated. Some get words from their own titles orbiting around them.
Settings
Section	Controls
Motion	Animation, automatic change (8, 16 or 32 seconds), speed, number of images, size, share of enlarged images
Look	Blend mode, image opacity, soft edges, background colour, show the typed words, orbiting words
Feedback	Trail amount, zoom, twist
Key out	Remove a chosen colour, dark areas or bright areas, with tolerance
Sound	Source (ambient music, microphone or audio file), volume, optional slow beat, sound → size, sound → speed, level meter
Animations

Tunnel, Drift, Orbit, Spiral, Rain, Bounce, Wave, Wall, Vortex, Strobe.

Blend modes

Normal, Screen, Add, Overlay, Hard light, Difference, Exclusion, Colour dodge, Multiply, Luminosity.

Keyboard

These work whenever the search box is not focused.

Key	Action
1–9, 0	Pick an animation
Space	Pause or play
F	Fullscreen
H	Hide or show the settings panel

With the panel hidden, the Settings button and the mouse cursor fade out after a few seconds without movement, leaving a clean output for a projector.

Sound
Ambient music is generated in the browser, so there are no audio files to ship.
Microphone input drives the visuals but is not played back through the speakers. Browsers usually allow microphone access only on https:// pages or localhost.
Audio file plays a file from your computer on a loop.

The bass level of whichever source is active can drive image size and speed.

Things to know
Images come from public libraries with little filtering, so a search can occasionally return something unexpected.
Images whose pixels the browser is not allowed to read are skipped, because colour keying needs pixel access. Some searches return fewer images for that reason.
Openverse limits how many anonymous searches one address can make. If it stops answering, results continue from Wikimedia Commons alone.
The images belong to their authors and carry their own licences (mostly Creative Commons or public domain). Check the licence of anything you capture and republish.
The interface font, Bricolage Grotesque, loads from Google Fonts and falls back to a system font offline.
Ideas for later
Presets saved and recalled with one key
Tap tempo and BPM-locked changes
MIDI controller mapping
A queue of words to step through
Local images, video clips and webcam as sources
A second window for the projector
Colour effects: hue cycling, invert, glitch, kaleidoscope
Recording the output to a video file
Built with

Plain HTML, CSS and JavaScript: Canvas 2D for drawing, the Web Audio API for sound. No frameworks or dependencies.

Licence

No licence has been chosen yet. Add a LICENSE file (MIT is a common choice for small tools) before inviting others to reuse the code.
