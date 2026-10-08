# Recruitment AI Team — Starter

A low-cost, human-supervised AI recruitment workflow for Poland.

## Architecture
Telegram (intake) → n8n (orchestration) → AI Director (routing) → specialist agents → Trello (tasks) → human approval.

## Agents
- `agents/director.md`: routes requests and enforces approval rules.
- `agents/recruiter.md`: candidate communications and qualification.
- `agents/job-manager.md`: vacancy normalization and matching.
- `agents/marketer.md`: drafts compliant vacancy posts.
- `agents/legal.md`: flags legal questions for human review.
- `agents/analyst.md`: KPI definitions and reporting.

## MVP milestones
1. Create Telegram bot and secure n8n instance.
2. Telegram message → n8n → director classification → Trello card.
3. Add specialist drafts with human approval before sending/publishing.
4. Add structured vacancy/candidate records in a private, access-controlled system.

## Security
Never commit personal candidate data, passport scans, phone numbers, access tokens, credentials or `.env` files. This repository is PUBLIC. Keep secrets in n8n credentials and personal data in a private, GDPR-compliant system. Avoid automated posting/sending without approval and platform authorization.
