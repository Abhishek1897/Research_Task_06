# Task_06_Deep_Fake

**Goal:** Transform the narrative from Task 05 into an AI‑generated interview.

This repository contains only the **required items** noted in the submission instructions:
- **README.md** (this file)
- **prompts/** (prompt(s) used)
- **scripts/** (script used to convert narrative → interview)

---

## What I Did (Process Overview)

1. **Defined the target format**  
   I decided on a concise Q&A interview between a *Host* and an *Analyst* (8–12 exchanges).

2. **Converted narrative → Q&A**  
   I wrote a small Python script (`scripts/build_interview_from_narrative.py`) that:
   - Reads a plain‑text narrative.
   - Uses seeded question templates aligned to common sports analysis points.
   - Maps sentences from the narrative to answers, preserving your voice while making it conversational.

3. **(Optional) Audio/Video**  
   The assignment prefers audio/video but is primarily graded on process. Audio/video is **not required** for submission. If desired, a simple TTS + audiogram can be added later (outside this minimal package).

---

## Tools I Considered

- **Local Python (standard library only)** for deterministic, reproducible conversion.  
- (Optional, not included): **pyttsx3** for offline TTS; **moviepy** for basic audiograms.

I chose not to include optional dependencies here to keep the package to *only the required files*.

---

## Workflow Steps (Reproducible)

1. Prepare your narrative from Task 05 as a text file (e.g., `narrative.txt`).  
2. Run the converter script:
   ```bash
   python scripts/build_interview_from_narrative.py narrative.txt interview_script.txt
   ```
3. Review and lightly edit the resulting Q&A for voice and clarity.

> Tip: Keep answers short and specific. Mention concrete stats or trends for credibility.

---

## Prompt(s) Used

See [`prompts/prompt_turn_narrative_into_interview.txt`](prompts/prompt_turn_narrative_into_interview.txt).  
I iterated on this prompt to bias toward short, conversational lines and clear takeaways.

---

## Submission Notes

- **Repo name:** `Task_06_Deep_Fake`  
- **Contents:** scripts, prompts, README (this repo has only those).  
- **Send link to:** `jrstrome@syr.edu`  
- **Time reporting:** Complete the Qualtrics check‑ins by **September 1**.

*(Dates and submission logistics copied from the assignment brief.)*

---

## Acknowledgments

Assignment: *Research Task 6: Deep Fake* (Process‑first emphasis).
