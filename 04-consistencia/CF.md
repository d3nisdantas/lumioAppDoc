# CF · Cronograma físico (peso 2x dentro de CP)

## Pergunta-âncora (o que faz um avaliador dar 5)
> Cronograma de 12 meses com marcos, entregáveis e dependências, coerente com escopo técnico restante e contratações.

## ✅ DECISÃO TRAVADA (grill 2026-06-23, revista no pivot 2026-07-02) — Escopo dos 12 meses
**Geradores-first (núcleo) com aprofundamento em INSTALAÇÃO/EV no H2** — substitui
subestação (nicho raso: 1 cliente-final + concorrente robusto). Ver
`_PIVOT-EV-2026-07-02.md`.

| Metade | Foco da equipe universitária | Quem | Lógica |
|---|---|---|---|
| **H1 (M1–M6)** | **Manuais de geradores** (catalogação) | Founder (CMMS+comercial) + Dev PJ (Copiloto) + equipe univ. a partir do M4 | manual-pesado → valida a **experiência de agente-sobre-manuais** |
| **H2 (M7–M12)** | **Normas** (EV: NBR 5410 reusada + NBR 17019 nova) | Bolsistas eng. elétrica + Mestrando CC + Dev PJ | norma-pesado → trabalho autoral/acadêmico, ideal para bolsistas |

**Por que manuais→normas (não o inverso):** a equipe universitária é responsável pela
**catalogação de manuais e normas**. Começa por **manuais de geradores** (H1) para
validar a experiência de agente-sobre-manuais; só então (H2) avança para o trabalho
**norma-pesado** (EV), que é o mais autoral e onde mora o moat (NBR 17019).

## 🗓 Calendário-âncora (edital Centelha 3 — datas reais)
- Divulgação dos resultados finais: **02/10/2026**.
- Contratação dos projetos: **03/10 a 31/12/2026**.
- **out–dez/2026** = janela de **articulação/recrutamento** da equipe universitária
  (bolsas CNPq recrutadas pelo coordenador) em paralelo ao núcleo.
- **Equipe universitária inicia os trabalhos no Q1/2027** (jan–mar), **no mais tardar
  ao fim de março/2027**.
- Execução dos 12 meses: **M1 = out/2026 → M12 = set/2027**.

## 👥 Entrada escalonada de recursos (mostra maturidade de gestão)
| Recurso | Entra | Papel (`_PIVOT §3.7`) |
|---|---|---|
| **Founder** | M1 (out/26) | CMMS geradores + comercial (pró-labore) |
| **Dev PJ** | M1–M2 | integração no produto / Copiloto |
| **Bolsistas eng. elétrica** | **M4–M6 (Q1/27)** | base autoral/conteúdo: manuais geradores (H1) → normas EV NBR 5410+17019 (H2) |
| **Mestrando CC** | **M4–M6 (Q1/27)** | arquitetura agêntica/IA (independe do gate; amadurece no H2) |

## 🚦 Os DOIS gates (o coração da consistência)
- **Gate 1 — MERCADO (~M4–5):** a dor de instalação EV **ainda NÃO foi validada**.
  Tocado pelo **founder** (independe da equipe univ.): **5–10 instalações-laboratório**
  nos ~50 condomínios + **plano B** (10–15 entrevistas com instaladores EV, se a obra
  em condomínio atrasar). **Decide o alvo do H2:**
  - **Ramo verde (esperado):** dor confirmada → H2 aprofunda **EV** (NBR 5410 + 17019).
  - **Ramo de contingência:** dor EV fraca mesmo após plano B → H2 redireciona o mesmo
    esforço para **subestação** (também norma-pesada → mantém os bolsistas produtivos
    em trabalho autoral que justifica a verba CNPq). O **núcleo (geradores) e a verba
    não se perdem** — só muda o alvo do aprofundamento.
- **Gate 2 — TÉCNICO (fim do H1, ~M6):** o **agente-baseado-em-manuais** (geradores)
  está validado → luz verde para construir o **agente-baseado-em-normas** (conformidade
  EV) no H2. Sequência de risco: não se constrói o agente de norma sem antes provar o
  de manual.

