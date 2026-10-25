# Plot Twist

*Check profiles against what matters to you.*

A small, mobile-first scrapbook game for sorting matrimonial profiles against your own preferences and keeping track of how things go. Open `index.html` in any modern browser. There's no build step and nothing to install.

## How it plays

1. **What matters to you.** On first launch, four quick questions about past relationships (what you valued, what you wished was different, what to avoid, what surprised you). The game suggests preferences from your answers, and you sort each one as **Non-negotiable**, **Nice to have**, **Nice to not have** or **Hard no**. You can skip this and do it later. **My preferences** lets you edit, move or add preferences at any time.
2. **Home.** Your shelf: one scrapbook per person, each with a status stamp (Undecided, Talking, Paused, Closed). Passed people sit on a shelf below.
3. **Add biodata.** Paste the details, attach an image (and optionally *Read text from image*), or use the sample.
4. **Filter check.** The biodata slides in and a stamp lands with the number of pass flags. Below it are *Potential incompatibilities*, *Reasons for curiosity* and *Talk about*. Each Talk about topic shows what to listen for. Then tap **Pass** or **Explore**.
5. **Their scrapbook.** The form's details become little moving objects. Tap one to see it up close, with the line from the form and what it could point to. Your talk-about topics and your meetings are here too. Tap the status stamp to change it.
6. **Add a meeting.** Flick each topic card right (*came up*) or left (*didn't*), tap the moments that fit, add a note if you like, and choose whether to keep talking. That's it.

## Rules it keeps

- Objects come only from lines that are actually on the form, and evidence only comes from what the profile states in its own words (about me, expectations, lifestyle lines such as smoking). The check never reads anything into job, education, caste, religion, family background or hobbies. Hobbies can show up as "Related, not proof".
- An unknown is never a failed match. A pass flag can be dismissed, and a passed person can be brought back by changing their stamp.
- No scores, rankings, timers or streaks.
- Privacy: everything stays in the browser's `localStorage`. Contact details are dropped when the biodata is parsed, and preference extraction runs on the device. Settings can delete everything, and each scrapbook has its own delete.
- Accessibility: card swipes have Didn't / Came up buttons and arrow keys. Reduced motion, sound and haptics can be toggled.

The bundled sample biodata (Rohan Deshpande) is fictional.
