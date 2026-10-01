---
name: find-the-moment
description: Find where something was said in the user's RiverScript transcripts. Use when they ask what was decided, agreed, promised or quoted, when they half-remember a conversation, or when they ask which meeting something came up in.
---

People rarely remember which transcript holds the thing they are looking for. Start from the words, not from the list.

1. Call `search_transcripts` with the phrase the user would have heard, not a paraphrase of their question. For "what did we agree about the price", search `price`, then `pricing`, then `discount`. The search matches the phrase as written, so short and literal beats long and clever.
2. If nothing comes back, try the other word people use for the same thing, and only then fall back to `list_transcripts` to see what exists at all. Narrow with `from` and `to` when the user gives a time, such as "last month" or "before the launch".
3. Answer from the passages that come back. Quote the words that settle the question, and say which transcript and date they came from, so the user can open it themselves.
4. Fetch the full text with `get_transcript` only when the passage is not enough, for example when the user asks how the discussion went rather than what was decided.

If two transcripts disagree, say so and give both, with their dates. The later one is usually the decision, but say which is which rather than choosing silently.
