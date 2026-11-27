# Aran Shayan

**Product engineer. I build AI tools people can trust with real data: MCP servers, evals, and the interfaces around them.**

Six years in software, most of it on banking and enterprise platforms where a wrong number is worse than no number. I bring that habit to AI work: give the model only the access it needs, check its output with something that does not depend on trusting it, and measure quality before and after every change.

[Portfolio](https://aranshayan.com) · [Résumé (PDF)](https://aranshayan.com/aran-shayan-resume.pdf) · [LinkedIn](https://www.linkedin.com/in/aranshayan) · [X](https://x.com/aranshayan) · [hi@aranshayan.com](mailto:hi@aranshayan.com)

## Selected work

**[statement-extract](https://github.com/aranshayan/statement-extract)**: Claude reads a PDF bank statement, then plain arithmetic checks the result. The opening balance plus every amount has to equal the closing balance to the cent, every printed running balance has to match, and every date has to fall inside the period. If a check fails, Claude gets one retry with the exact errors; if that fails too, the output is marked failed with the reasons. Ships with an eval suite of 16 statements with ground truth, covering eight countries, page-break carry-overs, zero- and three-decimal currencies, lakh grouping and newest-first ordering.

**[pg-guard-mcp](https://github.com/aranshayan/pg-guard-mcp)**: an MCP server that gives agents read-only, audited, PII-masked access to PostgreSQL. It assumes the agent will eventually be asked to do something it should not, and the database stays safe when it is.

**[Tellerline](https://github.com/aranshayan/tellerline)**: accessible React components for banking and back-office apps, installed with the shadcn CLI. A money input that never rounds, an audit timeline in the reader's time zone, and a maker-checker approval flow whose rules also run on the server. Tested with axe. [Docs and demos](https://tellerline-ui.vercel.app)

**[cold-start-poi-recsys](https://github.com/aranshayan/cold-start-poi-recsys)**: MSc research on recommendations for new users. Prototypical networks vs MAML on Foursquare check-ins: +21.7% NDCG@10 and +26.3% Recall@10 over a graph neural network baseline, with the prototypical network training 3.5x faster than MAML at similar accuracy. [Article](https://aranshayan.com/writing/meta-learning-cold-start)

## Tools for Claude and other MCP clients

- [mcp-web-reader](https://github.com/aranshayan/mcp-web-reader): web pages as clean Markdown, with SSRF protection and robots.txt support
- [mcp-docs-reader](https://github.com/aranshayan/mcp-docs-reader): PDF, Word, Excel and CSV as LLM-friendly text
- [mcp-git-insights](https://github.com/aranshayan/mcp-git-insights): read-only Git history and code archaeology
- [agent-skills](https://github.com/aranshayan/agent-skills): Agent Skills for SQL review, PR review, commits and research
- [page-to-markdown](https://github.com/aranshayan/page-to-markdown): a browser extension that copies a page or selection as Markdown

## Before AI

- Led the frontend of an API integration platform for banks and telecom operators, including a no-code builder for connecting APIs.
- Built liquidity supervision and settlement reporting interfaces that run in production at a national bank.
- Found a SQL injection risk in the platform's database nodes and specified the fix across six database engines.
- Designed an authorization control plane and the tenancy services behind an ERP, from data model to OpenAPI contract.

That client work runs behind bank firewalls, so I rebuilt the hard parts as demos: a [million-row ledger](https://aranshayan.com/lab/grid), a [live payments monitor](https://aranshayan.com/lab/dashboard) and a [no-code API flow builder](https://aranshayan.com/lab/flow).

## Writing

- [Meta-learning for cold-start recommendations](https://aranshayan.com/writing/meta-learning-cold-start)
- [Hide the button, enforce on the server](https://aranshayan.com/writing/authorization-multi-tenant)
- [APIs a frontend can live with: designing the contract first](https://aranshayan.com/writing/contract-first-apis)
- [A million rows in the browser](https://aranshayan.com/writing/million-row-grid)

## Stack

TypeScript, React, Next.js, Node.js, Python, PyTorch, PostgreSQL. Claude API, Model Context Protocol, Agent Skills, Claude Code. Also Rust, Go, Kafka, Docker and Kubernetes.

**Looking for** a product or applied AI engineering role, remote.
