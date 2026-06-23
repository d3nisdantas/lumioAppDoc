# INDEX.md — Memória do Orquestrador · Lumio Centelha Fase 2

> Painel central. O orquestrador (você) navega por AQUI. Cada sessão-worker
> atualiza a linha do seu tópico e o log de decisões ao terminar.
> Atualizado em: 2026-06-22

---

## 0. Objetivo desta rodada
Produzir os insumos brutos organizados para a submissão do **Projeto de Fomento
(Fase 2)** do Centelha 3, priorizando os critérios de maior peso e as lacunas
apontadas pelos avaliadores (ver `CLAUDE.md` §4).

**Deadline de submissão:** 10/08/2026 · **Buffer interno:** fechar até 03/08.

---

## 1. Dashboard de progresso (atualize aqui)
Status: ⬜ não iniciado · 🟡 em andamento · ✅ fechado · 🔴 bloqueado

| # | Critério (peso) | Arquivo | Pergunta-âncora ("o que dá 5?") | Status | Prioridade |
|---|---|---|---|---|---|
| EDD | Solução | `01-solucao/EDD.md` | Que evidências provam o estágio atual (MVP 70%, testes, piloto)? | ⬜ | Baixa (consolidar) |
| PDT | Solução | `01-solucao/PDT.md` | Qual a tese de evolução tecnológica nos 12 meses? | ⬜ | Média |
| PI | Impacto | `02-impacto/PI.md` | Que impacto positivo medível (segurança, conformidade)? | ⬜ | Baixa (consolidar) |
| EX | Impacto | `02-impacto/EX.md` | Que externalidades (acadêmico UFCG, regional, emprego)? | ⬜ | Baixa |
| FV | Mercado | `03-mercado/FV.md` | Que valor concreto entrego a cada segmento? Disposição a pagar? | ⬜ | **Alta** |
| PE | Mercado | `03-mercado/PE.md` | Como escala? PLG, efeito de rede, custo marginal? | ⬜ | **Alta** |
| GTM | Mercado (gap) | `03-mercado/GTM.md` | Posicionamento, canais, CAC, funil de aquisição? | ⬜ | **Crítica** |
| MN | Consistência ⚠ | `04-consistencia/MN.md` | Pricing por segmento, unit economics, receita? | ⬜ | **Crítica** |
| CF | Consistência ⚠ | `04-consistencia/CF.md` | Cronograma físico 12 meses, marcos, entregáveis? | ⬜ | **Alta** |
| O  | Consistência ⚠ | `04-consistencia/O.md` | Orçamento por rubrica, alinhado a equipe e cronograma? | ⬜ | **Alta** |
| DT | Equipe | `05-equipe/DT.md` | Domínio técnico do núcleo + UFCG comprovado? | ⬜ | Baixa (consolidar) |
| CE | Equipe (gap) | `05-equipe/CE.md` | Capacidade de execução + lacuna comercial endereçada? | ⬜ | Média |
| — | PI jurídica (gap) | `06-pi-juridico/propriedade-intelectual.md` | Que ativos proteger e como (marca, software, base autoral)? | ⬜ | **Alta** |
| — | Red-team | `99-red-team/gaps.md` | Onde um avaliador atacaria? (RODAR PRIMEIRO) | ✅ | feito 22/06 |

---

## 2. Log de decisões (append-only — nunca apagar)
Formato: `YYYY-MM-DD · [tópico] · decisão · porquê`

- 2026-06-22 · [setup] · Estrutura criada, priorização travada em Mercado+CP+PI · pareceres apontaram negócio como gargalo.
- 2026-06-22 · [red-team] · `gaps.md` gerado atacando o pitch real (v2). TOP 5: (1) MN sem modelo/pricing → risco de eliminação em CP; (2) equipe comercial abstrata; (3) beachhead indefinido (autônomo/MEI × PME); (4) circularidade UFCG; (5) PI zero.
- 2026-06-22 · [fatos] · Empresa-piloto ASSINADA (prova de tração). UFCG NÃO formalizada — condicional a vencer o Centelha (verba CNPq). Pricing em aberto. Perfil comercial e PI/registros = inexistentes. CLAUDE.md §1 corrigido.
- 2026-06-22 · [decisão pendente] · Beachhead não decidido pelo founder. Recomendação do red-team: PME de geradores (v1 só atende gerador/subestação; autônomo/MEI é v3). Reabrir só com ônus da prova.

---

## 3. Decisões de negócio que travam outras frentes (resolver cedo)
Estas precisam de resposta ANTES de orçamento/cronograma:
- [ ] **Segmento prioritário** do go-to-market (autônomo/MEI · PME · enterprise)?
- [ ] **Modelo de pricing** por segmento (assinatura? por OS? por técnico?).
- [ ] **Equipe a contratar** com recurso Centelha (define O e CE).
- [ ] **Escopo técnico restante** dos 12 meses (define CF).

---

## 4. Branches (Gitflow)
- `develop` — integra toda a pesquisa.
- `feat/red-team` · `feat/mercado` · `feat/modelo-negocio` · `feat/pi-juridico`
  · `feat/cronograma-orcamento` · `feat/solucao-impacto-equipe`
- Tópico fechado → merge em `develop`. Submissão final sai de `develop`.

---

## 5. Próximas ações (o orquestrador edita isto a cada sessão)
1. Rodar sessão **red-team** → gera `99-red-team/gaps.md`.
2. Resolver as 4 decisões do §3 (sessão de modelo de negócio).
3. Abrir frentes Alta/Crítica em paralelo.
