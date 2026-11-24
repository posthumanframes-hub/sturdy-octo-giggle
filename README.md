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
- **Edit** any journal entry from the timeline to change how you felt, the type or the text. Saving re-tags it, but tags you recoloured or cleared yourself stay as you left them.
- Tap any tag to see the sentence it came from, change its colour, or clear it. *Re-check* re-runs the first match after you change your preferences.
- Auto-tagging is a simple keyword reading that runs on the device (nothing is sent anywhere), so it will miss things and sometimes misread them. That's why every tag can be changed.
- **View profile** shows the form as a grid of little objects (tap one to see it up close). The full biodata lines and any attached image are folded away under *Full profile* until you tap it.
- **Photos:** each folder has a strip of polaroids. Tap *Add photos* to add one or several at once. Tap a photo to see it large, make it the **cover** (shown in the folder header and on Home), or remove it. Photos are shrunk before saving. If the browser's storage fills up, the app tells you instead of silently dropping anything.
- Each folder has a status (Exploring, Paused, Closed, Passed) and can be renamed, **archived** (moved off the main grid into a folded *Archived* section at the bottom of Home, and back again) or deleted.

## Stress and how you handle it (the VSA model)

A light take on the Vulnerability-Stress-Adaptation model (Karney & Bradbury), which looks at how a relationship is shaped by what each person brings, the stress around them, and how they adapt together. It lives entirely in the journal and is read from what you write. There's no separate section:
- **Stress:** a sentence like "rough week at work" or "stressful time with family" is tagged as context, for example **☁ Work stress**. It isn't a flag and doesn't count toward the tally.
- **Adaptation:** in an entry that reads as stressful, how you handled it is tagged too. "Talked it through", "was there for me" or "listened" earns a green *Under stress* flag. "Went quiet", "snapped", "argued" or "brushed it off" raises a yellow one.
- **Vulnerabilities:** *What I bring* in your preferences holds your own sore spots or patterns. When an entry reads as stressful, one comes back under the tags as a gentle reminder.
- Like every tag, these can be recoloured or cleared.

## Rules it keeps

- Objects come only from lines that are actually on the form, and evidence only comes from what the profile states in its own words (about me, expectations, lifestyle lines such as smoking). The match never reads anything into job, education, caste, religion, family background or hobbies.
- An unknown is never a flag. Flags are reviewable and can be cleared.
- Privacy: everything is stored **on this device only**, in the browser's IndexedDB, which has room for photos (with `localStorage` as a fallback). Older saves move over automatically. Contact details are dropped when the biodata is parsed, and preference suggestions are worked out on the device. Settings can delete everything, and each folder has its own delete.
- **Look:** in Settings, choose **Mode** (System, Light or Dark) and one of three **palettes**: Butter (warm butter and coral), Lagoon (sea-glass blue and teal) or Plum (mauve, plum and marigold). Each palette has a light and a dark version. System follows your device or the Claude viewer.
- Reduced motion, sound and haptics can be toggled.

The bundled sample biodata (Rohan Deshpande) is fictional.

## Design system

Follows *Plot Twist: Source-grounded design system* (v4, unified edition):
- Fraunces carries titles and anything you read or write. Nunito runs the interface. Metadata is at least 11px.
- Semantic aliases (`--surface-*`, `--text-*`, `--action-primary`, `--border-*`, `--status-*-paper`) sit on top of the original palette tokens. Spacing (`--space-1` to `--space-10`), `--radius-control` (8px) and `--touch-target` (44px) are tokens too.
- Paper objects stay light in dark mode and can be tilted or irregular. Controls are 8px-radius, 44px, and never rotated. Flag colours mean the same thing in every palette.
- Checked across Butter, Lagoon and Plum in light and dark, at 320px and 375px wide: meaningful text meets WCAG AA contrast. The operating system's reduced-motion setting turns off all animation.

