# Data Schema: GitHub Repository Deployment

```json
{
  "repository": {
    "name": "Plumbing Landing page",
    "owner": "soumitrohalder",
    "visibility": "public",
    "description": "Premium landing page for plumbing services.",
    "files_to_include": [
      "Plumbing project/",
      "architecture/",
      "claude.md",
      "task_plan.md",
      "findings.md",
      "progress.md",
      "gemini.md"
    ],
    "files_to_exclude": [
      ".tmp/",
      "node_modules/"
    ]
  },
  "deployment_trigger": "manual_push"
}
```
