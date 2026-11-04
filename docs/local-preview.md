# Preview the static CataSoft site locally

This repository contains a static website snapshot, generated assets, and a small
Node.js server. It is distinct from the private editable React project.

## Start the preview

1. Install Node.js and open a terminal in this repository root.
2. Run `npm start`. No dependency installation is required by the current server.
3. Open `http://localhost:3000` and confirm the page and local images load.
4. Stop the server with Ctrl+C when finished.

To use a different port in PowerShell:

```powershell
$env:PORT = '8080'
npm start
```

Open `http://localhost:8080`. Remove the temporary variable afterwards with
`Remove-Item Env:PORT` if you no longer need it.

## Diagnose a preview problem

- Address in use: select another port and use that port in the browser.
- Unstyled page: check `_next/static/` is present and inspect the browser's failed requests.
- A missing asset returns HTML: the server falls back to `index.html` for unknown
  paths, so HTTP 200 alone does not establish that an asset exists.

The server serves files from the repository directory and has no authentication.
Use it for local preview; do not expose it as a production service. Changes to
compiled `_next` bundles are difficult to maintain; use the original source project
for application changes and regenerate the static output.

This guide is an AI-assisted documentation update. See [verification](verification.md)
for the executed local smoke check. It does not establish original authorship or asset rights.
