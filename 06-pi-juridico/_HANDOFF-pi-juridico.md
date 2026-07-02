# HANDOFF — Sessão "PI Jurídica" (para agente cloud)

> Gerado em 2026-07-02. Projeto: Lumio Copiloto — submissão Centelha 3 / FAPESQ, Fase 2.
> Branch: `pivot-ev-instalacao-2026-07-02`. Base commit: `dce8dd0`.
> **Todo output em português-br.** Você roda isolado na cloud — tudo que precisa
> está no repo (não há memória da conversa anterior; leia os arquivos indicados).

## 0. Leitura obrigatória antes de começar (NÃO reler o repo inteiro)
1. `CLAUDE.md` — contexto do projeto, regras de sessão, fórmula da nota, §4 (lacunas).
2. `INDEX.md` — dashboard, log de decisões (leia as entradas de **2026-07-02**), §3 e §5.
3. `_PIVOT-EV-2026-07-02.md` — brief-mestre do pivot (o que se submete = **software +
   base autoral**; instalação EV é lab/dogfood, não a inovação).
4. `06-pi-juridico/propriedade-intelectual.md` — **arquivo-alvo** (hoje só esqueleto).
5. `00-fontes/evidencias.md` — ledger de fontes (registrar toda afirmação factual aqui).

## 1. Objetivo da sessão
Preencher `06-pi-juridico/propriedade-intelectual.md`: **estratégia de PI de 1 página**
que fecha a **lacuna nº3/nº5 dos avaliadores** (PI não protegida). Levá-lo de ⬜ → ✅.

## 2. Contexto travado que a sessão DEVE respeitar (não reabrir)
- **Ativos a proteger** (do pitch): (1) **marca** "Lumio"/Copiloto (INPI); (2) **software**
  (registro de programa de computador no INPI); (3) **base autoral de verbetes NBR
  5410 (+17019 no H2)** — é o **moat durável** (direito autoral + segredo de negócio);
  (4) know-how da arquitetura agêntica.
- **A base autoral é 100% a construir no projeto** (nenhum verbete pronto hoje — ver
  `05-equipe/DT.md`). Consequência de PI: a **estratégia de cessão/titularidade** dos
  verbetes produzidos por **bolsistas** é crítica (a PI tem que ficar com a empresa,
  não com os bolsistas/UFCG). Isso é o ponto de PI mais importante e mais negligenciado.
- **Rubrica JÁ existe:** o `04-consistencia/O.md` reserva **R$6.000 (§7.1.d)** para
  "registro de PI no INPI (marca + software) + assessoria jurídica". A estratégia de PI
  deve **caber nesse envelope** e amarrar aos marcos do `CF.md` (protocolo no H1).
- **Edital financia PI:** §7.1.d cobre registro de PI (ver `evidencias.md`, linha da §7.1).
- **UFCG não formalizada / bolsas não exigem convênio** (circularidade dissolvida) —
  mas isso REFORÇA a necessidade de cláusula de cessão de PI nos termos de bolsa.

## 3. Pontos a resolver (grelhar o founder OU decidir com recomendação)
- [ ] **Titularidade/cessão de PI dos verbetes:** como garantir que a base autoral
      produzida por bolsistas (e mestrando) seja **cedida à empresa**? (cláusula no
      termo de bolsa / contrato de cessão de direitos autorais). É o item nº1.
- [ ] **Marca:** classe(s) de Nice para "Lumio"/Copiloto (software SaaS = classe 9/42);
      já houve busca de anterioridade no INPI? custo (~R$1k por classe).
- [ ] **Software:** registro de programa de computador no INPI (barato, ~R$185) —
      protege como? (protege o código-hash, não a funcionalidade). Vale a pena vs. só
      direito autoral automático + segredo? Recomendar sim (baixo custo, sinal ao avaliador).
- [ ] **Segredo de negócio:** o que NÃO patentear/registrar e proteger como segredo
      (prompts, pipeline RAG, curadoria) — política interna + NDA com PJ/bolsistas.
- [ ] **Patente?** provavelmente NÃO (software puro + método de negócio = baixa
      patenteabilidade no BR; caro e lento). Recomendar deixar fora e justificar.
- [ ] **Cronograma de PI:** amarrar aos marcos do CF (busca de anterioridade + protocolo
      de marca no H1; registro de software após consolidar MVP; cessão nos termos de
      bolsa ANTES da entrada dos bolsistas M4).
- [ ] **Custo:** distribuir dentro dos R$6.000 do O.md (marca 1–2 classes + software +
      assessoria de contrato de cessão).

## 4. Regras do projeto (não esquecer)
- Um tópico por sessão. Escrever SÓ em `06-pi-juridico/propriedade-intelectual.md`.
- Toda afirmação numérica/factual (custos INPI, prazos, classes) → registrar em
  `00-fontes/evidencias.md` com fonte; se não achar, `[FONTE PENDENTE]` — **não inventar**.
- Ao terminar: atualizar `INDEX.md` (dashboard: linha PI → ✅ · log append-only ·
  §5 ações) e **commitar** na branch acima. Mensagem de commit termina com o
  Co-Authored-By/Claude-Session padrão do projeto.
- NÃO reabrir Solução/Impacto/MN/O/CF/CE/DT (já fechados/fortes).

## 5. Suggested skills
- **grill-me** — se houver decisões abertas de PI que exijam o founder (ex.: busca de
  anterioridade já feita? nome definitivo da marca?). Foi o fluxo das sessões anteriores.
- Se o founder não estiver disponível (rodada autônoma na cloud): **decidir com
  recomendação** cada ponto do §3, marcando as dúvidas factuais como `[VALIDAR]`.

## 6. Estado do repositório
- Working tree limpo em `dce8dd0` (O/CF/CE/DT/INDEX commitados e pushados).
- Único arquivo-alvo ⬜: `06-pi-juridico/propriedade-intelectual.md`.