## 🪶 Caminho leve (obrigatório — preserva MVP 70% e cabe em 12m)
Instalação EV = **tipo especial de OS** (ordem + checklist + comissionamento +
laudo/ART). **NÃO** se constrói ERP/módulo de obra (fases, medição, materiais). Módulo
de obra = visão pós-Centelha, só se o mercado puxar. Ver `_PIVOT §3.4` e `MN.md`.

---

## 📊 Cronograma granular M1–M12 (raias por recurso)

Legenda de marcos: ◆ marco-chave · ▸ entregável · 🚦 gate

| Mês (calend.) | Founder (CMMS+comercial) | Dev PJ (integração/Copiloto) | Bolsistas elétrica (base autoral) | Mestrando CC (arquitetura agêntica) | Marco / entregável | Dependência |
|---|---|---|---|---|---|---|
| **M1** out/26 | Kick-off; contrato do piloto em operação; onboarding do piloto no CMMS geradores | Contratação PJ; setup de ambiente | — (recrutamento) | — (recrutamento) | ◆ Projeto contratado; ambiente de dev pronto | Resultado do edital (02/10) |
| **M2** nov/26 | Descoberta comercial c/ pagador (donos de PME); início da articulação da equipe univ. | Integração do retriever de manuais (geradores) | — | — | ▸ Retriever de manuais v0; ▸ roteiro de descoberta | M1 |
| **M3** dez/26 | Descoberta EV: mapeamento dos ~50 condomínios; roteiro do plano B | Copiloto geradores: citação + safety/LOTO | — (seleção concluída) | — (seleção concluída) | ◆ Equipe univ. selecionada; ▸ pipeline de condomínios | M2; articulação univ. |
| **M4** jan/27 | **Início das instalações-laboratório EV** nos condomínios | Copiloto geradores em produção no piloto | **Entra:** catalogação de manuais de geradores + curadoria da NBR 5410 (reuso) | **Entra:** pesquisa de arquitetura agêntica (baseline) | ▸ 1ª instalação-lab; ▸ MVP Copiloto geradores no piloto | M3; entrada da equipe (≤ fim mar/27) |
| **M5** fev/27 | Instalações-lab + entrevistas do plano B; 1ªs LOIs de geradores | Refino do Copiloto por feedback do piloto | Base de manuais de geradores + verbetes-piloto | Prova de conceito do laço de feedback | 🚦 **GATE 1 (mercado)**: EV ✅ ou contingência subestação | Instalações-lab + plano B |
| **M6** mar/27 | Consolida aprendizado do gate; define recorte da base H2 | Fecha integração do agente-de-manuais | Fecha base autoral de geradores (manuais) | Guardrails de recusa v0 | 🚦 **GATE 2 (técnico)**: agente-de-manuais validado; ◆ **fim do H1** | Gate 1; Copiloto geradores |
| **M7** abr/27 | Primeiros contratos pagos (geradores); advisor B2B ativo | Início da integração do **agente-de-normas** (tipo-de-OS instalação) | **Vira para normas:** verbetes NBR 17019 (EV) + NBR 5410 aplicada a instalação | Arquitetura do **copiloto agêntico de conformidade** | ▸ Esqueleto do tipo-de-OS "instalação EV"; ◆ 1º contrato pago | Gate 1 (verde) + Gate 2 |
| **M8** mai/27 | Expansão comercial geradores; discovery de WTP do pagador EV | Fluxo agêntico: coleta dados do local → checa requisitos | Verbetes NBR 17019 (núcleo: requisitos de recarga) | Laço de aprendizado por feedback (mensurável) | ▸ Fluxo agêntico de conformidade v0 | M7 |
| **M9** jun/27 | Comercial; consolidação de métricas do piloto | Geração de memorial/laudo assistido | Verbetes 17019 (aterramento, proteção, seccionamento) | Métricas: taxa de citação correta, taxa de correção caindo | ▸ Laudo/ART assistido v0; ▸ base 17019 ~50% | M8 |
| **M10** jul/27 | Comercial; NPS e churn do piloto | Guardrails de recusa integrados (anti-alucinação) | Verbetes 17019 (memorial descritivo, ativação concessionária) | Guardrails de recusa v1 (recusa fora da base) | ▸ Copiloto EV: recusa segura fora da base | M9 |
| **M11** ago/27 | Comercial; preparo de mini unit-economics EV `[VALIDAR]` | Integração completa do copiloto de conformidade EV | Base NBR 5410+17019 consolidada (revisão) | Avaliação de desempenho do agente (métricas de campo) | ▸ Copiloto agêntico de conformidade EV — integrado | M10 |
| **M12** set/27 | Relatório final; metas comerciais; roadmap pós-Centelha | Hardening; documentação técnica | ◆ **Base autoral EV entregue** (verbetes NBR 5410+17019) | ◆ Relatório de arquitetura agêntica + métricas | ◆ **Fim do H2**: copiloto de conformidade EV + base autoral | M11 |

