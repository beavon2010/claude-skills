# claude-skills
## Skills

`.claude/skills/` holds the 16 Google Stitch agent skills from
[google-labs-code/stitch-skills](https://github.com/google-labs-code/stitch-skills)
(Apache-2.0, see `.claude/skills/STITCH-LICENSE`). Claude Code loads them
automatically in any session that has this repo attached.

Skills that call the Stitch API (`upload-to-stitch`, `manage-design-system`, etc.)
need a Stitch API key from https://stitch.withgoogle.com.

## Stitch MCP server

`.mcp.json` connects Claude Code to the Stitch MCP server. It reads the API key
from the `STITCH_API_KEY` environment variable (set it as a secret in your Claude
environment settings), so the key is never committed.
