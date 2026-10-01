---
name: interview-notes
description: Turn recorded interviews into structured notes, and compare several of them. Use for customer and user interviews, candidate interviews, research sessions and expert calls, and when the user asks what people said about a topic across conversations.
---

An interview is worth more as structure than as prose, and worth most when it can be compared with the others.

1. Find the interview with `list_transcripts` when the user names it, or `search_transcripts` when they describe what was discussed. For a candidate or a customer, their name is usually said out loud and searchable.
2. Fetch it with `get_transcript` and read it whole. Interviews turn on wording, hesitation and what a person returned to twice, and a search passage loses that.
3. Produce notes in the shape the user asked for. When they did not ask for a shape, use: what the person wants, what gets in their way today, what they do instead, and quotes worth keeping, verbatim and marked as quotes.
4. For a comparison, fetch each interview and answer question by question rather than person by person, so the agreement and disagreement are visible in one place. Name who said what.

Keep the person's words separate from the reading of them. A quote and a conclusion look alike in a summary and matter very differently to the person deciding on it.

When a transcript is a translation made in RiverScript, say so where you quote it: the wording is the translator's, not the speaker's.
