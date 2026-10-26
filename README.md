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

## Manuals, SOPs and document rewrites

- **Write** a manual, SOP, technical specification, clinical guide or NHS-style policy: the named make and model and the current guidance (UK: NICE, CQC, HSE, MHRA) are researched first, every measured value is traced to its source, and missing facts become marked placeholders. Delivered in Word and PDF with diagrams, a document control page and a training pack.
- **Rewrite** a document you already have (`document-revision`): reviewed, checked against current guidance and rewritten in plain English, Easy Read or Simplified Technical English, every fact and value kept, with a review report, change log and comparison.
- **Read your files**: CAD (STEP, IGES, DXF, DWG), 3D-print, BIM (IFC), PDF, Word, Excel, DITA, S1000D, Visio, Gerber/KiCad and more.
- **Audio**: manuals and books narrated, with steps, warnings and "see figure 3.2" read clearly.

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
| `inkflow_order` | Place a paid order (book, series, manual, document revision, translation, audiobook, short or YouTube video) |
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
- [AI technical manual writer](https://inkflowstudio.org/technical-manual-writer) — manuals from your product, files and CAD
- [Clinical SOP and NHS-style policy writer](https://inkflowstudio.org/nhs-policy-and-clinical-sop-writer) — checked against current guidance
- [Rewrite documents in plain English](https://inkflowstudio.org/rewrite-documents-in-plain-english) — upload, review, update, rewrite
- [Convert a book, manual or SOP to audio](https://inkflowstudio.org/convert-book-to-audiobook) — figures referenced by number
