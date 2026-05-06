[![Master Index](https://img.shields.io/badge/Master_Index-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/danielrosehill/Github-Master-Index)

# Israel Agent Skills — Dev Index

An index of repositories in the **Israel agent-skills ecosystem** maintained by Daniel Rosehill: the released plugins (destinations), the workspaces that feed into them, and adjacent / related indexes.

Trajectory for new skills:

> WIP workspace → exercised on real cases → added to a plugin → workspace kept open for future iteration.

## Plugins (destinations)

Released Claude Code plugins. Stable, installable, public.

| Repo | Scope |
|---|---|
| [Israel Agent Skills Plugin](https://github.com/danielrosehill/Claude-Israel-Agent-Skills-Plugin) | General-purpose Israel-specific agent skills for Claude Code and other agentic CLIs |
| [Israel Shopping Plugin](https://github.com/danielrosehill/Claude-Israel-Shopping-Plugin) | Israeli-resident shopping — domestic channels + overseas B2C (AliExpress, Amazon, iHerb), search-pattern mappings |

## Feeders — ![Added](https://img.shields.io/badge/Added-success)

Skills already folded into a plugin. Workspaces remain open for future iteration.

| Repo | Description |
|---|---|
| [Medication Research Skills](https://github.com/danielrosehill/Israel-Medication-Research-Skills) | Patient-facing medication availability and access in Israel — kupot cholim formulary checks, `sal briyut` (health basket) status, generic equivalents, personal-import paths, pharmacy availability. |

## Feeders — ![WIP](https://img.shields.io/badge/WIP-orange)

Active workspaces, not yet folded into a plugin.

| Repo | Description |
|---|---|
| [Property Research Skills](https://github.com/danielrosehill/Israel-Property-Research-Skills) | Israeli residential property due diligence — Tabu (`nesach tabu`, `nesach merukaz`), Israel Land Authority leasehold checks, building file (`tik binyan`) retrieval, `heter bniya` history, `shimush choreg` detection, TAMA 38 / `pinui-binui` status, preservation flags, comparable sales (nadlan / madlan / yad2), neighbourhood character. |
| [Mortgage Research Skills](https://github.com/danielrosehill/Israel-Mortgage-Research-Skills) | Israeli residential mortgages (משכנתא) — Bank of Israel track-composition rules, CPI-linked (Madad) and Prime stress testing, DSR / LTV ceilings, self-employed and foreign-currency income discounts, oleh and first-home benefits, `mas rechisha`, `ishur ekroni` workflow, bridging and refinance, bank-by-bank quirks. |
| [AliExpress Israel Skill](https://github.com/danielrosehill/AliExpress-Israel-Skill) | Planning notes for an AliExpress skill with an Israel-buyer focus — shipping, customs, VAT thresholds, payment quirks. Targeted to graduate into the Israel Shopping plugin. |

---

# Plugin contents — point-in-time snapshot

Snapshots of what's actually inside each plugin as of **2026-05-06**. These drift; the plugin repos themselves are authoritative.

## Israel Agent Skills Plugin — skills

| Skill | Purpose |
|---|---|
| `ben-gurion-flight-board` | Live Ben Gurion (TLV) arrivals/departures from the official Israel Airports Authority board, filterable by city, airline, status |
| `discover-israel-skills` | Browse / install third-party Israel-focused Claude Code skills (tax, gov services, health, rail, cinema, post, etc.) |
| `drug-co-il-lookup` | Look up an Israeli medication on `drug.co.il` (Pharmacists Organisation site); returns Hebrew + English structured data |
| `environment-check` | Verify or set up runtime dependencies (Python modules, Playwright browsers, CLI tools) when another skill reports a missing dep |
| `fiber-availability-check` | Check fiber-optic deployment at an Israeli address across providers (Bezeq Bfiber, HOT Fiber) |
| `home-front-command-guidelines` | Pikud HaOref (פיקוד העורף) civilian emergency / shelter / protection guidelines — what to do during rocket / missile alerts |
| `install-companion-plugins` | Install or review other Claude Code plugins that complement this one (curated shortlist) |
| `israel-conferences` | Find upcoming conferences / summits / expos in Israel by topic (tech, AI, biomed, finance, marketing, HR, cyber, startup, etc.) |
| `israel-drugs-registry-lookup` | Authoritative lookup in the Ministry of Health Israeli Drug Registry (`israeldrugs.health.gov.il`) |
| `israel-news-rss` | Latest Israeli news via RSS — Jerusalem Post / Times of Israel / JNS (English) and Ynet / Maariv / Walla / Haaretz (Hebrew) |
| `israel-post-appointment` | Check / book / cancel appointments at Israel Post branches (דואר ישראל) |
| `jerusalem-council-meetings` | Browse / list / download protocols from Jerusalem Municipality council committee sittings |
| `jerusalem-municipality-report` | File a "106" public-contact report with Jerusalem Municipality (פנייה ל-106) |
| `kol-zchut-lookup` | Citizen / consumer / employment / tenant rights lookups via Kol-Zchut |
| `list-skills` | Categorised map of every skill in this plugin |
| `maccabi-medicine-lookup` | Check medicine status in Maccabi Healthcare Services (listed, POM, in `sal briyut`, requires Form 29C, etc.) |
| `medicine-availability-check` | Orchestrator: chains per-source lookups to answer "is drug X available to me in Israel" end-to-end |
| `miklatim-lookup` | Find public bomb shelters (מקלט ציבורי) near an address / coordinate / current position |
| `nsc-travel-threat` | Israel National Security Council travel threat level / advisory for a country |
| `salary-conversion` | Convert salaries between Israeli (monthly NIS) and international (annual local currency) conventions |
| `add-skill-to-plugin` | Internal: turn raw notes into a new plugin skill |
| `update-plugin-readme` | Internal: refresh the plugin README's "Skills" section from current `skills/*/SKILL.md` |

## Israel Shopping Plugin — skills

| Skill | Purpose |
|---|---|
| `search-aliexpress` | Search AliExpress from an Israel-buyer perspective — ILS pricing, IL channel, Hebrew layer |
| `fetch-listing` | Parse a specific AliExpress product URL/ID into structured JSON (title, price, ship-to-IL fee, lead time, ratings, store, landed cost) |
| `fetch-listing-api` | Fallback for `fetch-listing` via the official AliExpress Affiliate API (HMAC-SHA256 signed) |
| `free-shipping-only` | AliExpress search with server-side `filterCode:freeshipping` for Israel only |
| `exclude-combo-deals` | AliExpress search hiding `Max Combo` bundle listings |
| `il-reviews-show` | Show only Israeli-buyer reviews on an AliExpress product |
| `compare-to-local` | Cross-check whether an AliExpress product is also sold by Israeli retailers, and at what price |

## Israel Shopping Plugin — slash commands

| Command | Purpose |
|---|---|
| `/search-zap` | Search `zap.co.il` — the canonical Israeli price-comparison aggregator |
| `/tech-product-search` | Search tier-1 Israeli tech retailers (Ivory, KSP, Bug, TMS) for consumer tech |
| `/general-search` | Broader Israeli retail search — Ace, Home Center, Office Depot, Audioline + Google IL + niche categories |
| `/store-zap-lookup` | Find a retailer's Zap profile and retrieve seller rating + review count |
| `/rrp-check` | Compare an Israeli price (ILS) against international RRP/MSRP or a specific international retailer; reports markup % |
| `/freier-check` | Playful "are you a freier" assessment — premium vs. international RRP, verdict on the freier scale |
| `/pn-check` | Reverse-lookup an Israeli listing to its manufacturer part number / international SKU (useful for relabelled consumables) |
| `/whats-this-brand` | Identify an obscure Israel-only brand — probable OEM and international equivalents |
| `/convert-currency` | Convert between ILS and USD/EUR/GBP using a live FX API with fallback rate |
| `/add-store` | Append a user-added Israeli vendor to the persistent user store list (survives plugin updates) |

---

## Related

Adjacent indexes and resource lists. Not skills repos themselves.

| Repo | Description |
|---|---|
| [Israeli AI](https://github.com/danielrosehill/Israeli-AI) | Israel-specific agent skills, MCPs, and builders — broader index of the Israeli AI/agent landscape |
| [Israeli Open Source Projects](https://github.com/danielrosehill/Israeli-Open-Source-Projects) | Curated index of open-source Israeli projects (data, civic tech, finance, careers, real estate, smart home, media) |
| [Israel Projects Index](https://github.com/danielrosehill/Israel-Projects-Index) | Master index of all Israel-related repositories |
| [Israel Open Data Resources](https://github.com/danielrosehill/Israel-Open-Data-Resources) | Open-access data and a list of Israeli data projects |

## Naming

Train-Case for repo names on GitHub. Display names in this index use natural casing for readability. Skill slugs inside `skills/` directories use kebab-case to match Claude Code slash-command conventions.
