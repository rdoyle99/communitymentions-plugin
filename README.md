# CommunityMentions plugin

Which subreddits AI answers cite, for AI agents (Claude, ChatGPT, Cursor, Grok Build).

This plugin connects your agent to the CommunityMentions MCP server at `https://communitymentions.com/api/mcp` (streamable HTTP, no sign-in) and adds a skill that tells the agent which tool to use.

## Tools
| Tool | What it does |
|---|---|
| `find_subreddits` | Describe a product or niche; get up to 10 subreddits where it fits, with how often AI answers cited each and member counts |
| `get_subreddit` | One subreddit's AI citations by engine (OpenAI models, Perplexity, Gemini), the kinds of questions those answers were about, and its most-cited threads |

The data covers subreddits cited 50+ times in the AI answers CommunityMentions tracks, or where it has placed 50+ verified comments. Read-only.

## Try it
- "Which subreddits fit an AI writing tool for marketers?"
- "How often do AI answers cite r/SaaS, and which threads?"

## Install
- **Claude Code / Cursor / other Agent Plugin hosts:** install this repo as a plugin, or add the server yourself:
  `claude mcp add --transport http communitymentions https://communitymentions.com/api/mcp`
- **Any MCP client:** use `.mcp.json` / `mcp.json` in this repo.

Also in the official MCP registry as `com.communitymentions/communitymentions`. Browse the data: https://communitymentions.com/subreddit-finder

License: MIT (this plugin). The data stays CommunityMentions'.
