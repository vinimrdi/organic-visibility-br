# Scoring model (v2.0)

Total **0–100**. Four pillars × 25. Conservative: missing evidence lowers score and confidence.

## Pillar A — Fundação SEO (0–25)

| Points | Criteria |
|--------|----------|
| 0–5 | Crawl/index basics: HTTPS, canonical, no accidental noindex on money pages |
| 0–5 | robots.txt + sitemap coherent; IndexNow when high-publish cadence |
| 0–5 | On-page essentials: unique titles, lang=pt-BR, usable IA |
| 0–5 | Mobile/CWV only with data (GSC/CrUX); else cap and [NEEDS USER] |
| 0–5 | Internal linking to primary offers; thin/doorway risk absent |

## Pillar B — Prontidão Agentic / GEO access (0–25)

| Points | Criteria |
|--------|----------|
| 0–6 | AI search bots allowed (OAI-SearchBot, PerplexityBot, Claude-SearchBot…) + no WAF false blocks |
| 0–4 | Training bots policy explicit (GPTBot etc.) — coherent policy scores; chaos scores low |
| 0–4 | Main content available without critical client-only JS |
| 0–3 | llms.txt present and accurate **or** excellent architecture / dedicated entity facts page compensating (llms.txt is hygiene, not a citation driver) |
| 0–1 | No nosnippet / max-snippet blocks on money pages (snippet eligibility) |
| 0–4 | Schema Organization/LocalBusiness/Person with @id + meaningful sameAs + CNPJ match when used |
| 0–3 | Business Hub claim readiness / domain verification when eligible; IndexNow active |

## Pillar C — AEO / Conteúdo (0–25)

| Points | Criteria |
|--------|----------|
| 0–8 | Answer-first on primary landing pages |
| 0–6 | FAQ/HowTo/tables suitable for extraction + evidence triples |
| 0–6 | Query coverage in pt-BR (intent match, not stuffing) |
| 0–5 | Snippet risk controls (thin copy, duplicate, cloaking absent) |

## Pillar D — Autoridade externa BR (0–25)

| Points | Criteria |
|--------|----------|
| 0–7 | Reclame Aqui presence + response hygiene (or justified N/A for pure B2B) |
| 0–5 | GBP completeness / reviews hygiene when local or hybrid (relative to local competitors) |
| 0–5 | Consistent NAP + CNPJ alignment across site, schema, GBP, Receita |
| 0–4 | Social entity graph + sameAs quality |
| 0–4 | Third-party mentions, press, earned media, brand co-occurrence, niche directories or lists (quality over quantity; brand mentions correlate strongly with AI visibility) |

## Confidence

| Label | Meaning |
|-------|---------|
| Alta | Live fetches + consistent public data + probes run |
| Média | Partial access; some [NEEDS USER] |
| Baixa | Heavy inference; many gaps |

## Backlog horizons

- **48h**: access blockers (bots/WAF), NAP/CNPJ mismatch, unclaimed critical platforms, false credentials
- **30d**: schema, bios, tactical pages, review response, first earned mentions
- **90d**: content depth, case studies, consistent off-site presence, measurement loop
