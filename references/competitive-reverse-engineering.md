# Competitive Reverse-Engineering (BR)

Módulo de engenharia reversa competitiva para a skill organic-visibility-br.
Inspirado em reverse-engineer-marketing (REM) e reverse-engineer-seo (seo-party-skills), adaptado ao mercado brasileiro e ao foco orgânico + AEO/GEO.

## Objetivo

A partir de 1–3 URLs de concorrentes (ou do próprio cliente), extrair:

1. Quais **page types** geram tráfego non-brand
2. Quais **padrões de busca** esses tipos respondem
3. Quais páginas funcionam como **link magnets**
4. Stance de AI crawlers + presença em AI answers
5. Moves concretos e de fácil execução para o cliente copiar (em escala menor)

Tudo com evidência citada e unknowns explícitos.

## Workflow obrigatório

### 1. Size the domain
- Estimativa de tráfego orgânico mensal (quando disponível via ferramentas públicas ou GSC do cliente)
- Volume de keywords ranking
- Share de brand vs non-brand (aproximado)
- Referring domains e tendência (quando público)

### 2. Identificar page types (traffic engines)
Agrupar URLs por padrão estrutural:
- `/blog/` ou `/artigos/`
- `/cidade/` ou `/servico-em-cidade/`
- `/vs/` ou `/alternativas/`
- `/templates/` ou `/ferramentas/`
- `/precos/` + páginas de comparação
- FAQ / perguntas
- Páginas de integração ou cases

Para cada grupo relevante, anotar:
- Quantidade aproximada de keywords non-brand no top 20
- Página top do grupo
- Se parece template programático ou conteúdo editorial

### 3. Extrair search patterns
Dos títulos e H1s das páginas que rankeiam:
- "[serviço] em [cidade]"
- "melhor [categoria] [ano]"
- "[marca] vs [concorrente]"
- "como [problema]"
- "quanto custa [serviço]"

Agrupar padrões e listar exemplos reais.

### 4. Link magnets
Identificar páginas que atraem backlinks de forma desproporcional:
- Ferramentas gratuitas
- Relatórios anuais / dados originais
- Guias longos citados
- Páginas de comparação muito completas

### 5. AI / GEO signals
- Existe `llms.txt`?
- robots.txt permite OAI-SearchBot, GPTBot, PerplexityBot, Google-Extended?
- Há citações conhecidas em AI Overviews ou respostas de ChatGPT/Perplexity (quando verificável)?
- Páginas que aparecem como fonte em probes

### 6. Moves to copy (o output mais importante)
Para cada move:
- O que o concorrente faz
- Evidência (page type + padrão de busca)
- Como adaptar em escala menor (especialmente para PMEs e profissionais BR)
- Primeira página concreta a construir
- Horizonte sugerido (48h / 30d / 90d)

Regras anti-doorway:
- Nunca recomendar páginas de cidade que só mudam o nome do bairro/cidade
- Exigir diferenciação real (informação local, cases, fotos, dados do bairro, etc.)

## Formato de saída no relatório

```markdown
## Engenharia Reversa Competitiva

### Playbook em 3 linhas
[onde vem o tráfego] → [o que ganha] → [primeiro move]

### Traffic Engines (page types)
| Seção / Tipo | Tipo de produção | Keywords non-brand (aprox.) | Página top | Padrão de busca principal |
|--------------|------------------|-----------------------------|------------|---------------------------|
| ... | editorial / template | ... | ... | ... |

### Search Patterns prioritários
| Padrão | Exemplos | Volume relativo | Ação sugerida |
|--------|----------|-----------------|---------------|
| ... | ... | alto/médio/baixo | ... |

### Link Magnets observados
| Página / Tipo | Por que atrai links | Adaptável? |
|---------------|---------------------|------------|
| ... | ... | sim/não + como |

### Moves to Copy (priorizados)
1. **[Nome do move]**  
   Evidência: ...  
   Como fazer em escala menor: ...  
   Primeira página: ...  
   Horizonte: 48h / 30d / 90d

### O que NÃO copiar
- Vantagens de marca/idade/orçamento que o cliente não tem
- Táticas de doorway ou thin content
```

## Regras de evidência

- Toda afirmação de ranking ou volume deve ser marcada `[OBSERVED]`, `[ESTIMATED]` ou `[NEEDS TOOL]`.
- Nunca inventar números de tráfego ou posição.
- Preferir padrões estruturais visíveis (URLs, títulos, schema) a números precisos quando a ferramenta não estiver disponível.
- Sempre listar unknowns no final da seção.

## Integração com o restante da skill

- Os moves gerados alimentam o backlog 48h/30d/90d.
- Page types de localização alimentam `tactical-pages.md` (com regras anti-doorway).
- Sinais de AI alimentam a seção de probes e o score GEO.
- Link magnets alimentam a seção de Parasite/Earned Mentions.
