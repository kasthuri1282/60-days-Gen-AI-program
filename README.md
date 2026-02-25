# n8n Automation Workflows – Newsletter & Meeting Summary

## 🚀 Overview

This repository contains two automation workflows built using n8n:

1. AI Newsletter Automation
2. AI Meeting Summary Automation



---

# 📌 Workflow 1: AI Newsletter Automation

## 🔹 Description

This workflow generates a formatted newsletter using AI and:

- Saves it as a Gmail Draft
- Sends it to a Slack channel

## 🔄 Workflow Architecture
Schedule Trigger->Tavily->AI agent->Split out ->Tavily ->AI agent -> Aggregate ->AI agent→ Gmail Draft → Slack Message

## ✨ Features

- scheduled triggered automation
- AI-powered newsletter generation
- Automatic Gmail draft creation
- Slack channel delivery
- Structured & formatted output

## 📤 Output

- Gmail draft ready to review & send
- Slack formatted newsletter post

---

# 📌 Workflow 2: AI Meeting Summary Automation

## 🔹 Description

This workflow processes meeting transcripts and generates a structured meeting summary which is automatically posted to Slack.

## 🔄 Workflow Architecture

Webhook → AI Summary Generation → Format Output → Slack Message

## ✨ Features

- Accepts Zoom/Meeting transcript input
- AI-generated structured summary
- Action items extraction
- Automatic Slack posting

## 📤 Output

- Clean meeting summary in Slack
- Highlighted action items

---

# ⚙️ Setup Instructions

## 1️⃣ Import Workflows

- Open n8n
- Import the provided JSON files

## 2️⃣ Configure Credentials

Add the following credentials in n8n:

- Slack OAuth Bot Token
- Gmail OAuth2 Credential
- OpenAI (or other LLM provider) API Key

## 3️⃣ Update Nodes

- Set correct Slack Channel ID
- Verify Gmail account connection
- Activate workflow

---

# 🔐 Required Credentials

- Slack Bot Token (`chat:write`, `channels:join`)
- Gmail OAuth2
- LLM API Key

⚠️ Do NOT upload API keys in this repository.

---

# 🛠️ Use Cases

- Daily team meeting automation
- Sprint update summaries
- Weekly newsletter generation
- Marketing updates
- Internal communication automation

---

# 📂 Files Included

- newsletter-workflow.json
- meeting-summary-workflow.json
- README.md

---

# 🧠 Tech Stack

- n8n
- Slack API
- Gmail API
- OpenAI / LLM API

---

# 📜 License

MIT License
