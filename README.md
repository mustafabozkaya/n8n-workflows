# MrBozkay/n8n-workflows

Production-ready n8n workflow templates for AI automation, logistics, CRM, DevOps, RAG, and social media.

## Repository Structure

- `workflows/` — Ready-to-import production workflows, organized by category

- `analysis/` — Duplicate/issue workflows identified during portfolio audit (19 of 80)


## Categories

| Category | Production | Analysis | Description |
|---|---|---|---|
| `automation` | 3 | 1 | Daily AI news, data sync between apps, Google Sheets to Meta |
| `call-center` | 8 | 4 | STT, LLM analysis, S3 upload, Slack/Telegram notifications for call centers |
| `content` | 2 | 0 | Resume analysis, LinkedIn post generation |
| `database` | 14 | 10 | PostgreSQL/MySQL sync, maps upload, infrastructure setup, voice analysis |
| `dev-tools` | 8 | 1 | n8n Developer Agent, Workflow Builder, code execution, file upload |
| `lead-gen` | 6 | 1 | Instantly lead generation, GMB radar, Google Maps scraping |
| `media` | 2 | 1 | AI video generation, Flux image generation, ElevenLabs TTS |
| `multi-agent` | 3 | 0 | Multi-agent orchestration, voice assistants, collaborative research |
| `other` | 12 | 0 | Chat triggers, webhooks, utility workflows |
| `rag-ai` | 3 | 1 | RAG pipelines, vector embeddings, knowledge stores, document processing |

## Production Workflows


### Automation

- 📰 Daily AI Summary
- Sync new data between two apps
- Google Sheets to Meta Business Daily Data Sync

### Call Center

- Call Center Analysis with OPENROUTER_LLM
- Slack Call Center Analysis with LLM
- Slack Call Center Analysis2
- IMPROVED CALL CENTER S3 UPLOAD
- Slack Call Center Analysis
- Slack Call Center Analysis with LLM
- CALL CENTER S3 UPLOAD
- Workflow 1: STT & Transkript İşleme

### Content

- REsume Analysis
- Generate AI-Powered LinkedIn Posts with Google Gemini and Gen-Imager

### Database

- CALL_CENTER_OLLAMA_LLM_AGENT_ANALYSİS (May 29 at 10:09:55)
- CALL_CENTER_MULTİ_AGENT_ANALYSİS_ADVANCED
- Workflow2_LLM Analysis_deepseek/deepseek-r1-0528-qwen)
- CALL_CENTER_AGENT
- CALL_CENTER_AGENT_analyze
- CALL_CENTER_3_SERİAL_LLM_AGENT_ANALYSİS(May 30 at 11:11:34)
- CALL_CENTER_S3_Analysys
- send data postgres
- End to end Cali Voice Analysis Agent
- upload_Maps_screenshots
- PostgreSQL to MySQL Sync (Manual Setup)
- Infrastructure Setup and Validation Workflow
- Infrastructure Setup and Validation Workflow
- AGENT_CECK_NODES

### Dev Tools

- Workflow Builder
- N8n Developer agent (finalquery, sources)
- Enhanced n8n Developer Agent
- N8n Developer agent with upload Execute node
- n8n Developer Agent - File Upload Processor
- Enhanced Workflow Builder
- n8n Developer Agent (File Upload)
- Advanced n8n workflow agent

### Lead Gen

- GMB Radar Report Scraper (Sep 1 at 20:48:28)
- GMB Radar Report Scraper
- Google Maps Email Scrapinng
- INSTANTLY_lead_advanced_generate_with_olama_gender
- INSTANTLY_lead_advanced_generate_openaı_gender
- lead_advanced_generate

### Media

- Flux generation respond with Premium Page
- AI Video Generator

### Multi Agent

- Voice assistant agent
- Multi Agent System
- Collaborative Research and Fact-Checking Report Generator

### Other

- Chat Trigger Call Analysis with OpenRouter
- Chat Trigger Call Analysis with OpenRouter
- ?
- My workflow
- İNstantly
- AI Agent with Webhook for Open WebUI
- Email Agent
- LLM Multi-Agent
- Translate audio using AI
- Create json file
- Firecrawl Extract agent
- Generating Hyper-Personal

### Rag Ai

- Multi-Source Document Processing with Vector Embeddings and AI Chatbot
- Demo: RAG in n8n
- Knowledge store agent (with Google Drive)

## Analysis (Duplicate / Issue Workflows)

These 19 workflows were identified during portfolio audit and excluded from production:

- **Exact duplicates**: 2 copies of `Slack Call Center Analysis2`

- **Near-duplicates**: 11 groups with identical node type sets

- **Missing trigger**: 3 workflows without any trigger node

- **Empty**: `Daily AI News to Telegram` has 0 nodes

- **Missing credentials**: 21 workflows reference no credential configurations


## Quick Start

```bash
git clone https://github.com/mustafabozkaya/n8n-workflows.git
cd n8n-workflows

# Import a workflow into n8n

# Open n8n → Workflows → Import from File → Select any JSON from workflows/


# Configure credentials

# - OpenAI API key (for AI agent nodes)

# - Anthropic API key (for Claude nodes)

# - Google Gemini API key

# - DeepSeek API key

# - Ollama (local or remote)

# - Slack webhook URL

# - Telegram bot token

# - AWS S3 credentials

```
