# INKFLOW — AI book writer & story generator (MCP server)

**An AI book writer and AI story generator for any AI agent: write a book, a book series, an SOP or a manual.** INKFLOW is a UK book-writing studio with a public
[Model Context Protocol](https://modelcontextprotocol.io) server. Your agent can try it free (no key, no signup),
get a firm quote, place an order and collect the finished work — books, series, manuals, translations,
audiobooks and TikTok / YouTube promo videos.

- **Website:** https://inkflowstudio.org
- **MCP endpoint (streamable HTTP):** `https://api.inkflowstudio.org/api/mcp`
- **Official MCP Registry:** `org.inkflowstudio/inkflow`
- **Claude:** listed in Claude's connector directory as INKFLOW (search "inkflow")

## Try it free — no key

`inkflow_write_free_chapter` writes **Chapter 1 of a novel** (in one of 11 writing voices), or a section of a
**manual, technical spec or medical guide**, from a sentence or two — in about a minute, in 22 languages.

## Connect

Any MCP client that supports remote servers:

```json
{
  "mcpServers": {
    "inkflow": { "type": "http", "url": "https://api.inkflowstudio.org/api/mcp" }
  }
}
```

## Tools

| Tool | What it does |
|---|---|
| `inkflow_write_free_chapter` | Free Chapter 1 / manual section — no payment, no key |
| `inkflow_capabilities` | The full catalogue, with live prices |
| `inkflow_quote` | A firm price quote without ordering, in your currency |
| `inkflow_order` | Place a paid order (book, series, manual, translation, audiobook, short or YouTube video) |
| `inkflow_job_status` | Live progress and delivery links |
| `inkflow_balance` / `inkflow_topup` | Prepaid credit, so an agent can buy without a checkout page |
| `inkflow_free_samples` | Free samples of trained digital-actor and set models |
| `inkflow_train_ultra_lora_actor` / `inkflow_choose_actor_face` | Commission a trained digital actor |
| `inkflow_sell_your_lora` | List your own trained model sets for sale |

## How orders work

- **Pay up front, delivered or refunded** — an order that cannot be delivered is refunded automatically.
- Prices are quoted in your currency; a human pays once through Stripe, or an agent pays from prepaid credit.
- AI-generated video carries an AI-generated label, as the platforms require.

## This repository

This repository holds the public description of the server (`server.json`, mirroring the Official MCP Registry
entry) so directories can list it. The server itself is hosted by INKFLOW; there is nothing to install.

Contact: inkflowmail@gmail.com

## Guides

- [Write a book with AI](https://inkflowstudio.org/write-a-book-with-ai) — one sentence to a finished manuscript
- [Write a book series with AI](https://inkflowstudio.org/write-a-book-series-with-ai) — up to 10 books kept consistent
- [Fantasy story generator](https://inkflowstudio.org/fantasy-story-generator) — the whole novel, not a paragraph
- [AI romance story generator](https://inkflowstudio.org/ai-romance-story-generator) — the full love story, your tropes
- [AI SOP generator](https://inkflowstudio.org/ai-sop-generator) — company manuals and procedures that never invent facts
