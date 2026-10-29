<div align="center">

# Awesome QuickBooks AI

**A curated list of AI tooling for QuickBooks Desktop, QuickBooks Online and QuickBooks Time:** agent skills, MCP servers, CLIs, starter kits, building blocks and services.

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)
[![License: CC0-1.0](https://img.shields.io/badge/license-CC0--1.0-lightgrey.svg?style=flat-square)](LICENSE)

</div>

---

Entries are grouped by **what kind of thing a tool is**, then by QuickBooks product, so you can go straight to what
you need: skills for your agent, an MCP server for your books, a library to build on, or a service that runs it for
you.

Every description here comes from the project's own repository or site. Star counts are live badges. Links were
checked on 20 and 21 October 2026.

## Legend

| | Meaning |
|---|---|
| 🎓 | Agent skills and plugins (Claude Code, Codex, Cursor…) |
| 🔌 | MCP server |
| 🖥 | CLI or standalone tool |
| 📦 | Starter kit or reference build |
| 🧩 | AI app or agent that does a bookkeeping job |
| 🧱 | SDK or library |
| ☁️ | Hosted or commercial product, or open-source code that needs one |
| 🧭 | Not QuickBooks-specific, but useful in a QuickBooks workflow |

## Contents

- [🎓 Agent Skills & Plugins](#-agent-skills--plugins)
- [🔌 MCP Servers](#-mcp-servers)
- [🧩 AI on the Books](#-ai-on-the-books)
- [🖥 CLIs](#-clis)
- [📦 Starter Kits & Reference Builds](#-starter-kits--reference-builds)
- [🧱 Building Blocks](#-building-blocks)
- [☁️ Hosted & Commercial](#️-hosted--commercial)
- [📚 Reading & Resources](#-reading--resources)
- [Contributing](#contributing)
- [License](#license)

---

## 🎓 Agent Skills & Plugins

Skills and plugins that teach an agent how to work with the books. They need a QuickBooks connection, such as an MCP
server below.

- **[quickbooks-claude-plugin](https://github.com/intuit/quickbooks-claude-plugin)** ![stars](https://img.shields.io/github/stars/intuit/quickbooks-claude-plugin?style=flat-square&label=&color=555) — Intuit's skills that turn QuickBooks Online data into plain-language business insights in Claude; needs the QuickBooks connector.
- **[quickbooks-month-end-close](https://github.com/fengyiqicoder/quickbooks-month-end-close)** ![stars](https://img.shields.io/github/stars/fengyiqicoder/quickbooks-month-end-close?style=flat-square&label=&color=555) — GAAP-aware month-end close walkthrough for QuickBooks, as an agent skill for Claude, Cursor and Codex.
- **[skill-finance-accounting](https://github.com/zavora-ai/skill-finance-accounting)** ![stars](https://img.shields.io/github/stars/zavora-ai/skill-finance-accounting?style=flat-square&label=&color=555) — Revenue operations skill for AI agents: invoicing, collections, reconciliation and financial reporting through mcp-finance, for QuickBooks or Xero.
- **[zeno-quickbooks-desktop](https://github.com/Zeno-Services/zeno-quickbooks-desktop)** ![stars](https://img.shields.io/github/stars/Zeno-Services/zeno-quickbooks-desktop?style=flat-square&label=&color=555) ☁️ — Zeno for QuickBooks Desktop: workflow skills for Claude, ChatGPT and Codex, and the MCP bundle releases, for Zeno's separately installed program.
- See also **[Agent Kit for QuickBooks Desktop](https://github.com/ph4mHoa/qbd-agent-kit)**: a Claude Code plugin with nine QuickBooks Desktop skills (daily brief, collections, bills and cash, month-end check, reorder, picking a report, entering a bill from a document, support cases) on top of its [command line](#-clis).

### 🧭 Adjacent & general-purpose

- **[bookkeeping-skills](https://github.com/Receiptor-AI/bookkeeping-skills)** ![stars](https://img.shields.io/github/stars/Receiptor-AI/bookkeeping-skills?style=flat-square&label=&color=555) — Open-source bookkeeping skills for AI agents.
- **[financial-services](https://github.com/anthropics/financial-services)** ![stars](https://img.shields.io/github/stars/anthropics/financial-services?style=flat-square&label=&color=555) — Anthropic's reference agents, skills and data connectors for financial services, among them a GL Reconciler and a Month-End Closer that draft work for review by a qualified professional.
- **[skills (hazlijohar95)](https://github.com/hazlijohar95/skills)** ![stars](https://img.shields.io/github/stars/hazlijohar95/skills?style=flat-square&label=&color=555) — Skills for better accountants: agent skills for closing real books, not vibe bookkeeping.

## 🔌 MCP Servers

### QuickBooks Desktop

- **[qbbridge](https://github.com/lilfroog/qbbridge)** ![stars](https://img.shields.io/github/stars/lilfroog/qbbridge?style=flat-square&label=&color=555) — An MCP frontend for QuickBooks Desktop: read, write and safely undo transactions via QBXML/QBFC from any MCP client.
- **[quickbooks-desktop-mcp](https://github.com/DesktopAccountingAPI/quickbooks-desktop-mcp)** ![stars](https://img.shields.io/github/stars/DesktopAccountingAPI/quickbooks-desktop-mcp?style=flat-square&label=&color=555) ☁️ — MCP server for QuickBooks Desktop by Desktop Accounting API, a hosted service, for Claude, Cursor, VS Code, Codex and other AI tools.
- **[quickbooks-mcp (devwithmj)](https://github.com/devwithmj/quickbooks-mcp)** ![stars](https://img.shields.io/github/stars/devwithmj/quickbooks-mcp?style=flat-square&label=&color=555) — Open-source MCP server connecting QuickBooks Desktop (Pro, Premier, Enterprise) to LLMs and agents, read-only by default, with previews and confirmation tokens for writes.
- **[Quickbooks-MCP-Desktop](https://github.com/RealDealCPA-VR/Quickbooks-MCP-Desktop)** ![stars](https://img.shields.io/github/stars/RealDealCPA-VR/Quickbooks-MCP-Desktop?style=flat-square&label=&color=555) — Safe, supervised hands on QuickBooks Desktop for AI agents: 154 tools across the whole ledger, multi-company switching, a live control page, remote agents over Tailscale and a simulation mode on any OS (no licence file).

### QuickBooks Online

> **Intuit** publishes the official QuickBooks Online MCP server; several entries below build on it.

- **[better-quickbooks-Claude-connector](https://github.com/IsaacCP9/better-quickbooks-Claude-connector)** ![stars](https://img.shields.io/github/stars/IsaacCP9/better-quickbooks-Claude-connector?style=flat-square&label=&color=555) — MCP server connecting Claude to QuickBooks Online with 54 tools and many companies from one connector, plus a setup guide for non-technical users.
- **[hermes-quickbooks](https://github.com/mindtrip101/hermes-quickbooks)** ![stars](https://img.shields.io/github/stars/mindtrip101/hermes-quickbooks?style=flat-square&label=&color=555) — Connector that gives the Hermes agent typed QuickBooks Online tools, with OAuth 2.0 and approval-gated writes.
- **[laravel-quickbooks-mcp-server](https://github.com/rajurayhan/laravel-quickbooks-mcp-server)** ![stars](https://img.shields.io/github/stars/rajurayhan/laravel-quickbooks-mcp-server?style=flat-square&label=&color=555) — PHP/Laravel Composer package that exposes QuickBooks Online as an MCP server over HTTP, mirroring Intuit's official server.
- **[ledger-mcp](https://github.com/Tight-Line/ledger-mcp)** ![stars](https://img.shields.io/github/stars/Tight-Line/ledger-mcp?style=flat-square&label=&color=555) — Intuit's QuickBooks Online MCP server, served remotely with OAuth sign-in and an email allowlist.
- **[mcp-quickbooks (amin-ale)](https://github.com/amin-ale/mcp-quickbooks)** ![stars](https://img.shields.io/github/stars/amin-ale/mcp-quickbooks?style=flat-square&label=&color=555) — QuickBooks Online MCP server with 18 tools over invoices, customers and payments, OAuth 2.1 with PKCE, and stdio or streamable HTTP.
- **[mcp-quickbooks (pipeworx-io)](https://github.com/pipeworx-io/mcp-quickbooks)** ![stars](https://img.shields.io/github/stars/pipeworx-io/mcp-quickbooks?style=flat-square&label=&color=555) — QuickBooks MCP pack to query customers, invoices and accounts, part of the Pipeworx MCP gateway.
- **[qbo-mcp (alveyautomation)](https://github.com/alveyautomation/qbo-mcp)** ![stars](https://img.shields.io/github/stars/alveyautomation/qbo-mcp?style=flat-square&label=&color=555) — Read-only QuickBooks Online MCP server with OAuth refresh-token rotation, retries and query-string escaping.
- **[qbo-mcp (matpb)](https://github.com/matpb/qbo-mcp)** ![stars](https://img.shields.io/github/stars/matpb/qbo-mcp?style=flat-square&label=&color=555) — Local-first QuickBooks Online MCP server that ships as a one-click Claude Desktop extension (`.mcpb`).
- **[qbo-mcp (SrishtiKalpa)](https://github.com/SrishtiKalpa/qbo-mcp)** ![stars](https://img.shields.io/github/stars/SrishtiKalpa/qbo-mcp?style=flat-square&label=&color=555) — QuickBooks Online MCP server for invoices, reports and books, with a human-in-the-loop draft and confirm step for writes.
- **[qbo-mcp (WYRE-AI)](https://github.com/WYRE-AI/qbo-mcp)** ![stars](https://img.shields.io/github/stars/WYRE-AI/qbo-mcp?style=flat-square&label=&color=555) — QuickBooks Online MCP server for customers, invoices, expenses, payments and reports, with an interactive invoice card for MCP Apps hosts.
- **[qbo-mcp (YanivErel-code)](https://github.com/YanivErel-code/qbo-mcp)** ![stars](https://img.shields.io/github/stars/YanivErel-code/qbo-mcp?style=flat-square&label=&color=555) — Self-hostable, read-only QuickBooks Online MCP server with encrypted tokens, deployed through Cloudflare Tunnel.
- **[qbo-mcp-proxy](https://github.com/marcusadolfsson/qbo-mcp-proxy)** ![stars](https://img.shields.io/github/stars/marcusadolfsson/qbo-mcp-proxy?style=flat-square&label=&color=555) — Serves QuickBooks Online to Claude and other MCP clients from your Mac's menu bar, for many companies and many clients.
- **[qbo-mcp-server](https://github.com/Kaizen-CFO/qbo-mcp-server)** ![stars](https://img.shields.io/github/stars/Kaizen-CFO/qbo-mcp-server?style=flat-square&label=&color=555) ☁️ — MCP server that connects Claude Code, Cursor and other AI tools to QuickBooks Online through the Kaizen API.
- **[quickbooks-mcp (laf-rge)](https://github.com/laf-rge/quickbooks-mcp)** ![stars](https://img.shields.io/github/stars/laf-rge/quickbooks-mcp?style=flat-square&label=&color=555) — QuickBooks Online MCP server for bookkeepers, CFOs and accountants to query, create and edit accounting data in plain language.
- **[quickbooks-mcp (nichewizard)](https://github.com/nichewizard/quickbooks-mcp)** ![stars](https://img.shields.io/github/stars/nichewizard/quickbooks-mcp?style=flat-square&label=&color=555) — QuickBooks Online MCP server where every create, update and delete waits for human approval, and QuickBooks text is treated as untrusted input.
- **[quickbooks-mcp-cloudflare](https://github.com/TimothyKrell/quickbooks-mcp-cloudflare)** ![stars](https://img.shields.io/github/stars/TimothyKrell/quickbooks-mcp-cloudflare?style=flat-square&label=&color=555) — Remote QuickBooks Online MCP server you deploy to your own Cloudflare account, rewritten from Intuit's server in Effect.
- **[quickbooks-mcp-server (kousie20)](https://github.com/kousie20/quickbooks-mcp-server)** ![stars](https://img.shields.io/github/stars/kousie20/quickbooks-mcp-server?style=flat-square&label=&color=555) — Local-first MCP server that connects Claude Desktop to QuickBooks Online, with 40 tools for reports, invoicing, expenses and bookkeeping.
- **[quickbooks-mcp-server (rjpaganini)](https://github.com/rjpaganini/quickbooks-mcp-server)** ![stars](https://img.shields.io/github/stars/rjpaganini/quickbooks-mcp-server?style=flat-square&label=&color=555) — Single-file MCP server giving Claude read and write access to QuickBooks Online, plus reconciliation tools that find bank-feed gaps and duplicates.
- **[quickbooks-online-mcp](https://github.com/LibreChat-AI/quickbooks-online-mcp)** ![stars](https://img.shields.io/github/stars/LibreChat-AI/quickbooks-online-mcp?style=flat-square&label=&color=555) — QuickBooks Online MCP server rebuilt on Cloudflare Workers with OAuth 2.0 and Streamable HTTP/SSE, drop-in compatible with LibreChat.
- **[quickbooks-online-mcp-server](https://github.com/intuit/quickbooks-online-mcp-server)** ![stars](https://img.shields.io/github/stars/intuit/quickbooks-online-mcp-server?style=flat-square&label=&color=555) — Intuit's official MCP server that exposes QuickBooks Online features as tools for AI assistants.

### QuickBooks Time

- **[qb-time-mcp-server](https://github.com/aallsbury/qb-time-mcp-server)** ![stars](https://img.shields.io/github/stars/aallsbury/qb-time-mcp-server?style=flat-square&label=&color=555) — MCP server that combines the QuickBooks Time job code, report, timesheet and user tools in one interface.

## 🧩 AI on the Books

Apps and agents that do one bookkeeping job with AI, grouped by the job. Most are young projects: try them on a copy
of the books first.

### Bank statements & categorizing

- **[invoice-ai-to-accounting](https://github.com/alejandrofernandezurbano/invoice-ai-to-accounting)** ![stars](https://img.shields.io/github/stars/alejandrofernandezurbano/invoice-ai-to-accounting?style=flat-square&label=&color=555) — Demo pipeline that reads bank statement PDFs (OCR, then rules or an LLM), works out who paid whom and for which invoice, validates the result and posts it to QuickBooks, sending only doubtful lines to a person.
- **[recat-qbo](https://github.com/tx-joshg/recat-qbo)** ![stars](https://img.shields.io/github/stars/tx-joshg/recat-qbo?style=flat-square&label=&color=555) — Self-hosted transaction categorization and review queue for QuickBooks Online, an open-source alternative to Uncat.

### Bills & payables

- **[gmail-quickbooks-invoice-automation](https://github.com/Sahib1231241242123/gmail-quickbooks-invoice-automation)** ![stars](https://img.shields.io/github/stars/Sahib1231241242123/gmail-quickbooks-invoice-automation?style=flat-square&label=&color=555) — Reads vendor invoices from Gmail with AI and imports them into QuickBooks Desktop Enterprise as bills, through the SDK or an IIF file.

### Collections

- **[ar-collections-agent](https://github.com/withoneai/ar-collections-agent)** ![stars](https://img.shields.io/github/stars/withoneai/ar-collections-agent?style=flat-square&label=&color=555) ☁️ — AI accounts-receivable pipeline: finds overdue QuickBooks invoices, has Claude write the chase email per your collections policy, and leaves drafts with the invoice PDFs in Gmail; built on One.

### Reporting

- **[autoconst-claude-construction-cfo](https://github.com/hamzaabduljabbar/autoconst-claude-construction-cfo)** ![stars](https://img.shields.io/github/stars/hamzaabduljabbar/autoconst-claude-construction-cfo?style=flat-square&label=&color=555) — Construction-CFO pipeline from a QuickBooks export to a reconciled Excel management pack (job cost, retention, cash flow, expense audit): Python does the math, and the LLM only classifies uncoded lines.

For QuickBooks Desktop, the [Agent Kit](#-clis) below does several of these jobs (collections, payment matching,
deposits, bills, month-end checks) from the command line.

## 🖥 CLIs

- **[Agent Kit for QuickBooks Desktop](https://github.com/ph4mHoa/qbd-agent-kit)** ![stars](https://img.shields.io/github/stars/ph4mHoa/qbd-agent-kit?style=flat-square&label=&color=555) — Command line made for AI agents on the Windows PC that runs QuickBooks Desktop: one line of JSON per command, workflows (daily brief, collections and payment matching, deposits, payables, cash, reorder, stock, purchasing with a three-way match, 1099, month-end check), any record or report, CSV import and export, and changes saved only after you approve them, with undo.
- **[ai-cfo-quickbooks](https://github.com/CharlesPSG/ai-cfo-quickbooks)** ![stars](https://img.shields.io/github/stars/CharlesPSG/ai-cfo-quickbooks?style=flat-square&label=&color=555) — Pull any client's financials from QuickBooks Online through Claude: a multi-client CLI and Claude skill for accounting firms.
- **[quickbooks-cli (osodevops)](https://github.com/osodevops/quickbooks-cli)** ![stars](https://img.shields.io/github/stars/osodevops/quickbooks-cli?style=flat-square&label=&color=555) — CLI for the QuickBooks Online API with OAuth2 PKCE sign-in, 36 entities, 25+ reports, SQLite caching and table, JSON, CSV or YAML output.
- **[quickbooks-cli (Robben-Media)](https://github.com/Robben-Media/quickbooks-cli)** ![stars](https://img.shields.io/github/stars/Robben-Media/quickbooks-cli?style=flat-square&label=&color=555) — Go CLI for QuickBooks Online: invoices, bills, payments, journal entries, customers, vendors, items and reports.
- **[quickbooks-desktop-bridge](https://github.com/SC-SoftwareHS/quickbooks-desktop-bridge)** ![stars](https://img.shields.io/github/stars/SC-SoftwareHS/quickbooks-desktop-bridge?style=flat-square&label=&color=555) — Bridges QuickBooks Desktop to other machines on your network with a 32-bit COM bridge, token-authed HTTP API, CLI and bank-import pipeline, read-only by default.

## 📦 Starter Kits & Reference Builds

- **[ai-invoice-quickbooks-agent](https://github.com/Zenith10-fck/ai-invoice-quickbooks-agent)** ![stars](https://img.shields.io/github/stars/Zenith10-fck/ai-invoice-quickbooks-agent?style=flat-square&label=&color=555) — Supplier invoice intake with n8n and Claude, where every number is checked against the PDF before it reaches QuickBooks Online.
- **[QBXML_SDK_Samples](https://github.com/IntuitDeveloper/QBXML_SDK_Samples)** ![stars](https://img.shields.io/github/stars/IntuitDeveloper/QBXML_SDK_Samples?style=flat-square&label=&color=555) — Intuit's sample applications and code for the QuickBooks Desktop SDK, with qbXML and QBFC samples.

## 🧱 Building Blocks

Libraries and SDKs for building your own QuickBooks tools.

### QuickBooks Desktop

- **[pyqwc](https://github.com/BillBarry/pyqwc)** ![stars](https://img.shields.io/github/stars/BillBarry/pyqwc?style=flat-square&label=&color=555) — Python server that uses QuickBooks Web Connector to access QuickBooks Desktop.
- **[qbwc](https://github.com/qbwc/qbwc)** ![stars](https://img.shields.io/github/stars/qbwc/qbwc?style=flat-square&label=&color=555) — A Rails interface for Intuit's QuickBooks Web Connector.
- **[qbxml](https://github.com/qbwc/qbxml)** ![stars](https://img.shields.io/github/stars/qbwc/qbxml?style=flat-square&label=&color=555) — QBXML parser and validation tool for Ruby.
- **[QBXML-Object-Models](https://github.com/sflagp/QBXML-Object-Models)** ![stars](https://img.shields.io/github/stars/sflagp/QBXML-Object-Models?style=flat-square&label=&color=555) — C# object models that generate qbXML for QuickBooks Desktop and Online editions.
- **[quickbooks-desktop-node](https://github.com/conductor-is/quickbooks-desktop-node)** ![stars](https://img.shields.io/github/stars/conductor-is/quickbooks-desktop-node?style=flat-square&label=&color=555) ☁️ — QuickBooks Desktop API for Node.js (TypeScript or JavaScript), a client for Conductor's hosted service.
- **[quickbooks-desktop-python (Conductor)](https://github.com/conductor-is/quickbooks-desktop-python)** ![stars](https://img.shields.io/github/stars/conductor-is/quickbooks-desktop-python?style=flat-square&label=&color=555) ☁️ — QuickBooks Desktop API for Python, a client for Conductor's hosted service.
- **[quickbooks-desktop-python (Donny-GUI)](https://github.com/Donny-GUI/quickbooks-desktop-python)** ![stars](https://img.shields.io/github/stars/Donny-GUI/quickbooks-desktop-python?style=flat-square&label=&color=555) — Python module for integrating with QuickBooks Desktop through the SDK: connecting, sending and receiving qbXML, and managing sessions.
- **[quickbooks-php](https://github.com/consolibyte/quickbooks-php)** ![stars](https://img.shields.io/github/stars/consolibyte/quickbooks-php?style=flat-square&label=&color=555) — QuickBooks integration for PHP, connecting Windows versions of QuickBooks and QuickBooks Online to PHP applications.
- **[quickbooks-sync](https://github.com/jsgoupil/quickbooks-sync)** ![stars](https://img.shields.io/github/stars/jsgoupil/quickbooks-sync?style=flat-square&label=&color=555) — NuGet packages to sync data from QuickBooks Desktop using qbXML.
- **[Zombie](https://github.com/pkpjpm/Zombie)** ![stars](https://img.shields.io/github/stars/pkpjpm/Zombie?style=flat-square&label=&color=555) — C# utility library for the QuickBooks SDK and QBFC.

### QuickBooks Online

> **Intuit** publishes official SDKs for the QuickBooks Online API.

- **[node-quickbooks](https://github.com/mcohen01/node-quickbooks)** ![stars](https://img.shields.io/github/stars/mcohen01/node-quickbooks?style=flat-square&label=&color=555) — Node.js client for Intuit's QuickBooks API.
- **[oauth-jsclient](https://github.com/intuit/oauth-jsclient)** ![stars](https://img.shields.io/github/stars/intuit/oauth-jsclient?style=flat-square&label=&color=555) — Intuit's Node.js client for OAuth 2.0 and OpenID Connect.
- **[python-quickbooks](https://github.com/routablehq/python-quickbooks)** ![stars](https://img.shields.io/github/stars/routablehq/python-quickbooks?style=flat-square&label=&color=555) — Python library for accessing the QuickBooks API.
- **[QuickBooks-V3-DotNET-SDK](https://github.com/intuit/QuickBooks-V3-DotNET-SDK)** ![stars](https://img.shields.io/github/stars/intuit/QuickBooks-V3-DotNET-SDK?style=flat-square&label=&color=555) — Intuit's .NET SDK for the QuickBooks REST API v3.
- **[QuickBooks-V3-Java-SDK](https://github.com/intuit/QuickBooks-V3-Java-SDK)** ![stars](https://img.shields.io/github/stars/intuit/QuickBooks-V3-Java-SDK?style=flat-square&label=&color=555) — Intuit's Java SDK for the QuickBooks REST API v3.
- **[QuickBooks-V3-PHP-SDK](https://github.com/intuit/QuickBooks-V3-PHP-SDK)** ![stars](https://img.shields.io/github/stars/intuit/QuickBooks-V3-PHP-SDK?style=flat-square&label=&color=555) — Intuit's official PHP SDK for the QuickBooks REST API v3.

### For coding agents

- **[LL-G](https://github.com/BoardPandas/LL-G)** ![stars](https://img.shields.io/github/stars/BoardPandas/LL-G?style=flat-square&label=&color=555) — Lessons learned and gotchas from many repositories, with a QuickBooks Online `llms.txt` and notes on OAuth traps in `kb/quickbooks`.

## ☁️ Hosted & Commercial

### QuickBooks Desktop

- **[Activepieces: QuickBooks Desktop (via Conductor)](https://www.activepieces.com/mcp/quickbooks-desktop-conductor)** — QuickBooks Desktop tools for Claude, Cursor and any MCP client through Conductor, in an open-source server that also reaches other apps.
- **[Apideck](https://www.apideck.com/integrations/quickbooks-desktop)** — Unified accounting API with a QuickBooks Desktop integration and a hosted MCP server.
- **[CData MCP Server for QuickBooks](https://github.com/CDataSoftware/quickbooks-mcp-server-by-cdata)** ![stars](https://img.shields.io/github/stars/CDataSoftware/quickbooks-mcp-server-by-cdata?style=flat-square&label=&color=555) — Read-only MCP server that queries live QuickBooks data through CData's JDBC driver, which is sold separately.
- **[Clockwork](https://www.clockwork.ai/)** — AI FP&A software built by a CFO: its AI builds the financial model and cash-flow forecasts from QuickBooks Online or QuickBooks Desktop, and Mira, its AI analyst, answers questions in plain English.
- **[Codat](https://docs.codat.io/integrations/accounting/quickbooksdesktop/accounting-quickbooksdesktop/)** — Accounting data API; its QuickBooks Desktop connector shares a company's consented data through the Intuit Web Connector, from the desktop app, QuickBooks Enterprise Cloud or Rightworks.
- **[Conductor](https://conductor.is)** — Real-time API for QuickBooks Desktop and Enterprise, with an [MCP server](https://docs.conductor.is/usage/mcp) for Claude, Cursor and Codex.
- **[Desktop Accounting API](https://www.desktopaccountingapi.com)** — A modern REST API for QuickBooks Desktop and Enterprise, with the MCP server listed above.
- **[Kipper](https://kipper.com/quickbooks-mcp-connector/)** — Hosted, read-only, audit-logged MCP connector for Claude, ChatGPT and Gemini; QuickBooks Desktop company files are an add-on.
- **[Rutter](https://www.rutter.com/integrations/quickbooks-desktop)** — Unified accounting API that syncs financial reports, bills, invoices, expenses and more from QuickBooks Desktop.
- **[Sage Expense Management (formerly Fyle)](https://www.fylehq.com/product/integrations/quickbooks-desktop-accounting-software)** — Expense management that exports employee expenses to QuickBooks Desktop as bills, journal entries or credit card transactions, with AI-based expense coding.
- **[Stampli](https://www.stampli.com/erp/quickbooks-desktop/)** — Procure-to-pay in the cloud (purchasing, approvals, payments) with QuickBooks Desktop kept as the system of record, through Stampli Bridge installed beside QuickBooks; Billy, its AI, does the busywork.

### QuickBooks Online

- **[Booke AI](https://booke.ai/)** — AI bookkeeper that categorizes QuickBooks Online bank feed transactions every day and matches them to invoices, bills and receipts; it also reconciles in Xero.
- **[Chaser](https://www.chaserhq.com/integrations/quickbooks-online)** — Credit control software that syncs QuickBooks Online invoices and chases payment by email, SMS and phone, with an AI email generator and AI debtor risk insights.
- **[Composio](https://composio.dev/toolkits/quickbooks)** — Hosted QuickBooks MCP for Claude, Cursor and ChatGPT, with managed OAuth.
- **[Coupler.io](https://www.coupler.io/mcp/quickbooks)** — QuickBooks Online MCP server for analyzing profit and loss, cash flow, invoices, bills and receivables with AI.
- **[Double](https://doublehq.com/)** — Month-end close management for accounting firms and finance teams on QuickBooks Online, Xero, Sage or NetSuite, with AI bank feeds, AI transactions and Ask Double.
- **[n8n](https://n8n.io/integrations/quickbooks-online/)** — Workflow automation with a QuickBooks Online integration and ready-made workflows, such as emailed invoices read with OCR and GPT-4 into QuickBooks.
- **[Pipedream](https://mcp.pipedream.com/app/quickbooks)** — MCP server that connects your QuickBooks account to Cursor, Claude and Windsurf.
- **[Zapier](https://zapier.com/mcp/quickbooks)** — Zapier MCP for QuickBooks Online.

## 📚 Reading & Resources

- **[Accounting AI Benchmark 2026](https://www.dualentry.com/benchmark)** — DualEntry, which sells AI accounting software, tested leading AI models on 101 synthetic tasks in eight areas of accounting, from transaction classification and journal entries to reconciliation, financial reporting and month-end close.
- **[Agent Skills](https://agentskills.io)** — The open format the agent skills above are written in.
- **[AI agents for QuickBooks: real use cases and guides](https://agentsfinance.io/erps/quickbooks/)** — Agents Finance, a free directory, collects documented cases of AI and agents with QuickBooks, such as reconciling the bank feed and payment-processor payouts, and multi-entity close and consolidation, each with its source.
- **[Compared with other options](https://github.com/ph4mHoa/qbd-agent-kit/blob/main/docs/comparison.md)** — Ways to connect an AI agent to QuickBooks Desktop, compared on where data goes, listed price and write safety.
- **[Model Context Protocol](https://modelcontextprotocol.io)** — The open protocol MCP servers speak.
- **[QuickBooks Desktop SDK](https://developer.intuit.com/app/developer/qbdesktop/docs/get-started)** — Intuit's documentation for building on QuickBooks Desktop.
- **[QuickBooks Desktop API reference](https://developer.intuit.com/app/developer/qbdesktop/docs/api-reference/qbdesktop)** — Intuit's reference for every qbXML request and response.
- **[QuickBooks MCP server: setup and 42 operations](https://www.codewords.ai/blog/quickbooks-mcp)** — CodeWords on connecting QuickBooks Online to AI assistants such as Claude, operation by operation.
- **[QuickBooks MCP Servers Compared: All 7 Options (2026)](https://kipper.com/blog/quickbooks-mcp-server-options-compared/)** — Kipper, a vendor listed above, compares Intuit's server, community builds, Zapier, CData, DeepLedger and Kipper on setup, write access, permissions and cost.
- **[QuickBooks Online AI tools](https://developer.intuit.com/app/developer/qbo/docs/develop/ai-tools)** — Intuit's developer page on AI tools for QuickBooks Online.

## Contributing

Found something missing? Pull requests and issues are welcome; see [CONTRIBUTING.md](CONTRIBUTING.md) for the entry
format and what gets in.

## License

[CC0-1.0](LICENSE). To the extent possible under law, contributions to this list are released into the public
domain. Linked projects keep their own licenses. QuickBooks is a trademark of Intuit Inc.; this list is not
affiliated with or endorsed by Intuit.
