# n8n MVP build guide

1. Create Telegram bot via BotFather. Store token ONLY in n8n Credentials.
2. Configure n8n securely (HTTPS, authentication, backups, restricted access).
3. Add Telegram Trigger for incoming messages.
4. Add AI model node with `agents/director.md` as system instructions.
5. Parse/validate JSON response; if invalid, route to manual review.
6. Add Switch on `assigned_agent`.
7. Create Trello card containing only non-sensitive summary and approval status.
8. Reply with an acknowledgement after human-approved text is available.
9. Test with synthetic sample messages, not real candidate records.

**Do not enable autonomous external sending or publication in the MVP.**
