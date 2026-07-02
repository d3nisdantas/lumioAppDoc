# MN · Modelo de Negócio (peso dobrado em CP)

## Pergunta-âncora (o que faz um avaliador dar 5)
> Como ganha dinheiro: pricing por segmento, unit economics (CAC, LTV, payback), projeção de receita coerente com SOM. Eliminatório se fraco.

## ✅ DECISÃO TRAVADA (sessão grill 2026-06-23) — Eixo de cobrança
**Assinatura por técnico/assento, mensalidade fixa, em faixas.**
- Âncora de preço: ~R$30–50/técnico/mês (o "R$30 por indivíduo" da pesquisa, que
  parecia matar o negócio, vira **âncora por assento**). Uma PME com 5–10 técnicos
  → **R$150–500/mês por empresa**, muito mais realista que o ticket R$300–800 do
  pitch antigo.
- **Por que por assento:** (a) casa com o formato preferido na pesquisa
  (mensalidade fixa, 4 votos); (b) alinha valor — mais técnicos = mais dor de
  papelada/histórico/retrabalho resolvida; (c) é o mais fácil de modelar CAC/LTV.
- Descartado "por equipamento" (1 voto; descasa custo, pois o copiloto custa por
  consulta, não por ativo) e híbrido (complexo demais para venda consultiva ano 1).

## 🔔 LEMBRETE (founder, grill 2026-06-25)
- [ ] **Incluir clientes freemium no cálculo de CAC.** O plano gratuito (autônomo,
      ≤10 equipamentos) é canal de aquisição/topo-de-funil. O custo de servir os
      free (IA por consulta + infra) e a taxa de conversão free→pago precisam
      entrar no CAC blended e no modelo de unit economics. NÃO esquecer em B2.
- [ ] **Estimar custo-de-servir COMPLETO por usuário** (founder, 2026-06-25): não
      só IA. Decompor em (a) **fixo** (vector DB/RAG, hosting base, monitoramento —
      independe de nº de usuários no início) + (b) **variável/usuário** (IA por
      consulta + cota de infra CMMS: compute, banco, storage de fotos/manuais,
      banda). Modelar COGS total vs receita total, não só "margem por assento"
      (no início o custo fixo domina). Expor como inputs ajustáveis na planilha.

## ✅ Dependências RESOLVIDAS (sessão grill 2026-06-25 — detalhe nas seções abaixo)
- [x] **Fair-use cap / medição do copiloto** → Copiloto INCLUÍDO no assento, uso
      justo soft (não bloqueia). Ver seção "Pricing".
- [x] **Unit economics** (margem, custo-de-servir real) → ver seção "Unit economics"
      + `unit-economics.csv`.
- [x] **CAC por canal e payback** → ver "Unit economics" (CAC blended R$843→R$451;
      payback ~7,5 meses Y1).
- [x] **Projeção de receita amarrada ao SOM** → MRR meses 1–36, ARR anos 1–3.
- [x] **Sensibilidade a churn** → 3% / 5%(base) / 8%.

## 📌 Clarificação A (do founder, registrar no texto)
Os números de custo de IA + infra do pitch (R$7k IA / R$4,3k infra/mês) são
**estimativa dimensionada pela verba Centelha**, NÃO custo atual em operação. O
custo real será menor com IA commodity/chinesa. A estimativa serve para
dimensionar o orçamento, não para descrever a operação de hoje.

---

# B1 · Pricing (grill 2026-06-25)

## Tese de preço por segmento
O produto são **dois motores** (CMMS + Copiloto) e cada segmento valoriza uma
metade. O eixo de cobrança é **por assento**, mas o desenho captura WTP distinta
por segmento via **empacotamento**, não via inflar o preço/assento:

| Segmento | Plano | Lógica de preço |
|---|---|---|
| **Autônomo / solo** | **Free** | WTP ≈ "Nada"/"Até R$30" na survey → não force pagamento. Capture de graça, use como topo-de-funil e converta quando virar empresa. |
| **PME geradores (beachhead)** | **Equipe** | Pagador = empresa (tem orçamento). R$40/assento, mín. 2. Resolve o paradoxo do pagador. |
| **Grande operador** | (sem Enterprise) | **Cortado nesta fase.** Hipótese não validada; não modelar preço custom agora. |

