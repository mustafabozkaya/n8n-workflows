# MrBozkay/n8n-workflows

Production-ready n8n workflow templates for AI automation, logistics, CRM, DevOps, RAG, and social media.

## Workflows

### 1. Lojistik AI Agent — Sipariş & Kargo Takip
- **File:** `workflows/01-lojistik-ai-agent.json`
- **Trigger:** Webhook (siparis-olustu)
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

### 4. RAG Pipeline — Belge → Vektör → AI Cevap
- **File:** `workflows/04-rag-pipeline.json`
- **Trigger:** Webhook (rag-soru)
- **AI Agent:** RAG agent with document search + citation tools
- **Features:** Input validation (prompt injection filter), embedding → Qdrant vector search, context re-ranking, structured output with sources + confidence, logging
- **Use case:** Şirket belgelerine dayalı AI cevap sistemi. Qdrant vektör veritabanında arama, re-ranking, kaynak gösterme

### 5. Multi-Agent Orchestration — Research → Writer → Editor
- **File:** `workflows/05-multi-agent-orchestration.json`
- **Trigger:** Webhook (multi-agent)
- **AI Agents:** Researcher → Writer → Editor (3 agent zinciri)
- **Features:** Task tracking, web + academic search tools, merge node, structured output with agent chain + quality score, Slack notification
- **Use case:** Research agent arama yapar → Writer agent taslak yazar → Editor agent düzenler. 3 agentli zincirleme orchestration

### 6. Social Media Content Pipeline — Blog → Multi-Platform
- **File:** `workflows/06-social-media-content.json`
- **Trigger:** Webhook (blog-publish)
- **AI Agent:** Content agent with hashtag + image generation tools
- **Features:** Content extraction, AI content generation, split to LinkedIn/X/Telegram, structured output, character count, logging
- **Use case:** Blog yazısı public olduğunda AI agent LinkedIn, X, Telegram için optimize edilmiş postlar üretir

## Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/mustafabozkaya/n8n-workflows.git
cd n8n-workflows

# 2. Import a workflow into n8n
# Open n8n → Workflows → Import from File → Select any JSON from workflows/

# 3. Configure credentials
# - OpenAI API key (for AI agent nodes)
# - Google Sheets API (for CRM workflow)
# - GitHub token (for code review workflow)
# - Slack webhook (for notifications)
# - LinkedIn API (for social media workflow)
# - Twitter/X API (for social media workflow)
# - Telegram bot token (for social media workflow)
# - Qdrant API (for RAG workflow)

# 4. Activate
```

## Requirements

- n8n instance (self-hosted or cloud)
- OpenAI API key (or compatible LLM provider)
- GitHub token (for code review workflow)
- Google Sheets API (for CRM workflow)
- Slack webhook URL
- Qdrant vector DB (for RAG workflow)
- LinkedIn, Twitter/X, Telegram APIs (for social media workflow)

## Tags

`lojistik` `ai-agent` `automation` `kargo` `siparis` `crm` `lead` `github` `code-review` `rag` `vector-db` `multi-agent` `orchestration` `social-media` `content`

## License

MIT