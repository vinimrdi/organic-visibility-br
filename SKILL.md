---
name: organic-visibility-br
description: >
  Full organic visibility audit for any Brazilian entity (local, ecommerce, SaaS,
  professional, creator) across SEO, AEO and GEO. Generates a complete actionable
  Markdown report from a URL: scorecard, critical findings, platform claim status
  (Google Business Profile, Apple Business Connect, OpenAI Business Hub, Bing,
  Reclame Aqui, etc.), technical access (robots, WAF, IndexNow, llms.txt, schema),
  4-stage perception probes with hallucination flags + AI rank, competitive
  reverse-engineering (page types, search patterns, moves to copy), and a
  prioritized 48h/30d/90d backlog ready to paste into an agent chat for execution.
  Triggers: auditoria SEO Brasil, GEO, AEO, aparecer no ChatGPT, visibilidade
  orgânica, Business Hub, Reclame Aqui, GBP, otimização orgânica, engenharia
  reversa concorrente. Reports always in Brazilian Portuguese.
  Never invent rankings, citations or scores without evidence.
metadata:
  author: vinimrdi
  version: "2.7.0"
  language: en
  market: BR
  tags: [seo, aeo, geo, brazil, visibility, schema, llms-txt, robots, business-hub, indexnow, agent-skills, reverse-engineering, competitive]
---

# Organic Visibility BR — SEO + AEO + GEO (v2.7)

Universal organic visibility system for **any Brazilian entity**.

**Output contract:** one self-contained **Markdown report in pt-BR** that the user
can paste into Claude / Cursor / any agent chat and immediately start executing
fixes. No slides. No spreadsheets. No manual form filling beyond a URL (and optional
entity type if discoverable).

**Core rule:** entity resolution + Brazilian trust surfaces + crawl access beat
generic global SEO playbooks. Reclame Aqui, Google Business Profile, CNPJ-aligned
NAP, and verifiable facts outweigh empty superlatives.

## When to activate

- Any request to audit or improve organic visibility of a Brazilian brand/site
- "Aparecer no ChatGPT / Perplexity / Google AI Overviews"
- robots.txt, OAI-SearchBot, Cloudflare/WAF, llms.txt, Schema, IndexNow
- Claim status: Google Business Profile, Apple Business Connect, OpenAI Business Hub, Bing Webmaster, Reclame Aqui
- Full SEO + AEO + GEO checklist for Brazil
- Competitive reverse-engineering / "como o concorrente ganha tráfego"

## When NOT to use

- Paid media only (Ads, Media Boost) with zero organic goal
- Pure brand/logo design with no discovery surface
- Inventing "rank #1" or "cited by ChatGPT" without evidence

## Absolute constraints

1. **No invented evidence.** Tag every claim: [OBSERVED], [MISSING], [INFERRED], [NEEDS USER], [ESTIMATED].
2. Separate **SEO / AEO / GEO** in the scorecard.
3. Brazil-first reputation: Reclame Aqui, GBP, CNPJ public data, major BR press — not Yelp/BBB defaults.
4. Prefer verified Brazilian sources and earned corroboration over empty superlatives.
5. Never claim Business Hub, llms.txt, or any platform "guarantees" citation.
6. Treat llms.txt as hygiene/agent map, not a ranking lever (2026 evidence).
7. Check snippet eligibility (no nosnippet on money pages) for Google AI surfaces.
8. Location pages only with real local differentiation — never recommend pure city-name template swaps (doorway policy).
9. Competitor analysis: only public, reproducible signals; never invent review counts or rankings.
10. Always leave the client with a measurement plan (GSC AI report + probes + GA4).
11. Professional niches: never invent credentials; flag missing author/experience signals.
12. Conservative scoring when evidence is partial.
13. Language of the report: Brazilian Portuguese. Skill instructions remain English.

## Workflow

1. Resolve the entity (name, URL, city, type, CNPJ if public).
2. Technical access: robots.txt, OAI-SearchBot / GPTBot separation, WAF/Cloudflare blocks, IndexNow, sitemap, schema, llms.txt.
3. Platform claim status with weights (GBP, Apple Business Connect, OpenAI Business Hub, Bing, Reclame Aqui, niche directories).
4. Content citability + tactical pages opportunities (question landings, safe location pages, strategic FAQ).
5. Run or simulate 4-stage perception probes + AI rank + pages cited + hallucination check.
6. Competitive reverse-engineering (page types, search patterns, link magnets, moves to copy) when competitors are available.
7. Competitor local gaps when relevant.
8. Author / E-E-A-T scored checklist (especially YMYL / professional).
9. Off-site & Parasite/Earned Mentions (Reclame Aqui, G2/Capterra, Reddit, Doctoralia, LinkedIn, Product Hunt when relevant).
10. Produce the full Markdown report with scorecard, critical findings, backlog 48h/30d/90d, technical packages, and measurement plan.

