# E-E-A-T Audit Checklist — Brazil (v2.5)

Practical, observable signals only.  
Score each item **0 / 1 / 2** (0 = absent or false, 1 = partial, 2 = clear & verifiable).  
Not every site needs every item. Weight higher for **YMYL / professional / health / law / finance**.

**Total possible:** varies by entity type. Report the raw score + the most critical gaps.

---

## 1. Experience (Experiência de primeira mão)

| # | Signal | 0 | 1 | 2 | Notes / evidence |
|---|--------|---|---|---|------------------|
| E1 | First-hand language on money pages (“atendemos”, “no nosso consultório”, números reais de casos) | | | | |
| E2 | Specific local or process details a non-practitioner could not invent (bairros, fluxos, prazos) | | | | |
| E3 | Original photos / job evidence / before-after (when ethical and real) | | | | |
| E4 | Case studies or client outcomes with concrete numbers or timelines | | | | |

**Subtotal Experience:** __ / 8

---

## 2. Expertise (Especialidade)

| # | Signal | 0 | 1 | 2 | Notes / evidence |
|---|--------|---|---|---|------------------|
| X1 | Named author or practitioner on key service / content pages (byline) | | | | |
| X2 | Author bio with role + relevant background | | | | |
| X3 | Verifiable credentials (CRM, OAB, CREFITO, CRC, certificates) — only true ones | | | | |
| X4 | Credentials link to public council / registry page when available | | | | |
| X5 | Schema `Person` with `name`, `jobTitle`, `hasCredential` or `sameAs` | | | | |
| X6 | “Revisado por” / medical or legal reviewer on YMYL content (when applicable) | | | | |

**Subtotal Expertise:** __ / 12

---

## 3. Authoritativeness (Autoridade)

| # | Signal | 0 | 1 | 2 | Notes / evidence |
|---|--------|---|---|---|------------------|
| A1 | Brand / professional mentioned on third-party sites (press, associations, lists) | | | | |
| A2 | Consistent profiles on high-weight BR platforms (LinkedIn, Doctoralia, Jusbrasil, council) | | | | |
| A3 | Organization / LocalBusiness schema with stable `@id` + meaningful `sameAs` | | | | |
| A4 | Appears in niche “melhores …” or directory lists with accurate NAP | | | | |
| A5 | Knowledge presence (Google Knowledge Panel or clear entity resolution) — if notable | | | | |

**Subtotal Authoritativeness:** __ / 10

---

## 4. Trustworthiness (Confiança) — highest priority

| # | Signal | 0 | 1 | 2 | Notes / evidence |
|---|--------|---|---|---|------------------|
| T1 | NAP identical across site, schema, GBP, and public CNPJ data | | | | |
| T2 | CNPJ / taxID accurate on site + schema when used | | | | |
| T3 | Reclame Aqui claimed + visible response process | | | | |
| T4 | Contact page with real channels (phone `+55`, WhatsApp, address or service area) | | | | |
| T5 | Privacy policy + basic legal pages present and linked | | | | |
| T6 | HTTPS everywhere; no obvious cloaking or doorway patterns | | | | |
| T7 | Visible “Atualizado em …” or `dateModified` on sensitive / price / process pages | | | | |
| T8 | Reviews responded to on GBP (and Reclame Aqui when relevant) | | | | |

**Subtotal Trustworthiness:** __ / 16

---

## Scoring guide for the main report

| Entity type | Focus | Minimum viable |
|-------------|-------|----------------|
| Local service / clinic / professional | Trust + Expertise + Experience | T1–T4, T8, X1–X3, E1–E2 |
| Ecommerce | Trust + Authoritativeness | T1–T6, A3 |
| SaaS / B2B | Authoritativeness + Expertise | A1–A3, X1–X2, T4–T5 |
| Creator / informational | Experience + Expertise | E1–E4, X1–X2 |

**How to use in the audit report**

1. Fill only the rows that apply.
2. List the **0s and critical 1s** under “Achados críticos” or “Sinais de autor / experiência”.
3. Turn each material gap into a backlog item (48h for false credentials or NAP mismatch; 30d for bios + schema; 90d for case studies and earned mentions).
4. Never invent credentials or experience. Mark [NEEDS USER] when the public page does not show the signal.

---

## Quick red flags (automatic critical)

- Credential claimed on site but absent or different on the professional council page
- NAP or CNPJ mismatch between site, GBP and Receita
- No human attribution on YMYL / professional service pages
- Reclame Aqui unclaimed with public complaints
- Thin location pages that only swap city names (doorway risk — already covered in tactical-pages)

---

## Link to other modules

- Platforms & NAP → `platforms-brasil.md`
- Schema patterns → `aeo-geo-schema.md`
- Measurement of citations after fixes → `measurement.md`
- Competitor gaps on reviews / authority → `competitor-local.md`
