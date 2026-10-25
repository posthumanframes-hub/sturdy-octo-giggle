# Plot Twist

*People are more than their biodata.*

A mobile-first, illustrated narrative game prototype about turning a matrimonial biodata into curiosity, and real encounters into a scrapbook. Open `index.html` in any modern browser. There's no build step and nothing to install.

## Chapters

**01 Filter In: unpack the biodata**
- **First read.** As soon as a biodata is added, the game checks it against filters you set yourself: age, height, diet, location, education, community, manglik and interests, each marked Off, Nice or Must. A rubber stamp then shows *Likely pass*, *Likely fail* or *Not enough info*, along with whether the form covers enough basics (9 are checked) and the reason behind every check. Any profile can still be unpacked.
- A parcel arrives. Drag the flap (or tap) to open it, then unfold the biodata panel by panel.
- Each detail on the form becomes an illustrated object on a tabletop. You can drag objects, turn them, and tap to inspect.
- Inspecting an object shows what the form says (**Known**) beside an optional open question (**Wondering**). You can save the question to your pocket, write your own, or leave it.
- After a few objects, an empty space appears. It holds questions a form can't answer.
- The curiosity board is a freeform space for your questions.
- When you're done, you can leave the profile for now, archive it, or get to know them. That last choice packs your chosen questions into a keepsake box.

**02 Continue?: unpack the encounter**
- *So, what happened?* Open the scrapbook to start a page for a call, messages, a conversation or a date.
- **Conversation fragments:** movable speech bubbles in your own words (theirs, yours, or a pause).
- **Memory table:** neutral moment tokens (laughter, curiosity, silence, discomfort, surprise, uncertainty, affection, or your own). Drag them, or tap a token and then tap the page.
- **Then, and now:** a question from Chapter One comes back. Its Known, Wondering and Experienced parts sit side by side. You can add an observation, revise the question (earlier versions are kept), or leave it unanswered.
- **The unfinished page:** *What, if anything, would you like to discover next?*
- **Connection scrapbook:** one tab per encounter, plus a "how questions changed" view. You can annotate pages and move moments or fragments between them. Continue, Pause, Close the chapter and Leave it unfinished all look and behave the same.

## Rules the game keeps

- Objects come only from lines that are actually on the form. The parser maps `Label: value` lines to objects, and hobbies it doesn't recognise become a plain tag with the hobby's name. It never infers traits.
- The only verdict is the first read. It compares what the form literally says with your own filters, shows each reason, and doesn't infer anything. The game has no compatibility scores, timers, streaks or achievements.
- Privacy: everything stays in the browser's `localStorage`. Contact details are dropped when the biodata is parsed. Packing the keepsake box discards the paperwork and keeps only the questions you chose. Settings include deletion for each archived profile, each scrapbook, or everything at once.
- Accessibility: every drag has a tap or keyboard alternative (Tab, arrow keys, Enter). Reduced motion, sound and haptics can be toggled.

The bundled sample biodata (Rohan Deshpande) is fictional.