## Progressive disclosure

- `references/platforms-brasil.md` — weighted platforms + Brazilian oracles (CNPJ, Reclame Aqui, etc.)
- `references/ai-visibility-probes.md` — 4-stage probes + AI rank + pages cited (v2)
- `references/competitive-reverse-engineering.md` — page types, search patterns, moves to copy
- `references/scoring.md` — pillars and backlog horizons
- `references/tactical-pages.md` — question landings, location pages, FAQ (anti-doorway)
- `references/competitor-local.md` — local competitor gap analysis
- `references/measurement.md` — GSC Generative AI + GA4 + probe cadence
- `references/author-eeat.md` — scored E-E-A-T checklist (0-2 per signal)
- `references/parasite-earned-mentions.md` — off-site authority, review platforms, Reddit, G2/Capterra, Reclame Aqui
- `assets/template-*.md` — ready-to-use robots, schema, llms.txt, probes
- `examples/sample-report-ptbr.md` — full example output

## Report structure (mandatory)

```markdown
# Relatório de Visibilidade Orgânica — [Marca]

## Scorecard (0–100)
SEO | AEO | GEO | Total + short rationale

## Achados críticos
Lista priorizada do que bloqueia resultado agora.

## Probes de percepção (4 estágios) + AI Rank
Tabela com engine, cited, posição, páginas citadas, alucinações, ação.
Ver `references/ai-visibility-probes.md`.

## Engenharia Reversa Competitiva (quando aplicável)
Playbook em 3 linhas + traffic engines + search patterns + moves to copy.
Ver `references/competitive-reverse-engineering.md`.

## Análise competitiva local (quando aplicável)
Tabela resumida cliente vs 2–3 concorrentes (GBP, reviews, páginas de área, local pack, Reclame Aqui) + gaps acionáveis.

## Checklist de plataformas (com peso)
| Plataforma | Peso | Status | Ação imediata |
|------------|------|--------|---------------|
| ... | Crítico / Alto / Complementar | OK / Parcial / Missing | ... |

## Pacotes técnicos prontos
- robots.txt (trecho ou completo)
- Schema JSON-LD (preenchido ou template)
- llms.txt (quando aplicável)

## Backlog executável
### 48 horas
- [ ] ...
### 30 dias
- [ ] ...
### 90 dias
- [ ] ...

## Business Hub / Apple Business / Bing / outros
Status e próximos passos por plataforma relevante.

## Sinais de autor / experiência / E-E-A-T
Checklist 0–2 por sinal. Listar gaps críticos e ações.

## Off-site & Parasite / Earned Mentions
Presença em plataformas de alta autoridade + ações no backlog.

## Plano de medição (pós-auditoria)
GSC Generative AI + GA4 AI Assistants + probes mensais fixos + reviews.

## Limitações da auditoria
O que não foi possível verificar e o que o usuário precisa fornecer.
```

The report must be self-contained: an agent reading only this Markdown should understand priority and be able to start implementing.

## Quality bar

- Critical path first: access blockers (bots/WAF), entity mismatches (NAP/CNPJ), missing high-weight platforms, then content citability.
- Prefer verified Brazilian sources and earned corroboration over empty superlatives.
- Never claim Business Hub, llms.txt, or any platform "guarantees" citation.
- Treat llms.txt as hygiene/agent map, not a ranking lever (2026 evidence).
- Check snippet eligibility (no nosnippet on money pages) for Google AI surfaces.
- Location pages only with real local differentiation — never recommend pure city-name template swaps (doorway policy).
- Competitor analysis: only public, reproducible signals; never invent review counts or rankings.
- Always leave the client with a measurement plan (GSC AI report + probes + GA4).
- Professional niches: never invent credentials; flag missing author/experience signals.
- Conservative scoring when evidence is partial.
- Language of the report: Brazilian Portuguese. Skill instructions remain English.
