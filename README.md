# n8n workflows

Personal automations built with self-hosted n8n.

## Workflows

**monthly-application-report.json**
Reads my job application emails from an Outlook folder, extracts company, position and status with a local LLM (Ollama, qwen2.5:7b), groups them per company (Rejected > Interview > Applied) and serves a colored HTML report that I save as PDF once a month.

**daily-design-jobs-germany.json**
Fetches UX/Product Designer jobs from the Bundesagentur für Arbeit Jobsuche API, filters out internships and junior roles, removes duplicates and emails me a digest.

## Stack
n8n (self-hosted), Microsoft Outlook (Graph API), Ollama, JavaScript (Code nodes), HTML/CSS

## Import
In n8n: ⋯ → Import from File. Credentials (Outlook, Ollama) need to be set up separately.