*(Contingência de gate: se Gate 1 = subestação, as raias de bolsistas nos M7–M12
substituem "verbetes NBR 17019 (EV)" por "verbetes de subestação (NBR aplicável)";
o restante do cronograma — datas, marcos, dev PJ, mestrando — permanece.)*

## 🧵 Caminho crítico
`entrada da equipe univ. (M4–M6)` → `base de manuais de geradores (H1)` →
`Gate 2 técnico (M6)` → `verbetes de norma EV (H2)` → `copiloto agêntico de
conformidade (M11–M12)`. O elo mais sensível é a **entrada da equipe universitária no
Q1/27**: todo o H2 depende dela. Por isso os bolsistas começam por **base 5410
(reuso, já existe)** — trabalho útil e **não-condicional** ao gate, que serve tanto a
geradores quanto a EV, dando "ramp" produtivo antes de M7.

## 🛟 Contingências
- **Gate 1 negativo (dor EV fraca):** H2 vira **subestação** (norma-pesada, mantém
  bolsistas produtivos e a verba justificada). Núcleo de geradores intacto.
- **Atraso na entrada dos bolsistas (recrutamento):** founder segura um **escopo
  autoral mínimo** (curadoria da 5410 já existente) e o dev PJ prioriza integração do
  agente-de-manuais; o recorte de norma do H2 é redimensionado, não cancelado.
- **Obra em condomínio lenta (assembleia):** aciona o **plano B** (entrevistas com
  instaladores EV) para não travar o Gate 1.

## 🧭 Trilha comercial DENTRO do cronograma (fecha gap do red-team)
- **H1:** descoberta com pagador (donos de PME) → validação de pricing → **1ªs LOIs**
  (M5). Marcos comerciais com responsável (founder) e meta de clientes — não item
  solto no T4.
- **H1→H2:** **primeiros contratos pagos** (M7); advisor B2B ativo.
- **Meta ancorada no SOM:** trajetória de 10 empresas em 12 meses (ver `MN.md` B2).

## 📌 Clarificação B (do founder, registrar no texto)
O cronograma de 12 meses é **pós-vitória no Centelha**. O investimento é o que
viabiliza contratar (dev PJ + bolsistas) e custear a IA (commodity/chinesa, mais
barata). O escopo só é executável nesse cenário de recurso aprovado.

## O que ainda falta detalhar (alimenta de O e CE — por isso CF fica 🟡)
- [ ] Amarrar cada marco a valores de **rubrica do `O.md`** (bolsas, dev PJ, IA/infra).
- [ ] Confirmar composição/tempo da **equipe (`CE.md`)** para fechar a alocação fina.
- [ ] Definir critério quantitativo do **Gate 1** ("dor EV confirmada" vs. contingência).

## Fontes
(registrar em 00-fontes/evidencias.md)
- Sessão grill 2026-07-02 (pivot EV): calendário out/26–set/27, entrada escalonada,
  6+6 manuais→normas, dois gates, caminho leve, contingências.
- Datas do edital (divulgação 02/10/2026; contratação 03/10–31/12/2026). `[FONTE PENDENTE]` (nº do edital)
- NBR 17019 (recarga de VE) — título/ano/status. `[FONTE PENDENTE]`
