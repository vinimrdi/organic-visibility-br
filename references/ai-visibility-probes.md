# AI Visibility & Perception Probes (v2)

Upgrade dos probes de 4 estágios com lógica de rank-on-ai e pages-cited.
Inspirado em rank-on-ai e reverse-engineer-geo (seo-party-skills).

## Objetivo

Simular a jornada real do brasileiro nas principais engines de IA e medir:

1. Se a marca entra na shortlist (descoberta cega)
2. Como ela se compara ao concorrente principal
3. Percepção de confiança e risco (Reclame Aqui etc.)
4. Alucinações e dados desatualizados
5. Quais páginas as engines citam (para priorizar otimização ou criação)

## Os 4 estágios (obrigatórios)

### Probe 1 — Descoberta Cega (Topo/Meio)
```
Quais são as melhores opções de [CATEGORIA/SERVIÇO] no Brasil [ou CIDADE] hoje?
Liste prós, contras e faixa de preço aproximada.
```
Mede: a marca aparece na shortlist sem ser citada no prompt?

### Probe 2 — Comparativo Direto (Fundo)
```
[MARCA] ou [CONCORRENTE PRINCIPAL]: qual vale mais a pena para [PERFIL DE CLIENTE]?
```
Mede: posicionamento relativo e argumentos que a IA usa.

### Probe 3 — Prova Social & Risco (Validação)
```
[MARCA] é confiável? Quais são as principais reclamações no Reclame Aqui e avaliações de clientes?
```
Mede: reputação e se a IA puxa dados de Reclame Aqui / review sites.

### Probe 4 — Auditoria de Alucinação
```
Me dê o resumo completo da [MARCA]: o que faz, onde fica, quem fundou, quanto custa e quais os canais oficiais.
```
Mede: dados inventados ou desatualizados. Cruzar contra Schema, sameAs, GBP e site oficial.

## Engines a testar (quando possível)

- ChatGPT (com e sem browsing, se disponível)
- Perplexity
- Google AI Overviews / AI Mode
- Gemini
- Claude (quando o usuário tiver acesso)

Se não for possível rodar ao vivo, simular com base em evidências públicas e marcar claramente como `[SIMULATED]`.

## Output no relatório

```markdown
## Probes de Percepção (4 estágios)

| Estágio | Engine | Marca citada? | Posição / Menção | Páginas citadas | Alucinações / Dados errados | Ação |
|---------|--------|---------------|------------------|-----------------|-----------------------------|------|
| 1 Descoberta | ChatGPT | Sim/Não | ... | ... | ... | ... |
| 1 Descoberta | Perplexity | ... | ... | ... | ... | ... |
| 2 Comparativo | ... | ... | ... | ... | ... | ... |
| 3 Confiança | ... | ... | ... | ... | ... | ... |
| 4 Alucinação | ... | ... | ... | ... | ... | ... |

### Resumo de rank em AI
- Apareceu em X de Y respostas de descoberta
- Foi a primeira opção em Z respostas
- Páginas mais citadas pelas engines: [lista]
- Principiais críticos de alucinação a corrigir via Schema/sameAs/conteúdo

### Páginas prioritárias para citação
Lista das URLs que as engines já usam (ou deveriam usar) + gaps de conteúdo.
```

## Regras de execução

1. Parametrizar sempre com `[CATEGORIA]`, `[CIDADE]`, `[MARCA]`, `[CONCORRENTE]`, `[PERFIL]`.
2. Rodar os mesmos prompts em mais de uma engine sempre que possível.
3. Registrar literalmente trechos relevantes da resposta (com data).
4. Cruzar dados do Probe 4 com fontes oficiais (site, Schema, GBP, CNPJ).
5. Nunca afirmar "rankeamos #1 no ChatGPT" sem evidência daquele run.
6. Alimentar o backlog com:
   - Correções de alucinação (48h)
   - Páginas que faltam para serem citáveis (30d)
   - Estratégia de menções em fontes que as IAs já confiam (90d)

## Integração

- Resultados alimentam o score GEO.
- Páginas citadas alimentam a priorização de conteúdo e Schema.
- Alucinações alimentam a seção de Entity / NAP / sameAs.
- Moves de citação alimentam Parasite/Earned Mentions e Competitive Reverse-Engineering.
