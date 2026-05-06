[![Master Index](https://img.shields.io/badge/Master_Index-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/danielrosehill/Github-Master-Index)

# Israel Agent Skills — Dev Index

An index of repositories in the **Israel agent-skills ecosystem** maintained by Daniel Rosehill: the released plugins (destinations), the workspaces that feed into them, and adjacent / related indexes.

Trajectory for new skills:

> WIP workspace → exercised on real cases → verified → promoted into a plugin → workspace kept open for future iteration.

## Plugins (destinations)

Released Claude Code plugins. Stable, installable, public.

| Repo | Scope |
|---|---|
| [Claude-Israel-Agent-Skills-Plugin](https://github.com/danielrosehill/Claude-Israel-Agent-Skills-Plugin) | General-purpose Israel-specific agent skills for Claude Code and other agentic CLIs |
| [Claude-Israel-Shopping-Plugin](https://github.com/danielrosehill/Claude-Israel-Shopping-Plugin) | Israeli-resident shopping — domestic channels + overseas B2C (AliExpress, Amazon, iHerb), search-pattern mappings |

## Feeders (skills workspaces)

Where individual skills are drafted, exercised, and refined before promotion into a plugin.

| Repo | Stage | Description |
|---|---|---|
| [Israel-Medication-Research-Skills](https://github.com/danielrosehill/Israel-Medication-Research-Skills) | **integrated** | Patient-facing medication availability and access in Israel — kupot cholim formulary checks, `sal briyut` (health basket) status, generic equivalents, personal-import paths, pharmacy availability. Already folded into the main agent-skills plugin; workspace remains open for iteration. |
| [Israel-Property-Research-Skills](https://github.com/danielrosehill/Israel-Property-Research-Skills) | **WIP** | Israeli residential property due diligence — Tabu (`nesach tabu`, `nesach merukaz`), Israel Land Authority leasehold checks, building file (`tik binyan`) retrieval, `heter bniya` history, `shimush choreg` detection, TAMA 38 / `pinui-binui` status, preservation flags, comparable sales (nadlan / madlan / yad2), neighbourhood character. |
| [Israel-Mortgage-Research-Skills](https://github.com/danielrosehill/Israel-Mortgage-Research-Skills) | **WIP** | Israeli residential mortgages (משכנתא) — Bank of Israel track-composition rules, CPI-linked (Madad) and Prime stress testing, DSR / LTV ceilings, self-employed and foreign-currency income discounts, oleh and first-home benefits, `mas rechisha`, `ishur ekroni` workflow, bridging and refinance, bank-by-bank quirks. |
| [AliExpress-Israel-Skill](https://github.com/danielrosehill/AliExpress-Israel-Skill) | **WIP** | Planning notes for an AliExpress skill with an Israel-buyer focus — shipping, customs, VAT thresholds, payment quirks. Targeted to graduate into the Israel Shopping plugin. |

### Stage legend

| Stage | Meaning |
|---|---|
| `draft` | Sketched, not yet exercised on a real case |
| `WIP` | Actively being drafted / exercised; not in a plugin yet |
| `verified` | Used multiple times, output reviewed, edge cases mapped |
| `integrated` | Folded into a plugin; workspace open for future iteration |

## Related

Adjacent indexes and resource lists. Not skills repos themselves.

| Repo | Description |
|---|---|
| [Israeli-AI](https://github.com/danielrosehill/Israeli-AI) | Israel-specific agent skills, MCPs, and builders — broader index of the Israeli AI/agent landscape |
| [Israeli-Open-Source-Projects](https://github.com/danielrosehill/Israeli-Open-Source-Projects) | Curated index of open-source Israeli projects (data, civic tech, finance, careers, real estate, smart home, media) |
| [Israel-Projects-Index](https://github.com/danielrosehill/Israel-Projects-Index) | Master index of all Israel-related repositories |
| [Israel-Open-Data-Resources](https://github.com/danielrosehill/Israel-Open-Data-Resources) | Open-access data and a list of Israeli data projects |

## Naming

Train-Case for repos and folders. Skill slugs inside `skills/` directories use kebab-case to match Claude Code slash-command conventions.
