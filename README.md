# RiverScript plugin for Claude

Work with your [RiverScript](https://riverscript.com) transcripts in Claude.

RiverScript records and transcribes meetings, calls, lectures, podcasts and interviews. It captures the audio playing on your computer from any app, with no bot joining the call, and transcribes audio and video files up to 50 GB and 8 hours long, in 100 languages.

This plugin bundles the RiverScript connector with four skills that tell Claude what to do once it has your transcripts:

- **find-the-moment** — search what was said across your transcripts and answer with the passage, the transcript it came from and its date.
- **meeting-followup** — pull decisions, owners and deadlines out of a meeting and draft the message that goes out afterwards.
- **interview-notes** — turn customer, user and candidate interviews into structured notes, and compare several of them question by question.
- **lecture-notes** — turn a lecture or training session into study notes, key terms and questions to be tested on.

## Installing

Install the plugin, then connect RiverScript on the plugin's **Connectors** tab and sign in with your RiverScript account. The connector is read-only: it reads your transcripts and translations and changes nothing.

## Connector

The plugin points at the RiverScript MCP server at `https://riverscript.com/api/mcp/v2`, which is also listed in the Claude directory on its own. Install both and you get one set of tools, not two.

Documentation: [riverscript.com/docs/platform-details/mcp](https://riverscript.com/docs/platform-details/mcp)

## License

MIT, see [LICENSE](LICENSE).
