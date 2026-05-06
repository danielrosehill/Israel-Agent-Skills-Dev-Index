[![Master Index](https://img.shields.io/badge/Master_Index-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/danielrosehill/Github-Master-Index)

# Israel Agent Skills — Dev Index

An index of **work-in-progress skills baskets** developed by Daniel Rosehill that feed into the [Israel-Agent-Skills-Dev](https://github.com/danielrosehill/Israel-Agent-Skills-Dev) plugin (and its public counterpart, [Claude-Israel-Agent-Skills-Plugin](https://github.com/danielrosehill/Claude-Israel-Agent-Skills-Plugin)).

Each repo listed below is a thematic basket of skills under active development. Skills graduate out of these repos into the canonical plugin once they have been **exercised, refined, and verified** against real cases.

## Status convention

Within each basket repo, skills are tagged:

| Tag | Meaning |
|---|---|
| `draft` | Sketched, not yet exercised |
| `exercised` | Used on a real case at least once |
| `verified` | Used multiple times, output reviewed, edge cases mapped |
| `promoted` | Folded into Israel-Agent-Skills-Dev (PR linked) |

## Skills baskets

### Israel Property Research Skills
WIP skills basket for Israeli residential property due diligence — Tabu (`nesach tabu`, `nesach merukaz`), Israel Land Authority leasehold checks, building-file (`tik binyan`) retrieval, `heter bniya` history, `shimush choreg` (unauthorised use) detection, TAMA 38 / `pinui-binui` status, preservation/heritage flags, comparable sales (nadlan/madlan/yad2), neighbourhood character.

[![Repo](https://img.shields.io/badge/Repo-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/danielrosehill/Israel-Property-Research-Skills)

---

### Israel Mortgage Research Skills
WIP skills basket for Israeli residential mortgages (משכנתא) — Bank of Israel track-composition rules (Prime ≤ 1/3, variable ≤ 2/3, fixed ≥ 1/3), CPI-linked (Madad) stress testing, Prime-rate stress, DSR / LTV ceilings, self-employed and foreign-currency income discounts, oleh and first-home benefits, `mas rechisha` brackets, `ishur ekroni` workflow, bridging loans, refinance (`michzur`), and bank-by-bank quirks.

[![Repo](https://img.shields.io/badge/Repo-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/danielrosehill/Israel-Mortgage-Research-Skills)

---

### Israel Medication Research Skills
WIP skills basket for medication availability and access in Israel — patient-facing (non-professional) lookups, kupot cholim formulary checks, `sal briyut` (health basket) status, generic equivalents, import/personal-import paths, pharmacy availability.

[![Repo](https://img.shields.io/badge/Repo-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/danielrosehill/Israel-Medication-Research-Skills)

---

## Destination plugins

| Plugin | Visibility | Purpose |
|---|---|---|
| [Israel-Agent-Skills-Dev](https://github.com/danielrosehill/Israel-Agent-Skills-Dev) | private | Development / staging plugin where verified skills land first |
| [Claude-Israel-Agent-Skills-Plugin](https://github.com/danielrosehill/Claude-Israel-Agent-Skills-Plugin) | public | Public release of the Israel-specific Claude Code plugin |

## Related indexes

- [Israel Projects Index](https://github.com/danielrosehill/Israel-Projects-Index) — the broader index of all Israel-related repos (apps, datasets, dashboards, this index, etc.)

## Naming

Train-Case for repos and folders. Skill slugs inside `skills/` directories use kebab-case to match Claude Code slash-command conventions.
