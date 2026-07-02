# O · Orçamento (peso 2x dentro de CP)

## Pergunta-âncora (o que faz um avaliador dar 5)
> Orçamento por rubrica alinhado a cronograma e equipe; o que o recurso Centelha financia (bolsistas, etc), dentro das regras do edital.

## ✅ DECISÃO TRAVADA (sessão grill 2026-06-23) — Estrutura de recursos
Dois envelopes distintos (regras do edital, §6 e §7.1):

### A) Subvenção econômica — até R$85.333 (itens financiáveis §7.1)
| Item edital | Uso planejado | Resolve gap |
|---|---|---|
| (g) Pró-labore de sócio (≤30% do valor total) | Founder: CMMS + liderança comercial | banda do founder / bus factor |
| (d) Serviços de terceiros PJ | **Dev do Copiloto** (consultoria/assessoria técnica) | núcleo do Copiloto |
| (d) Serviços de terceiros PJ | **Advisor B2B + assessoria de plano de negócios + marketing/anúncios** | **gap comercial nº1** |
| (d) Serviços de terceiros PJ | **Registro de PI no INPI (marca + software)** | **gap PI nº5** |
| (d/h) Serviços PJ | Contador | obrigação legal |
| (c) Material de consumo (inclui software) | API de IA (commodity/chinesa) + cloud + normas NBR + livros | custo Copiloto |
| (a/b) Diárias e passagens nacionais | Visitas ao piloto + prospecção comercial em campo | trilha comercial |
| (f) Equipamentos/material permanente | Mínimo (arquitetura cloud-first) | — |
| (e) Incubadora (pré-incubação) | Opcional, se aplicável | — |

### B) Bolsas de Fomento Tecnológico — até R$50.000 (§6, via FAPESQ↔CNPq)
- 2 bolsistas eng. elétrica (DTI) → verbetes NBR + curadoria de manuais.
- 1 mestrando/doutorando CC (DTI/SET) → arquitetura de IA/LLM (aprofundamento).
- **Concedidas ao projeto aprovado; recrutadas pelo coordenador** — NÃO dependem
  de convênio institucional formal com a UFCG (ver PDT: circularidade dissolvida).

## ⚠ Restrições do edital que moldam a equipe (registrar)
- **Nenhum salário CLT pela subvenção.** Dev do Copiloto = **PJ** (serviço técnico,
  com nota fiscal, sem caracterizar vínculo) ou sócio com pró-labore.
- Pró-labore só para **sócios** formalmente na equipe executora, teto **30%** do
  total, parcelas mensais iguais, ≤12 meses.

## 💰 Orçamento detalhado por rubrica (grill 2026-07-02) — amarrado a CF e CE

### A) Subvenção econômica — R$85.333 (fecha exatamente o teto)
| # | Rubrica | Valor | §7.1 | Amarração ao CF (marco) | Resolve |
|---|---|---|---|---|---|
| 1 | Pró-labore do founder — R$1.000/mês × 12 (**15h/sem**) | **R$12.000** | (g) | M1–M12 (liderança CMMS+comercial) | banda founder / bus factor |
| 2 | Dev PJ júnior (founder = tech lead) — pacotes PJ, média R$3.000/mês | **R$36.000** | (d) | concentra M1–M6 (integração/agente-de-manuais) e M7–M11 (agente-de-normas) | núcleo do Copiloto |
| 3 | **Comercial** — assessoria de plano de negócios + ads/marketing | **R$16.000** | (d) | H1 descoberta→LOIs (M5); H2 ads no funil (M7–M12) | **gap nº1** (GTM/vendas) |
| 4 | **PI/INPI** — marca + programa de computador + assessoria jurídica | **R$6.000** | (d) | registro protocolado no H1; estratégia de PI | **gap nº5** (PI) |
| 5 | IA/infra — API commodity + cloud + normas ABNT + livros | **R$8.000** | (c) | M2+ (retriever), escala no H2 (base de normas) | custo Copiloto |
| 6 | Contador — R$400/mês × 12 | **R$4.800** | (d/h) | M1–M12 | obrigação legal |
| 7 | Diárias/passagens — visitas ao piloto + prospecção | **R$2.533** | (a/b) | M2–M5 (descoberta) e M7+ (comercial) | trilha comercial |
| | **TOTAL SUBVENÇÃO** | **R$85.333** | | | |

