# Voiceovers for Reels

The standard, settled with Colin on 2026-11-09 after testing on the Mars retrograde and three-weeks Reels.

**Voice:** ElevenLabs, Sedona ("Sedona - Calm Grounded Female", voice id `Y02DpjDrIqEQiinPoGZG`), model v4, the same voice as Journeys.

**Script:** one script per video, about 25 words, a little more conversational than the words on screen (the voice says "old arguments come back" where the screen says "conflicts that were put away come back"; degrees and long numbers stay on screen only). Full sentences, few fragments.

**Rendering:** each sentence on its own, starting `[gently] [warmly] [calm and unhurried]`. A single opening tag wears off after a sentence or two, and `[softly]` makes it too breathy. Words like "quietly" can still pull a sentence breathy; re-render that one with "clear" added.

**Assembly:**
- Trim each sentence at -55 dB, keeping about 0.08 s before and 0.25 s after the words; fade in 0.06 s and out 0.22 s; level each to -18 LUFS.
- Place each sentence at its start time (0.65 s between sentences), over a faint room tone (brown noise, 60 Hz–1.5 kHz, about 40 dB under the speech), never digital silence.
- Warmth EQ: +2.5 dB at 220 Hz, -2 dB at 7.5 kHz. Start 0.5 s into the video, fade in over 0.4 s, final level -16 LUFS.

**Video:** record the Reel with its lines timed to the voice: `?cues=` (ms each sentence starts, counting the 0.5 s lead-in) and `?end=` (ms the end card comes in, about 0.3 s after the voice ends), with `REELS_MS` = end + 3 s. Each line leaves in the gap before the next sentence.

**Sound:** no trending sound under the voice (Colin, 2026-11-10). A voiced Reel goes out with its own voice and room tone only; trending sounds stay for the captions-only Reels.

**Which Reels:** the lessons, the composite sign-by-sign videos and the Mars videos are voiced (17 of the 30 in `library/2026-12`). Sky events, countdowns and the launch-day videos stay captions only, with a trending sound, and the chime on about one in five.

The scripts for those 17 are in `scripts.md` next to this file.