## Tabela de planos

| | **Free** | **Equipe** (pago) |
|---|---|---|
| **Alvo** | autônomo / solo | PME geradores 2–10 |
| **Preço** | R$0 | **R$40/assento/mês, mín. 2 assentos** |
| **Usuários** | 1 | 2+ |
| **Equipamentos** | **≤ 10** | ilimitado |
| **CMMS** | ✓ completo | ✓ completo + gestão de equipe/rota |
| **Copiloto** | ✓ incluído, **uso justo ~20 consultas/mês** | ✓ incluído, **uso justo ~100 consultas/assento/mês** |
| **Cobrança** | — | **mensal default** + opção anual (~2 meses grátis, ~17% off) |

- **Sem Enterprise.** Decisão do founder: preferir base **Freemium** a topo Enterprise.
- **Gate de conversão Free→Equipe (duplo, o que estourar primeiro):** contratou
  **2º usuário** OU passou de **10 equipamentos**. O momento de pagar coincide com
  "virar empresa" — exatamente o beachhead PME.

## Resolução do fair-use cap (a dependência central)
O "problema" do assento fixo × IA por consulta **quase não existe** quando se olham
os números: custo de IA = R$0,01–0,05/consulta; uso típico (survey) ≈ 4–20
consultas/técnico/mês → **R$0,20–1,00/assento/mês** contra um assento de R$40.
A IA come 1–3% da receita do assento no caso típico.

→ **Decisão: Copiloto INCLUÍDO no assento, com uso justo generoso e SOFT** (cap
ancorado bem acima do uso real; monitora abuso, **não bloqueia o técnico no campo**
— bloquear destruiria a proposta de valor de segurança). Modelo medido/add-on foi
**descartado** no ano 1: adicionaria fricção de venda por ~R$1 de custo e mataria a
narrativa de bundle ("CMMS = receita imediata, Copiloto = acelerador embutido").
Add-on medido fica reservado para um eventual tier topo no futuro.

---

# B2 · Unit economics (grill 2026-06-25)

> Planilha completa: **`04-consistencia/unit-economics.csv`** (4 sheets: modelo
> mensal 1–36, ARR anual, CAC/LTV/payback por canal, sensibilidade a churn).
> Todos os custos marcados **`[VALIDAR]`** e expostos como inputs ajustáveis.

## Premissas travadas
| Premissa | Valor |
|---|---|
| Preço/assento | R$40 · mín. 2 · média **3 assentos/empresa** |
| ARPA | **R$120/empresa/mês** (= R$1.440/ano) |
| Churn base | **5%/mês** (consistente com GTM) → vida ~20 meses |
| CAC | R$1.000 (network) · R$216 (distribuidor, 15% do contrato anual) |
| Mix de canais | **80/20 → 50/50 → 30/70** (network→distribuidor, anos 1–3) |
| Horizonte | **36 meses**; trajetória 10 → 40 → 125 empresas (ancorada no SOM) |

## Custo-de-servir em 2 camadas `[VALIDAR — placeholders]`
A margem só é honesta se incluir **infra do CMMS + IA**, não só IA. E no início o
**custo fixo domina** — "margem por assento" engana.

- **Camada 1 — Fixo (independe de nº de usuários):** vector DB/RAG + hosting base +
  monitoramento ≈ **R$400–800/mês** (modelado R$600).
- **Camada 2 — Variável/usuário:** pago ≈ **R$2,50/assento/mês** (IA ~R$0,50 +
  infra ~R$2,00); free ≈ **R$1,80/usuário/mês** (IA ~R$0,30 + infra ~R$1,50).

## CAC, LTV, payback (churn base 5%/mês)

| Métrica | Network | Distribuidor | Blended Y1 (80/20) |
|---|---|---|---|
| CAC | R$1.000 | R$216 | **R$843** |
| LTV (receita) | R$2.400 | R$2.400 | R$2.400 |
| **LTV/CAC** | **2,4×** | **11,1×** | **2,8×** |
| Payback (contribuição) | 8,9 meses | 1,9 mês | **~7,5 meses** |

