---
name: meeting-followup
description: Turn a recorded meeting or call into decisions, owners, deadlines and the message that goes out afterwards. Use when the user asks for minutes, action items, a recap, a follow-up email, or what they committed to on a call.
---

The work after a meeting is always the same: what was decided, who owes what, and the message that goes out.

1. Find the meeting. If the user named it, use `list_transcripts` and match on the title and date. If they described it instead, `search_transcripts` on a phrase that would have been said in it.
2. Check `get_transcript_summary` first. When RiverScript already generated a summary, it saves reading the whole thing. When it returns nothing, that is normal: fetch the text with `get_transcript`.
3. Pull out, in this order, and only what the transcript actually supports:
   - decisions, each with the reasoning if it was given
   - actions, each with an owner and a date when one was named, and plainly marked as unassigned when not
   - open questions that were raised and left unanswered
4. Write the follow-up in the register of the meeting. A team call gets a short message. A client call gets a formal recap. Lead with the decisions, keep the actions as a list, and put open questions last.

Never invent an owner or a deadline that nobody said. "No owner was named" is a useful line in a recap; a guessed name is a problem the user discovers in a week.

If the user wants the message sent, hand them the draft. Sending is theirs.
