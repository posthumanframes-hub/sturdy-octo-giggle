# Plot Twist

*Check profiles against what matters to you.*

A small, mobile-first scrapbook game for matching matrimonial profiles against your own preferences, then tracking how you feel with a person and whether there's a good balance of **Spark** (how it feels) and **Fit** (how it lines up with what matters to you). Open `index.html` in any modern browser. There's no build step and nothing to install.

## Three steps

1. **Your preferences.** Add your **non-negotiables** and your **green**, **yellow** and **red flags**. Type them in directly, or tap *Help me find them from past relationships* to answer four questions and get suggestions you can edit and sort.
2. **Add a folder.** One folder per person.
3. **Add a profile to the folder.** Paste a biodata, attach an image (optionally *Read text from image*), or use the sample. The folder is matched against your preferences straight away. That **first match** is the start of a timeline:
   - a **green flag** for each preference the profile's own words support (or, for a red or yellow flag preference, explicitly rule out)
   - a **red flag** for a clash with a non-negotiable or red flag
   - a **yellow flag** for a clash with a green or yellow flag
   - everything the profile doesn't mention is listed under *To find out*, never counted against them

## The timeline

- **Check in** after a call, chat or date:
  - how you felt with them (Off, Meh, Okay, Warm, Sparks): that's **Spark**
  - three prompts drawn from your preferences, starting with what the profile couldn't answer, each answered *Felt right*, *Not sure* or *Felt off*: that's **Fit**
  - *Felt off* raises a flag in that preference's colour, *Felt right* earns a green flag, and *Not sure* adds nothing
- The folder shows Spark and Fit on a **seesaw**. Each is a little character that grows and cheers up as it rises, and the plank tips toward whichever is ahead and sits level when they're balanced. Below it are a one-line read, a tally of green, yellow and red flags, and a **Flags over time** chart showing how they accumulate.
- Tap any flag to see where it came from, or clear it if it no longer applies. *Re-check* re-runs the first match after you change your preferences.
- Each folder has a status (Exploring, Paused, Closed, Passed) and can be renamed or deleted.

## Rules it keeps

- Objects come only from lines that are actually on the form, and evidence only comes from what the profile states in its own words (about me, expectations, lifestyle lines such as smoking). The match never reads anything into job, education, caste, religion, family background or hobbies.
- An unknown is never a flag. Flags are reviewable and can be cleared.
- Privacy: everything stays in the browser's `localStorage`. Contact details are dropped when the biodata is parsed, and preference suggestions are worked out on the device. Settings can delete everything, and each folder has its own delete.
- Reduced motion, sound and haptics can be toggled.

The bundled sample biodata (Rohan Deshpande) is fictional.