**CAC blended cai com o tempo** conforme o canal escalável amadurece:
Y1 R$843 (2,8×) → Y2 R$608 (3,9×) → Y3 R$451 (5,3×). Esta é a história de escala
(o canal barato — distribuidor — não está provado, por isso ele **ramps**, não
domina no ano 1).

## Projeção de receita e a curva de margem (a história certa de SaaS)

| Ano | Empresas (saída) | MRR saída | **ARR run-rate** | Margem (só pago) |
|---|---|---|---|---|
| 1 (mês 12) | 10 | R$1.200 | **R$14.400** | 43,8% |
| 2 (mês 24) | 40 | R$4.800 | **R$57.600** | 81,2% |
| 3 (mês 36) | 125 | R$15.000 | **R$180.000** | 89,8% |

- **Margem core (só pago)** sobe 44% → 81% → 90% — a curva SaaS clássica (no início
  o fixo pesa; dilui com escala).
- **Freemium é investimento deliberado** que drena a margem líquida (R$2.700/mês de
  custo de free no mês 36) — é o motor de aquisição. Por isso o **custo do free
  entra no CAC** (ver lembrete). Margem líquida incl. free: 29% (M12) → 72% (M36).

## Sensibilidade a churn (LTV base receita, ARPA R$120)
| Churn/mês | Vida | Retenção anual | LTV | LTV/CAC network | LTV/CAC distribuidor |
|---|---|---|---|---|---|
| 3% (alvo/upside) | 33 m | 69% | R$4.000 | 4,0× | 18,5× |
| **5% (BASE)** | 20 m | 54% | R$2.400 | **2,4×** | **11,1×** |
| 8% (downside) | 12,5 m | 37% | R$1.500 | 1,5× | 6,9× |

Mesmo no downside (8%), o canal distribuidor mantém LTV/CAC 6,9× — o modelo **não
é frágil**. A tese de lock-in de dados (histórico de equipamentos) sustenta a
narrativa de que o churn real tende ao cenário 3%.

---

# B3 · Scoring de verticais (grill 2026-06-25)

## Método
O critério "fit técnico" foi **dividido em dois**, porque o produto tem dois motores
e as verticais os valorizam de forma assimétrica: **Fit CMMS** (manutenção
recorrente de ativo) ≠ **Fit Copiloto** (decisão técnica em campo + reuso da base
autoral NBR já produzida). Pesos:

| Critério | Peso | O que mede |
|---|---|---|
| Mercado + crescimento | 30% | tamanho e taxa de expansão |
| Dor / decisão-em-campo | 25% | intensidade da dor → valor do Copiloto na hora |
| WTP | 15% | disposição a pagar do pagador |
| Fit CMMS | 15% | encaixe com manutenção recorrente |
| Fit Copiloto / reuso da base | 15% | quanto da base NBR 5410 já serve, sem conteúdo novo |

## Heatmap (escala 1–5; 🟥1 🟧2 🟨3 🟩4 🟢5)

> ⚠ **Pivot 2026-07-02:** "Solar + EV charging" estavam **agrupados** e penalizados
> juntos em reuso de base. Foram **desmembrados**: EV é instalação de baixa tensão
> que **REUSA a NBR 5410** (+ adiciona a NBR 17019, norma nova de foco = moat) → alto
> Fit Copiloto/reuso; **solar** é que puxa a NBR 16690 e não reusa a base. São
> verticais distintas. Ver `_PIVOT-EV-2026-07-02.md §5`.

| Vertical | Mercado (30%) | Dor/campo (25%) | WTP (15%) | Fit CMMS (15%) | Fit Copiloto (15%) | **Score** |
|---|---|---|---|---|---|---|
| **Instalação/adequação EV** *(H2, hipótese-a-validar)* | 🟢5 | 🟢5 | **`[VALIDAR]`** | 🟧2 | 🟩4 | **3,80–4,40** ¹ |
| **Solar / fotovoltaico** *(hipótese posterior)* | 🟢5 | 🟢5 | 🟨3 | 🟧2 | 🟧2 | **3,80** |
| ~~**Subestações BT/MT**~~ *(descartada como prioridade — ver nota ²)* | 🟨3 | 🟨3 | 🟩4 | 🟢5 | 🟩4 | 3,60 |
| Autônomo geral *(= canal Free, não receita direta)* | 🟩4 | 🟩4 | 🟥1 | 🟨3 | 🟩4 | 3,40 |
| Instalações prediais | 🟩4 | 🟨3 | 🟧2 | 🟧2 | 🟢5 | 3,30 |
| Bombas / motores industriais | 🟨3 | 🟨3 | 🟩4 | 🟩4 | 🟧2 | 3,15 |

