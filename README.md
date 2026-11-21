# organic-visibility-br

Agent skill for **organic visibility in Brazil**: SEO (blue links), AEO (answer boxes / AI Overviews), and GEO (citations inside ChatGPT, Perplexity, Gemini, Copilot).

Works for **any Brazilian entity** — local business, ecommerce, SaaS, professional, creator — with local trust surfaces (Google Business Profile, Reclame Aqui, CNPJ-consistent NAP), correct AI crawler separation (OAI-SearchBot vs GPTBot), IndexNow, Business Hub readiness, and 4-stage perception probes with hallucination detection.

**Primary deliverable:** a single actionable Markdown report in Brazilian Portuguese, structured so it can be pasted into an agent chat and executed.

Skill instructions: English. Client report: pt-BR.

## Install

```bash
cp -R organic-visibility-br ~/.claude/skills/organic-visibility-br
```

`SKILL.md` must sit at the skill root.

### Claude.ai

Paste `SKILL.md` into a skill review card, or upload a ZIP whose first level contains `SKILL.md` plus `references/` and `assets/`.

## Usage

```text
Use organic-visibility-br. Audite a visibilidade orgânica de https://exemplo.com.br
Relatório completo em pt-BR, pronto para execução.
```

Optional: entity type or city if not discoverable from the URL.

## Layout

```
organic-visibility-br/
  SKILL.md
  README.md
  references/
    platforms-brasil.md      # weighted matrix + BR oracles + niches
    aeo-geo-schema.md        # bots, IndexNow, Business Hub, probes, citability evidence
    scoring.md               # 4 pillars + backlog horizons
    tactical-pages.md        # question landings, location pages, FAQ
    competitor-local.md      # local competitor gap analysis
    measurement.md           # GSC AI, GA4, probe cadence
    author-eeat.md           # scored E-E-A-T checklist (0-2 per signal)
    parasite-earned-mentions.md # off-site authority, review platforms, Reddit, G2
  assets/
    template-llms-txt.md
    template-robots-txt.md
    template-json-ld.md
    template-probes.md       # 4-stage probes ready to run
  examples/
    sample-intake.md
    sample-report-ptbr.md    # full sample output in pt-BR
```

## What this is not

- Not a substitute for Google Search Console or paid rank trackers
- Not is-agentic.com (UI agent usability); this skill covers discovery, entity, AEO/GEO and BR reputation
- Not legal, medical or financial advice

## Version

**2.6.0** — Parasite SEO & Earned Mentions module (Reclame Aqui, G2/Capterra, Reddit, Product Hunt, Doctoralia) with safe execution rules.

**2.5.0** — Full scored E-E-A-T audit checklist (Experience / Expertise / Authoritativeness / Trust) with Brazil-specific signals (CNPJ, Reclame Aqui, councils).

**2.4.0** — Measurement plan (GSC Generative AI + GA4 AI + probe cadence), Author/Experience signals for professionals & YMYL, stronger brand-mention weight, internal linking rule for tactical pages.

**2.3.0** — Competitor local SEO module: GBP, reviews, location pages, local pack gaps → closable backlog items.

**2.2.0** — Tactical pages: question landings, safe location/service-area pages (anti-doorway), strategic FAQ — high-ROI easy execution patterns.

**2.1.0** — Evidence refresh: Google official AI Overview rules, llms.txt demoted to hygiene (2026 studies), AI info/entity page alternative, nosnippet check, stronger earned-media emphasis, practitioner consensus (Bailyn/Indig/Solís/Ray).

**2.0.0** — Deep upgrade: autonomous Markdown report contract, universal entity support, research-backed citability rules, expanded platform detection (Apple Business Connect, Business Hub, Bing/IndexNow, etc.), critical-path backlog optimized for agent execution, evidence tags mandatory.

**1.1.1** — Probes template + sample report.  
**1.1.0** — Weighted matrix, BR oracles, IndexNow, Business Hub, 4-stage probes.  
**1.0.0** — Initial release.
