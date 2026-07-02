# INDEX.md — Memória do Orquestrador · Lumio Centelha Fase 2

> Painel central. O orquestrador (você) navega por AQUI. Cada sessão-worker
> atualiza a linha do seu tópico e o log de decisões ao terminar.
> Atualizado em: 2026-07-02

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
| PI | Impacto | `02-impacto/PI.md` | Que impacto positivo medível (segurança, conformidade)? | 🟡 revisar (EV) | Baixa (consolidar) |
| EX | Impacto | `02-impacto/EX.md` | Que externalidades (acadêmico UFCG, regional, emprego)? | 🟡 revisar (EV) | Baixa |
| FV | Mercado | `03-mercado/FV.md` | Que valor concreto entrego a cada segmento? Disposição a pagar? | 🟡 revisar (EV) | **Alta** |
| PE | Mercado | `03-mercado/PE.md` | Como escala? PLG, efeito de rede, custo marginal? | 🟡 revisar (EV) | **Alta** |
| GTM | Mercado (gap) | `03-mercado/GTM.md` | Posicionamento, canais, CAC, funil de aquisição? | 🟡 revisar (EV) | **Crítica** |
| MN | Consistência ⚠ | `04-consistencia/MN.md` | Pricing por segmento, unit economics, receita? | 🟡 revisar (EV) | **Crítica** |
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
- 2026-06-23 · [modelo de negócio · grill] · As 4 decisões do §3 RESOLVIDAS. (1) Beachhead = PME de geradores (pagador=empresa, usuário=técnico); expansão p/ eletricistas em geral nas Fases 2–3 ("entrar caro-e-estreito p/ sair barato-e-amplo"). (2) Pricing = assinatura por técnico/assento, mensalidade fixa, ~R$30–50/assento. (3) Equipe = founder (CMMS+comercial, pró-labore) + dev PJ (Copiloto) + advisor B2B 20 anos (carta a formalizar) + bolsas: 2 elétrica + 1 mestrando CC; comercial dedicado por gatilho. (4) Escopo = geradores H1 (núcleo) + subestação H2 (bolsistas). · pareceres apontavam negócio como gargalo.
- 2026-06-23 · [fatos · edital] · Circularidade UFCG DISSOLVIDA: bolsas (§6.1–6.3) são concedidas ao projeto aprovado via FAPESQ↔CNPq e recrutadas pelo coordenador — não exigem convênio UFCG. Subvenção §7.1.d financia explicitamente assessoria de plano de negócio/marketing/anúncios E registro de PI → gaps comercial e PI ganham rubrica. Restrição: sem CLT pela subvenção (dev=PJ); pró-labore só sócio, teto 30%.
- 2026-06-23 · [pesquisa] · pesquisa.csv (n=9) registrada no ledger com ressalvas: viés de seleção (grupo de geradores) → usar como apetite, não dimensionamento; WTP individual ~R$30 vira âncora por assento; paradoxo do pagador (quem paga não vê valor e vice-versa) → reforça pagador=empresa.
- 2026-06-25 · [modelo de negócio · grill · Track B] · MN FECHADO. Pricing: Free
  (autônomo, CMMS+Copiloto, 1 usuário, ≤10 equip., uso justo ~20/mês) + Equipe
  (R$40/assento, mín. 2, uso justo ~100/assento); SEM Enterprise (founder preferiu
  Freemium a topo). Copiloto INCLUÍDO no assento, uso justo soft (IA custa só 1–3%
  do assento → cap é trava anti-abuso, não alavanca). Gate Free→pago: 2º usuário OU
  >10 equip. Cobrança mensal default + opção anual. Unit economics (`unit-economics.csv`,
  4 sheets): ARPA R$120; churn base 5%/mês (consistente c/ GTM), sens. 3%/8%; custo-
  de-servir 2 camadas (fixo R$400–800 + var R$2,50 pago/R$1,80 free) `[VALIDAR]`;
  CAC blended R$843→R$451 (mix 80/20→30/70); LTV/CAC 2,4×(network)/11,1×(distrib.);
  payback ~7,5 m; ARR 14,4k→57,6k→180k (36m, SOM-ancorado); margem core 44%→90%.
  Freemium = canal PARALELO (não infla SOM), custo do free entra no CAC (lembrete).
  Scoring verticais: fit dividido em CMMS×Copiloto; pesos Mercado30/Dor-campo25/WTP15/
  FitCMMS15/FitCopiloto15. Sequência: geradores→SUBESTAÇÃO (comprometida, puxada por
  cliente)→SOLAR/EV (hipótese-a-validar: alto mercado/Copiloto mas exige conteúdo de
  norma novo). 2 LEMBRETES no MN.md: incluir free no CAC + estimar custo-de-servir real.
