# TED Europa & SEAP Public Tenders & Buyer Email Scraper

[![Run on Apify Store](https://img.shields.io/badge/Apify_Store-Run_Actor-00C853?style=for-the-badge&logo=apify)](https://apify.com/willowy_catamaran_fco/ted-europa-seap-tenders-scraper)

Extract active European Union and SEAP Romania public procurement tenders and contract awards with direct buyer emails, phones, CPV codes, and budgets.

---

## 1-Click n8n Workflow Template (Ready to Import)
Import directly into **n8n** (`Workflows -> Import from URL`) using:
`https://raw.githubusercontent.com/m3t4n01a/ted-europa-seap-public-tenders-scraper/main/n8n-workflow.json`

Or download [`n8n-workflow.json`](./n8n-workflow.json) from this repository.

## Claude Desktop / Cursor MCP Server Integration
Use this B2B intelligence engine directly inside Claude Desktop, Cursor, or Windsurf:
```json
{
  "mcpServers": {
    "ted-europa-seap-tenders-scraper": {
      "command": "npx",
      "args": [
        "-y",
        "@apify/actors-mcp-server",
        "--actors",
        "willowy_catamaran_fco/ted-europa-seap-tenders-scraper"
      ],
      "env": {
        "APIFY_TOKEN": "YOUR_APIFY_API_TOKEN"
      }
    }
  }
}
```

## Direct Synchronous REST API (cURL / Clay / Make)
```bash
curl -X POST "https://api.apify.com/v2/acts/willowy_catamaran_fco~ted-europa-seap-tenders-scraper/run-sync-get-dataset-items?token=YOUR_APIFY_API_TOKEN" \
  -H 'Content-Type: application/json' \
  -d '{"countryIso3": "ROU", "daysBack": 3, "maxItems": 30}'
```