*(Geradores = beachhead atual, fora do ranking de expansão.)*

¹ **Score exibido como faixa** porque a WTP do pagador de instalação EV é
**desconhecida** (`[VALIDAR em H1]`, ver `_PIVOT §6`): 3,65 fixos (Mercado+Dor+Fit)
+ WTP×0,15 → **3,80** se WTP=1 até **4,40** se WTP=5. Não fingimos precisão de WTP
que ainda não medimos.

² **Subestação: descartada como PRIORIDADE**, mas **retida como plano de contingência
do gate H1** — se a dor de EV não se confirmar, a equipe universitária redireciona o
esforço de norma para subestação (também é trabalho norma-pesado, adequado ao perfil
acadêmico dos bolsistas). O "de-risco por cliente concreto" do texto antigo **não
existe mais**: subestação é nicho raso (1 único cliente-final + concorrente de
software robusto). Ver `CF.md` (gate H1) e `_PIVOT §7`.

**Leitura:** **EV lidera** pela dupla mercado+Dor de campo somada a **reuso de base
alto** (a grande correção do pivot: EV reusa a NBR 5410 e só adiciona a 17019 — não
começa do zero como solar). A **penalidade em Fit CMMS (🟧2) é esperada e coerente**:
instalação é projeto/comissionamento, **não** manutenção recorrente — por isso entra
pelo **caminho leve** (tipo especial de OS, ver abaixo), não como módulo de obra.
Solar fica logo atrás mas **sem** o reuso de base (puxa NBR 16690) → hipótese
posterior, separada de EV.

## Recomendação: sequência de expansão pós-Centelha
1. **Geradores** — beachhead (em curso). *(inalterado)*
2. **Instalação/adequação EV — TRILHA DE APROFUNDAMENTO H2 (HIPÓTESE-A-VALIDAR).**
   Substitui subestação. **Forças:** reuso da NBR 5410 + norma nova NBR 17019 (moat) +
   laboratório na mão (~50 condomínios) + tailwind de frota EV + **abre o TAM**
   (CNAE 4321-5, 332k — instalação elétrica). **Fraqueza:** **dor ainda NÃO validada**
   → de-riscada pelo **gate de validação H1** (5–10 instalações-lab nos condomínios +
   plano B de 10–15 entrevistas com instaladores EV). Registrada honestamente como
   **hipótese**, não certeza (geradores é o fato; EV é a aposta de crescimento).
3. **Solar / demais** — hipóteses posteriores (solar exige NBR 16690, baixo reuso).
   **Subestação = contingência do gate H1**, não trilha ativa (ver nota ²).

*Autônomo geral* não é vertical de receita: é o **plano Free** (canal de aquisição).
*Prediais* e *bombas/motores* ficam para trás (predial: WTP/fit CMMS baixos e muito
informal; industrial: exige conteúdo novo e é nicho).

## Caminho leve e mini unit-economics do segmento EV
- **Instalação = tipo especial de OS** (ordem + checklist + comissionamento +
  laudo/ART), **não** um módulo de obra/ERP (fases, medição, materiais). Isso mantém
  o **pricing por assento coerente** (EV não vira produto de projeto à parte) e
  preserva a alegação de MVP 70%/500 testes. Ver `_PIVOT §3.4` e `CF.md`.
- **Unit economics de EV = a validar.** A WTP do **pagador de instalação** é
  desconhecida → a vertical EV terá **mini unit-economics própria após o gate H1**
  (`[VALIDAR]`). **O modelo de geradores (B2, ARPA R$120, churn 5%, LTV/CAC) NÃO muda
  por causa de EV** — ele é ancorado em geradores e permanece.

---

## Fontes
(registrar em 00-fontes/evidencias.md — WTP e formato da pesquisa já registrados)
- Sessão grill 2026-06-25 (Track B): pricing, fair-use cap, unit economics, scoring.
- `unit-economics.csv`: modelo próprio; premissas de custo `[VALIDAR]`.
