# SOP: Serving the Plumbing Landing Page Locally

## Overview
This document outlines the procedure for serving the static plumbing landing page on a local machine.

## Prerequisites
- Python 3.x installed.

## Execution Steps
1. Navigate to the project root.
2. Run the command:
   ```bash
   python3 -m http.server 8000 --directory "Plumbing project"
   ```
3. Access the site via your browser at `http://localhost:8000`.

## Edge Cases
- **Port Conflict:** If port 8000 is in use, specify a different port (e.g., 8080).
- **Directory Path:** Ensure the `--directory` flag points to the correct folder containing `index.html`.