- 2026-06-25 · [impacto · grill · Track D] · PI + EX FECHADOS. (1) Espinha causal
  MEDIADA: Copiloto eleva conformidade/adesão a LOTO+citação de norma (proxy
  controlável); 840 mortes = contexto, não KPI → desarma "vínculo copiloto→vida é
  narrativo". (2) DUAS espinhas de valor/impacto: A=segurança+agilidade diagnóstica
  (Copiloto); B=digitalização/inclusão via CMMS especializado-por-nicho de baixo
  custo (via IA) vs. generalistas. (3) FBC pragmático 13 blocos (cortados Biophysical
  Stocks/Ecosystem Services/Value Co-Destruction); Ecosystem Actors = humanos
  influenciados (não ecologia). (4) Negativos declarados+mitigados: viés-IA, pegada-IA,
  deskilling; "deslocamento júnior" reposicionado como POSITIVO (inclusão). Sem
  correlação ambiental forçada (só pegada-IA no lado Planeta). (5) Externalidades em
  2 ANDARES: piso garantido (empregos, capacitação piloto, digitalização, bolsas CNPq,
  normas replicáveis) + upside IES (lab, orientação, Campina Grande/NE) → desarma
  circularidade. (6) Impact Gap Canvas: lacuna = INTERSEÇÃO de 5 atributos (fundamentado
  +seguro+no-fluxo+acessível+especializado). (7) ToC: indicadores = proxies medidos no
  piloto (LOTO/citação, tempo-diagnóstico); COMPROMISSO DE MEDIÇÃO + baseline, NÃO
  percentuais cravados (desarma "tudo é hipótese"); metas duras só onde controla
  (adoção, verbetes, bolsistas). `*` marca tudo condicionado a vencer o edital.
- 2026-06-25 · [mercado · grill] · Track A (FV+PE+GTM) fechado. TAM=332.833 (CNAE 4321-5, Econodata mai/2026). SAM=~8.750–10.000 (CNAE 3313-9/01, ≤10 func.). SOM 12m=10 empresas; SOM 36m=100–150. CMMS como produto de receita imediata (mês 1 pós-resultado), Copiloto como acelerador H2. VPC 3 segmentos: autônomo (digitalização+laudo), PME geradores (margem+junior autônomo — beachhead), grande operador (padronização+auditabilidade — hipótese). Bullseye: interno=WhatsApp+distribuidores; meio=referral+SEO; externo=YouTube/LinkedIn/CREA. AARRR: CAC R$144–1.000; aha moment = Copiloto cita manual específico; MRR mês 12 = R$1.200; LTV/CAC 2,4–11×. Subestações incluídas no SAM (mesmo CNAE, mesmo perfil). 840 mortes por acidentes elétricos 2024 (ABRACOPEL) — dado mais forte que "centenas" do pitch.
- 2026-07-02 · [solução · PIVOT · grill] · **SUBESTAÇÃO SAI, INSTALAÇÃO/ADEQUAÇÃO EV ENTRA** como vertical de aprofundamento H2 (subestação = nicho raso: 1 cliente-final + concorrente robusto; custo de sair baixo pois tração é de geradores). Brief-mestre: `_PIVOT-EV-2026-07-02.md`; briefings por pasta: `03-mercado/`, `04-consistencia/`, `02-impacto/_BRIEFING-pivot-ev.md`. **8 decisões:** (1) submete-se o SOFTWARE + base autoral; instalação EV = lab/dogfood, NÃO a inovação (evita colapso de CP). (2) Geradores segue beachhead (piloto ASSINADO = tração intacta). (3) Subestação sai; EV entra em H2. (4) **Caminho leve:** instalação = tipo especial de OS + laudo/ART, NÃO ERP de obra → preserva MVP 70%/500 testes e cabe em 12m. (5) **Gate de validação H1** (~mês 4–5): dor EV NÃO validada → 5–10 instalações-lab nos ~50 condomínios + plano B (10–15 entrevistas c/ instaladores EV) decidem o recorte de H2. (6) **PDT-espinha:** copiloto agêntico de conformidade normativa + laço de aprendizado por feedback + guardrails de recusa, ancorado em base autoral NBR 5410+17019. (7) Equipe/verba: bolsistas elétrica=base/conteúdo · mestrando CC=arquitetura agêntica · dev PJ=integração. (8) Refrigeração/Linha 1 = FORA da submissão (adjacência de geradores; baixa norma → sem moat, não justifica CNPq) = expansão pós-Centelha. ⚠ CORREÇÃO a propagar: no MN.md desmembrar "Solar+EV" → EV REUSA NBR 5410 (+17019 nova=moat), perfil ≈ "instalações prediais" (alto reuso/base, baixo Fit CMMS); solar é que puxa NBR 16690. Moat NÃO inverte: base autoral=moat durável; arquitetura agêntica=PDT/motor. EV é HIPÓTESE-a-validar, geradores é fato. Status FV/PE/GTM/MN/PI/EX → 🟡 revisar (EV).

