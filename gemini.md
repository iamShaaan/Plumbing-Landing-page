# Data Schema: GitHub Repository Deployment

```json
{
  "repository": {
    "name": "Plumbing Landing page",
    "owner": "iamShaaan",
    "visibility": "public",
    "description": "Premium landing page for plumbing services.",
    "remote_url": "https://github.com/iamShaaan/Plumbing-Landing-page.git",
    "files_included": "All source + project metadata",
    "branch": "main"
  },
  "deployment_trigger": "manual_push"
}
```

# Data Schema: Booking Webhook Payload

```json
{
  "name": "string",
  "phone": "string",
  "service": "string",
  "message": "string",
  "timestamp": "ISO-8601 string",
  "metadata": {
    "source": "landing-page",
    "version": "1.0.0"
  }
}
```

# Maintenance Log

## 2026-04-10: Initial Export
- **Event:** Successfully created and populated the project's new GitHub repository.
- **Action:** Created `iamShaaan/Plumbing-Landing-page`, linked local repository via a temporary PAT-authenticated remote, and pushed all files including planning metadata.
- **Status:** Complete and Verified.

## 2026-04-10: Webhook Update
- **Event:** Update booking form to send data to n8n webhook.
- **Action:** Update `script.js` to use `fetch` with the new n8n URL.
- **Status:** Complete and Verified.
