# Agents Learning Hub

Interactive, visual learning resources for Microsoft's agent stack. Each topic is a single self-contained HTML page: no build step, no external requests, and light and dark themes. Open the pages straight from disk or through GitHub Pages.

**Live site:** https://testonprod.github.io/agents-learning-hub/

## Tracks

| Track | Start here | Status |
|---|---|---|
| Microsoft 365 Agents SDK | [`agents-sdk/index.html`](agents-sdk/index.html): the Atlas, covering every module and how it connects | Live |
| Agent Framework, Agent 365, Copilot Studio, Foundry | — | Planned |

### Microsoft 365 Agents SDK learning path

| # | Page | Status |
|---|---|---|
| 00 | [Atlas: every module and how they connect](agents-sdk/index.html) | Live |
| 01 | Nucleus: Activity Protocol & TurnContext | Planned |
| 02 | AgentApplication & routing | Planned |
| 03 | State, storage & memory design | Planned |
| 04 | Identity end to end | Planned |
| 05 | Bring your own brain (Semantic Kernel, Agent Framework) | Planned |
| 06 | Teams extension deep dive | Planned |
| 07 | Proactive & long-running work | Planned |
| 08 | Multi-agent (agent client, Copilot Studio, A2A) | Planned |
| 09 | Testing & telemetry | Planned |
| 10 | Ship to production | Planned |

## Repository layout

```
agents-learning-hub/
├── index.html              # landing page: tracks + learning path
├── README.md
├── .nojekyll               # serve files as-is on GitHub Pages
└── agents-sdk/             # one folder per track (kebab-case)
    ├── index.html          # 00 · track overview (the Atlas)
    ├── 01-nucleus.html     # deep dives: NN-topic-name.html
    └── …
```

## Conventions for new pages

- **One folder per track**, named in kebab-case (`agents-sdk`, `agent-framework`, …). The track overview is always `index.html`.
- **Deep dives** are named `NN-topic-name.html`, where `NN` is the order in the learning path (`01-nucleus.html`, `02-agentapplication-routing.html`).
- **Every page is self-contained**: CSS, JS and data inlined, no CDNs or web fonts, and it must open offline.
- **Link back** to the hub (`../index.html`) in the footer, and to the track overview from deep dives.
- **Register the page** in the `PAGES` list on the landing page and in the tables above, changing its status from *Planned* to *Live*.
- **Cite sources.** Every claim should trace back to Microsoft Learn or an official repository, with preview features labelled.

## Sources

Content is sourced from public [Microsoft Learn](https://learn.microsoft.com/microsoft-365/agents-sdk/) documentation and the official [microsoft/Agents](https://github.com/microsoft/Agents) repositories. This isn't an official Microsoft publication, so check the linked docs for the latest details.