---

## 3. Decisões de negócio que travam outras frentes (RESOLVIDAS 2026-06-23 · escopo H2 revisto no pivot 2026-07-02)
Resolvidas na sessão de grill (modelo de negócio). Detalhe nos arquivos citados.
- [x] **Segmento prioritário:** PME de manutenção de **geradores** (pagador=empresa,
      usuário=técnico); expansão p/ eletricistas em geral nas Fases 2–3. → `03-mercado/GTM.md`
- [x] **Modelo de pricing:** assinatura **por técnico/assento**, mensalidade fixa,
      ~R$30–50/assento. Dependência: fair-use cap + unit economics.
      Instalação EV entra como **tipo especial de OS dentro do modelo por assento**
      (caminho leve), **não** como produto de projeto à parte. → `04-consistencia/MN.md`
- [x] **Equipe/verba:** founder (CMMS+comercial, pró-labore) + dev **PJ** (Copiloto)
      + advisor B2B (carta a formalizar) + bolsas (2 elétrica + 1 mestrando CC);
      comercial dedicado por gatilho. Composição **inalterada** pelo pivot; papéis das
      bolsas definidos no `_PIVOT-EV §3.7` (elétrica→base autoral NBR 5410+17019;
      mestrando CC→arquitetura agêntica; dev PJ→integração). → `05-equipe/CE.md` + `04-consistencia/O.md`
- [x] **Escopo técnico 12 meses:** geradores H1 (núcleo, founder+subvenção) +
      **instalação/adequação de carregadores EV** H2 (aprofundamento, bolsistas),
      via **caminho leve** (instalação = tipo especial de OS, não ERP de obra) e
      **gate de validação H1** (~mês 4–5: 5–10 instalações-lab nos ~50 condomínios +
      plano B de entrevistas c/ instaladores EV). Substitui subestação (nicho raso:
      1 cliente-final + concorrente robusto). → `04-consistencia/CF.md`
      · detalhe no log 2026-07-02 e `_PIVOT-EV-2026-07-02.md`.

---

## 4. Branches (Gitflow)
- `develop` — integra toda a pesquisa.
- `feat/red-team` · `feat/mercado` · `feat/modelo-negocio` · `feat/pi-juridico`
  · `feat/cronograma-orcamento` · `feat/solucao-impacto-equipe`
- Tópico fechado → merge em `develop`. Submissão final sai de `develop`.

---

## 5. Próximas ações (o orquestrador edita isto a cada sessão)
1. ~~Rodar sessão red-team~~ ✅ · ~~Resolver as 4 decisões do §3~~ ✅ (2026-06-23).
2. ~~**MN** — fechar unit economics + pricing + scoring~~ ✅ (Track B, 2026-06-25).
   ⚠ Pendências `[VALIDAR]` herdadas: custo-de-servir real (CMMS+IA), conversão
   freemium, e **incluir custo do free no CAC** (2 lembretes no `MN.md`).
3. **O** — valores por rubrica somando aos tetos (R$85.333 + R$50.000), amarrados
   a marcos do CF; confirmar base do teto de 30% do pró-labore.
4. **CE/DT** — obter carta de intenção do advisor B2B (ação urgente, < 10/08).
5. **PI jurídica** — estratégia de 1 página + INPI marca/software + cláusula de
   cessão de PI nos termos de bolsa.
6. **FV/PE/CF** — entrevistas com pagador + curva de custo marginal + cronograma
   granular com marcos comerciais.
7. **CF/EV** — cronograma físico nasce com **H2 = instalação/EV** (não subestação),
   incluindo o **gate de validação H1** (~mês 4–5) como marco entre validar e
   aprofundar, o caminho leve (tipo-de-OS, não ERP de obra) e a divisão de equipe do
   `_PIVOT-EV §3.7`. Ver pivot §9.
