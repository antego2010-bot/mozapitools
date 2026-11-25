# Moz API Tools

Homepage for mozapitools.app. Each tool is its own Vercel project; this project serves the homepage and routes each path to its tool:

| Path | Tool | Project |
| --- | --- | --- |
| /page-grader/ | On-page grader for SEO and AI search | onpage-grader.vercel.app |
| /cannibalization-checker/ | Keyword cannibalization checker | cannibalization-checker.vercel.app |
| /internal-linking/ | Internal linking tool | internal-linking-tool-kappa.vercel.app |

Pages load through this domain (rewrites in `vercel.json`). API calls go straight to each tool's own project, which allows `https://mozapitools.app` via CORS, so long Claude requests aren't limited by the proxy timeout.
