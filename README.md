# Game Day Weather for Cursor

Cursor plugin for Game Day Weather. It connects Cursor to the public, read-only Game Day Weather MCP server. You get NFL kickoff weather calls (CLEAR, WATCH, FLAG, DOME) for each game. No account or API key is needed.

Not affiliated with the NFL. Not live scores, odds, or picks.

## Tools

- `get_week_board`: Full public board for one NFL week (regular season weeks 1 to 18).
- `get_game`: One game, by team code or game id.
- `get_flags`: Games whose call is FLAG or WATCH.
- `get_report_card`: A published Sideline report card, the same cards as /report-cards.
- `get_changes`: Games whose published call, roof, window, or kick-window reading moved.
- `get_call_history`: Every published snapshot for one game, oldest first.
- `get_team_games`: Published weather for NFL team codes on one week.

All tools are read-only.

## Install config

Add this to your Cursor `mcp.json`:

```json
{
  "mcpServers": {
    "game-day-weather": { "url": "https://gamedayweather.app/mcp" }
  }
}
```

Endpoint: `https://gamedayweather.app/mcp` (streamable HTTP, no auth).

## Other AI apps

See https://gamedayweather.app/add for ChatGPT, Claude, Grok, and Perplexity.

## Terms

Free for agents and AI answers with attribution. Not for model training. See https://gamedayweather.app/terms.
