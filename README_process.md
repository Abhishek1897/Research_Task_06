# Deep Fake Interview – Process Documentation

## Goal
Transform Task 05 narrative insights (SU sports team seasonal stats) into a synthetic interview showcasing data-driven talking points.

## Narrative Source
- Task 05 outputs (games = 19; offense focus; Emma Ward = offensive leader; Joely Caramelli = most improved; scoring 1st vs 4th periods; no neutral-site games; Emma Ward top efficiency).

## Tools Used
- **edge-tts** (Microsoft free text-to-speech CLI/Python) – quick synthetic voices.
- **Coqui TTS** – alternative with more voices.
- **Audacity** – for mixing and editing audio.
- **(Optional)** Wav2Lip – for lip-syncing video to audio.
- **(Optional)** Shotcut – for video editing and captions.

## Workflow
1. **Script** drafted (host + coach).
2. **TTS generation**: two voices (host and coach) via edge-tts or Coqui TTS.
3. **Mixing** in Audacity: aligned dialogue, trimmed silences, normalized audio.
4. **Optional video path**: Wav2Lip for lip-sync, Shotcut for editing and captions.
5. **Export**: final MP3 (audio-only) or MP4 (video).

## Iterations & Issues
- Adjusted pacing and speaking rate in TTS.
- Mixed multiple takes to improve flow.
- Lip-sync experiments had artifacts; static audio submission chosen.

## Ethics & Labeling
- This media is **AI-generated** for coursework.
- No attempt to impersonate real people; voices are synthetic defaults.
- Real names (Emma Ward, Joely Caramelli) are used only as part of a data summary, not impersonation.
- Final product is clearly labeled: “Synthetic interview generated with TTS + editing.”

## Reproduction Commands
Example with edge-tts:

```bash
edge-tts --text "Coach, looking back at last season—what stands out?" --voice en-US-AriaNeural --write-media host1.mp3
edge-tts --text "We played 19 games and learned a lot about our pacing and finishing." --voice en-US-GuyNeural --write-media coach1.mp3
```

## Time & Compute
- TTS generation: seconds per clip.
- Editing: ~30 minutes in Audacity.
- Optional lip-sync: 10–20 minutes GPU runtime if attempted.
