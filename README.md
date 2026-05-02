# Whisper2Verbatim

Turn raw AI transcription into clean, structured verbatim.

Whisper2Verbatim is a lightweight web tool that transforms Whisper JSON output into readable, structured verbatim.

Unlike transcription tools, it focuses on the post-processing stage: making transcripts usable, structured and ready for analysis.

---

## Context

This tool was created as part of a Master’s degree research project.

While working on transcription with Whisper, I was looking for a tool that would allow me to efficiently transform raw outputs into structured verbatim. I did not find any solution that matched my needs, so I built one.

This tool is only a step in the process. It does not replace a full review of the final transcription.

Its purpose is to help regain control over the text:
- reviewing and correcting content
- reintroducing hesitations if needed
- removing or adjusting simplifications produced by Whisper

It combines automation and human validation in a practical workflow.

---

## Why not just use Whisper?

Most tools stop at transcription.

They provide:
- raw text
- fragmented segments
- poorly structured dialogue

Whisper2Verbatim focuses on what comes next:

- structured speaker formatting  
- readable dialogue  
- pause detection  
- metadata integration  
- ready-to-use verbatim  

From AI output to a usable document.

---

## Features

- Import JSON transcription files (Whisper, WhisperX, Scriberr…)
- Detect and rename speakers
- Generate structured verbatim
- Optional timecodes
- Merge segments by speaker
- Automatic pause detection
- Metadata integration (context, participants, date…)
- Export to TXT and RTF
- Copy to clipboard

---

## Example

### Input (Whisper JSON)

```json
{
  "start": 0.0,
  "end": 2.5,
  "text": "bonjour euh merci d'être là",
  "speaker": "SPEAKER_00"
}