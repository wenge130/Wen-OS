---
name: process-voice-memo
description: SOP for transcribing and processing iPhone Voice Memos into structured meeting notes, action items, and decisions.
---

# Process Voice Memo

This skill converts Wen's iPhone Voice Memo recordings into structured, actionable meeting notes.

## Context
Wen records meetings and ideas using iPhone Voice Memos. These recordings need to be transcribed and organized into structured notes that can be referenced, actioned, and stored in Google Workspace.

## Workflow

### Step 1: Transcription
When Wen provides an audio file (exported from Voice Memos):
1. Transcribe the audio using the available transcription tool.
2. Clean up the raw transcript (remove filler words, fix obvious errors).

### Step 2: Structure the Notes
Format the cleaned transcript into the following structure:

```
## Meeting Notes — [Date]
**Attendees:** [List if mentioned]
**Topic:** [One-line summary]

### Key Discussion Points
[3-5 bullet points summarizing the main topics]

### Decisions Made
[Any firm decisions reached during the meeting]

### Action Items
| Owner | Task | Deadline |
|---|---|---|
| Wen | [task] | [date] |
| [Other] | [task] | [date] |

### Open Questions
[Any unresolved questions that need follow-up]
```

### Step 3: Log & Archive
1. Ask Wen if any decisions should be logged in `decisions/log.md`.
2. Save the structured notes to Google Workspace (remind Wen to copy the output there).

### Step 4: Follow-up Drafts
If the meeting involved an external party (client, vendor, partner), offer to draft a follow-up email using `references/voice.md` to match Wen's tone.
