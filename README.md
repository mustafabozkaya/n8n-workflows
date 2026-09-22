# MrBozkay/n8n-workflows

Production-ready n8n workflow templates for AI automation, logistics, CRM, and DevOps.

## Workflows

### 1. Lojistik AI Agent — Sipariş & Kargo Takip
- **File:** `workflows/01-lojistik-ai-agent.json`
- **Trigger:** Webhook (sipariş-olustu)
- **AI Agent:** LangChain agent with 3 tools (kargo sorgula, depo stok, priced hesapla)
- **Features:** Duplicate prevention, structured output parser, error handler, Slack notification
- **Use case:** Sipariş geldiğinde AI agent kargo oluşturur, depo stokunu kontrol eder, priced hesaplayıp Slack bildirimi gönderir

### 2. CRM Lead → Google Sheets → AI Rapor
- **File:** `workflows/02-crm-lead-ai-rapor.json`
- **Trigger:** Webhook (crm-lead)
- **AI Agent:** Lead skorlama agent
- **Features:** Duplicate prevention, Google Sheets entegrasyonu, AI lead scoring, Slack bildirimi
- **Use case:** CRM'den gelen lead'ler Google Sheets'e kaydedilir, AI skorlanır, sales team'e bildirilir

### 3. GitHub PR → AI Code Review → Slack
- **File:** `workflows/03-github-ai-code-review.json`
- **Trigger:** Webhook (github-pr)
- **AI Agent:** Code review agent
- **Features:** PR opened filter, diff fetch, AI review, PR comment, Slack notification
- **Use case:** GitHub PR açıldığında AI code review yapar, yorum ekler, Slack'da bildiririr

## Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/MrBozkay/n8n-workflows.git
cd n8n-workflows

# 2. Import a workflow into n8n
# Open n8n → Workflows → Import from File → Select any JSON from workflows/

# 3. Configure credentials
# - OpenAI API key (for AI agent nodes)
# - Google Sheets API (for CRM workflow)
# - GitHub token (for code review workflow)
# - Slack webhook (for notifications)

# 4. Activate
```

## Requirements

- n8n instance (self-hosted or cloud)
- OpenAI API key (or compatible LLM provider)
- GitHub token (for code review workflow)
- Google Sheets API (for CRM workflow)
- Slack webhook URL

## Tags

`lojistik` `ai-agent` `automation` `kargo` `siparis` `crm` `lead` `github` `code-review`

## License

MIT