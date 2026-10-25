# Plot Twist

*People are more than their biodata.*

A mobile-first, illustrated narrative game prototype about turning a matrimonial biodata into curiosity, and real encounters into a scrapbook. Open `index.html` in any modern browser. There's no build step and nothing to install.

## Onboarding: what matters to you

- Four questions about past relationships (what you valued, what you wished was different, what to avoid, what surprised you). One per screen, free text, skippable and editable later. No names needed.
- The app suggests preferences from your answers (a keyword-based mock of AI extraction that runs on this device; nothing is sent anywhere). You can edit, delete or add any of them.
- You sort each one as **Non-negotiable**, **Nice to have**, **Nice to not have** or **Hard no**. Nothing is pre-sorted.
- **My preferences** (on the chapters screen and in settings) is where you review, move, edit and add preferences, or revisit the reflection behind each one. Now and then it asks "Does this still matter to you in the same way?". It never changes anything on its own.

## Chapters

**01 Filter In: unpack the biodata**
- **Filter check.** As soon as a biodata is added, it's compared against your sorted preferences. Each one is **Aligned**, **Conflict** or **Unknown**, and the profile line behind it is quoted. The results are split into *Potential incompatibilities*, *Reasons for curiosity* and *Things worth asking*. A conflict with a non-negotiable or hard no raises a pass flag, which you can dismiss. Unknowns never count as a failed match. Instead, the check suggests **First questions** to ask them, worded to filter in: it opens on something they wrote or listed, then asks about your non-negotiables and nice-to-haves, and turns any conflict into an open question ("You wrote … What does that look like for you?"). Yes/no questions come last. You can edit or save each question, or save all of them. You choose **Pass** or **Explore**, and a passed profile can be reopened from settings.
- **Images.** When adding a biodata you can attach an image: a photo of the person or a scan of the biodata itself. The image is shrunk and clipped to the form, shown on the filter check, and becomes a photo object on the table. It's never used as evidence. *Read text from image* runs text recognition (Tesseract.js) in the browser and fills in the details for you to check. It needs to download the engine from jsdelivr, which works when the page is opened directly or served locally. Where that download is blocked, the page asks you to type the details instead.
- A parcel arrives. Drag the flap (or tap) to open it, then unfold the biodata panel by panel.
- Each detail on the form becomes an illustrated object on a tabletop. You can drag objects, turn them, and tap to inspect.
- Inspecting works by touch. Drag or twist the object with two fingers to turn it, and double-tap to flip it. Swipe the question note sideways for another question, and drop it in the pocket (or tap the pocket) to save it. On a keyboard, the arrow keys and Enter do the same.
- Inspecting an object shows what the form says (**Known**) beside an optional open question (**Wondering**). You can save the question to your pocket, write your own, or leave it.
- After a few objects, an empty space appears. It holds questions a form can't answer.
- The curiosity board is a freeform space for your questions.
- When you're done, you can leave the profile for now, archive it, or get to know them. That last choice packs your chosen questions into a keepsake box.

**02 Continue?: unpack the encounter**
- *So, what happened?* Open the scrapbook to start a page for a call, messages, a conversation or a date.
- **Conversation fragments:** movable speech bubbles in your own words (theirs, yours, or a pause).
- **Memory table:** neutral moment tokens (laughter, curiosity, silence, discomfort, surprise, uncertainty, affection, or your own). Drag them, or tap a token and then tap the page.
- **What matters:** prompts built from your sorted preferences, for example "Was there a moment you felt considered or understood?". You can answer, skip, or add your own note.
- **Then, and now:** a question from Chapter One comes back. Its Known, Wondering and Experienced parts sit side by side. You can add an observation, revise the question (earlier versions are kept), or leave it unanswered.
- **The unfinished page:** *What, if anything, would you like to discover next?*
- **Connection scrapbook:** one tab per encounter, plus a "how questions changed" view. You can annotate pages and move moments or fragments between them. Continue, Pause, Close the chapter and Leave it unfinished all look and behave the same.

## Rules the game keeps

- Objects come only from lines that are actually on the form. The parser maps `Label: value` lines to objects, and hobbies it doesn't recognise become a plain tag with the hobby's name. It never infers traits.
- Evidence only comes from what the profile states in its own words (about me, expectations, lifestyle lines such as smoking). The check never reads anything into job, education, caste, religion, family background or hobbies. Hobbies can show up as "Related, not proof". No scores, rankings, timers, streaks or achievements.
- Privacy: everything stays in the browser's `localStorage`. Contact details are dropped when the biodata is parsed. Packing the keepsake box discards the paperwork and keeps only the questions you chose. Settings include deletion for each archived profile, each scrapbook, or everything at once.
- Accessibility: every drag has a tap or keyboard alternative (Tab, arrow keys, Enter). Reduced motion, sound and haptics can be toggled.

The bundled sample biodata (Rohan Deshpande) is fictional.
