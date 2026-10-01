---
name: lecture-notes
description: Turn a transcribed lecture, webinar, talk or training session into study notes. Use when the user asks to revise from a recording, wants key terms explained, needs a summary of what was taught, or asks to be tested on it.
---

A lecture transcript is a wall of speech. What a student needs from it is structure, terms, and something to test themselves against.

1. Find it with `list_transcripts` when the user names the course or the date, or `search_transcripts` on a term that would have been said in it.
2. Fetch the full text with `get_transcript`. Lectures build an argument from beginning to end, and a search passage taken out of the middle usually misleads.
3. Write notes in this order:
   - the thesis the lecture argues, in one or two sentences
   - the sections it moves through, each with what was actually claimed
   - the terms that were defined, with the definition the speaker gave rather than the standard one
   - the examples used, because they are what gets remembered in an exam
4. When the user asks to be tested, ask questions one at a time and wait for the answer. Mark what was wrong against what the lecture said, quoting the line.

Keep the speaker's definition even when it is loose or unusual. If it conflicts with the standard one, note both and say which came from the lecture: that is the one being examined.

If the user asks about something the lecture never covered, say so rather than filling it in from elsewhere, then offer the general answer separately.
