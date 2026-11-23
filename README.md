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

- **Journal entry** after a call, chat or date:
  - tap how you felt with them (Off, Meh, Okay, Warm, Sparks): that's **Spark**
  - write what happened in your own words. The helper is optional: tap *Need a hand?* to see a few starter prompts drawn from what you still want to find out, and tap one to drop it onto the page
  - as you type, the entry is **auto-tagged** against your preferences: that's **Fit**. A sentence that shows something you want, or rules out something you don't, earns a green flag. One where it leans off raises a flag in that preference's colour (red for non-negotiables and red flags, yellow for green and yellow flags). A plain mention of a preference you typed yourself counts as support.
- The folder shows Spark and Fit on a **seesaw**. Each is a little character that grows and cheers up as it rises, and the plank tips toward whichever is ahead and sits level when they're balanced. Below it are a one-line read and a tally of green, yellow and red flags.
- Tap any tag to see the sentence it came from, change its colour, or clear it. *Re-check* re-runs the first match after you change your preferences.
- Auto-tagging is a simple keyword reading that runs on the device (nothing is sent anywhere), so it will miss things and sometimes misread them. That's why every tag can be changed.
- Each folder has a status (Exploring, Paused, Closed, Passed) and can be renamed or deleted.

## Rules it keeps

- Objects come only from lines that are actually on the form, and evidence only comes from what the profile states in its own words (about me, expectations, lifestyle lines such as smoking). The match never reads anything into job, education, caste, religion, family background or hobbies.
- An unknown is never a flag. Flags are reviewable and can be cleared.
- Privacy: everything stays in the browser's `localStorage`. Contact details are dropped when the biodata is parsed, and preference suggestions are worked out on the device. Settings can delete everything, and each folder has its own delete.
- **Look:** in Settings, choose **Mode** (System, Light or Dark) and one of three **palettes**: Butter (warm butter and coral), Lagoon (sea-glass blue and teal) or Plum (mauve, plum and marigold). Each palette has a light and a dark version. System follows your device or the Claude viewer.
- Reduced motion, sound and haptics can be toggled.

The bundled sample biodata (Rohan Deshpande) is fictional.