> **Base do teto de 30% do pró-labore = valor da subvenção (R$85.333).** 30% =
> R$25.600; o pró-labore adotado (R$12.000 = 14%) fica **bem abaixo do teto** →
> defensável. Confirmado no texto do edital (registrar em `evidencias.md`).

> **Decisão de desenho (grill 2026-07-02):** o founder mantém outro emprego e dedica
> **15h/sem** ao Lumio → puxa pró-labore **simbólico** (R$1.000/mês, mantém a rubrica
> §7.1.g viva como sócio-executor) e **realoca R$6.000 do pró-labore para a linha
> comercial** (R$10k→R$16k). Narrativa de consistência: *"o founder garante a própria
> subsistência por fora, permitindo que a subvenção seja majoritariamente reinvestida
> no produto (dev PJ) e no gap comercial — reduzindo o risco de colapso se a receita
> demorar."* Transforma o "part-time" em mitigação de risco, não em fraqueza.

> **Advisor B2B = pro-bono** (carta de intenção, ação urgente <10/08) → **não consome**
> a rubrica comercial; os R$16.000 vão para plano de negócios + ads (alimenta o CAC do
> GTM/AARRR). Ver `05-equipe/CE.md`.

### B) Bolsas de Fomento Tecnológico — ≤ R$50.000 (§6, via FAPESQ↔CNPq)
| Bolsista | Modalidade | Papel (CF/`_PIVOT §3.7`) | Valor unitário |
|---|---|---|---|
| 2× eng. elétrica | DTI (nível a confirmar) | base autoral: manuais geradores (H1) → normas EV NBR 5410+17019 (H2) | `[VALIDAR: tabela FAPESQ/CNPq]` |
| 1× mestrando CC | modalidade superior (mestrado) | arquitetura agêntica / IA | `[VALIDAR: tabela FAPESQ/CNPq]` |

> **Valores unitários NÃO inventados** — tabelados pela agência. Marcados `[VALIDAR]`;
> founder pesquisa a tabela do edital. O total (R$50.000) é o teto real.
>
> ⚠ **Tensão de consistência O↔CF a resolver com a tabela** `[VALIDAR]`: o O modela
> **12 bolsa-mês por bolsista**, mas o CF põe a **entrada em M4 (~9 meses efetivos)**.
> Ao obter a tabela, reconciliar por uma das três vias: (i) a modalidade sobe e 12m
> cabe no teto; (ii) antecipa-se a entrada dos bolsistas; ou (iii) o O passa a orçar
> 9 meses. Deixar explícito é o tipo de coerência que o CP premia.

## Como isto rebate o ataque do red-team (O)
O orçamento antigo "desmentia" a intenção comercial e não tinha PI. Agora **ambos
têm rubrica explicitamente autorizada pelo edital** (§7.1.d), e o dinheiro
condicional (bolsas) está amarrado a entregável condicional (aprofundamento/H2),
mantendo o núcleo financiado por recursos não-condicionais (subvenção).

## O que falta detalhar (sessão dedicada de O)
- [x] Valores por rubrica somando ≤ R$85.333 (subvenção) + R$50.000 (bolsas). ✅ grill 2026-07-02.
- [x] Amarrar cada rubrica a um marco do cronograma (CF). ✅ (coluna "Amarração ao CF").
- [x] Confirmar base do teto de 30% do pró-labore = valor da subvenção (R$85.333). ✅.
- [ ] `[VALIDAR]` valores unitários de bolsa (tabela FAPESQ/CNPq) + reconciliar 12m vs. entrada M4.

## Fontes
(registrar em 00-fontes/evidencias.md — §6 e §7.1 do edital já registrados)
