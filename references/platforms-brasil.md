# Platform matrix — Brazil (v2.0)

Mark each row: **OK / Partial / Missing / N/A**.  
Weight: **Crítico** (fix early) · **Alto** · **Complementar**.

Works for every entity type. Apply the universal block first, then the matching add-on block.

## Universal (all types)

| Platform | Weight | Why | Action if missing/partial |
|----------|--------|-----|---------------------------|
| Official website (HTTPS) | Crítico | Canonical entity home | Single host; clear About/Contact; schema |
| Google Business Profile | Crítico | Local + Maps + entity signals | Claim, categories, photos, posts, NAP match |
| Google Search Console | Crítico | Index / queries / CWV | Property verified |
| Bing Webmaster Tools + IndexNow | Alto | Bing index feeds ChatGPT Search & Copilot | Verify property; enable IndexNow key |
| Reclame Aqui | Crítico (consumer) / Alto (hybrid B2B) | Highest-weight BR trust signal for LLMs | Claim/verify; respond; improve indices |
| LinkedIn (Company or Personal) | Alto | B2B entity + strong sameAs | Complete About; same legal/trade name |
| Instagram (professional) | Alto | Discovery; Google indexes public posts | Bio + link + consistent handle |
| YouTube | Alto | Transcripts/titles feed Google/Gemini | Brand channel; accurate titles |
| OpenAI Business Hub (Businesses in ChatGPT) | Alto | Claim profile inside ChatGPT | Check eligibility; claim when available |
| Facebook Page | Complementar | Local/contact signals | Public page; NAP match |
| X (Twitter) | Complementar | Real-time / Grok-adjacent | Public bio + site link |
| Wikidata (if notable) | Complementar | Strong sameAs / KG | Only if item exists or is justified |
| Pinterest / Threads | Complementar | Extra discovery | Consistent branding when relevant |

## Brazilian data oracles (entity resolution)

| Source | Weight | What to verify | Action |
|--------|--------|----------------|--------|
| Receita Federal / CNPJ public data | Crítico | Razão social, nome fantasia, CNAE, endereço, situação | Match Schema taxID, site footer, GBP |
| Casa dos Dados / Econodata / similar | Alto | Quadro societário, secondary addresses | Flag name collisions or stale data |
| CNPJ on site + schema | Crítico | Public taxID accuracy | Use only when appropriate and correct |

**Rule:** Any mismatch between CNPJ data, Schema, GBP and site footer is high-severity.

## Add-ons by entity type

### Local (store, clinic, restaurant, services with area)

| Platform | Weight | Notes |
|----------|--------|-------|
| Apple Business Connect | Alto | Maps + Siri path |
| WhatsApp Business (consistent link) | Alto | Primary contact in BR |
| iFood / Rappi / vertical apps (if F&B) | Alto | Category discovery |
| TripAdvisor / Booking-class (tourism) | Alto | Review + entity |
| Quality city/vertical directories | Complementar | GuiaMais, sector councils, city portals — NAP-consistent only; avoid pure spam PACs |

### Professional / YMYL (health, law, finance, education)

| Platform | Weight | Notes |
|----------|--------|-------|
| Doctoralia / equivalent | Alto | Health professionals |
| Jusbrasil | Alto | Legal |
| Conselho / registry pages (CRM, OAB, CREFITO…) | Crítico | Credential verification |
| Google Scholar / Lattes (academic) | Alto | When research-facing |

### SaaS / B2B software

| Platform | Weight | Notes |
|----------|--------|-------|
| G2 / Capterra / B2B Stack | Alto | Review + category rankings |
| Product Hunt | Complementar | Launch / innovation signal |

### Ecommerce

| Platform | Weight | Notes |
|----------|--------|-------|
| Marketplace presence (Mercado Livre, Amazon BR…) | Alto | When relevant |
| Trustpilot / Reclame Aqui | Alto | Trust layer |

## How to score in the report

- List only platforms that apply.
- Crítico gaps → 48h backlog.
- Alto gaps → 30d.
- Complementar → 90d or later.
