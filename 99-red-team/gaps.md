# 99-red-team/gaps.md — Ataque cético à proposta (Fase 2 · Centelha 3)

> Avaliador ad hoc cético, especialista em mercado e viabilidade de negócio.
> Fonte atacada: pitch real `~/projects/lumioApp/lumio-copiloto_v2.md` (22 slides
> + apêndices) + `requirements.md` do GerenciaLume + `CLAUDE.md`. Sem elogios.
> Atualizado em 2026-06-22.

## Fatos apurados nesta sessão (base do ataque)
- **Beachhead INDEFINIDO.** Founder oscila entre autônomo/MEI/ME(≤5) e PME. O
  produto v1 (escopo Centelha) só atende gerador + subestação; autônomo/MEI é,
  pelo próprio pitch (Slide 10), a fase **v3**. Vender p/ autônomo agora =
  vender algo que ainda não existe pra ele.
- **Pricing EM ABERTO.** Nenhum modelo decidido; "pesquisa dará luz". Slide 12
  cita ticket R$300–800/mês como hipótese, sem validação.
- **Perfil comercial ABSTRATO.** Nenhuma pessoa real para mercado/vendas/
  estratégia. Sem rubrica no orçamento (Slide 17). Era o ponto nº1 dos 2 pareceres.
- **Empresa-piloto: acordo ASSINADO** (prova forte e real de tração).
- **UFCG: NÃO formalizada.** Será buscada *se* vencer o Centelha (viabilizada
  pela verba de bolsas CNPq). → circularidade: o moat depende do prêmio.
- **PI formal = ZERO.** Sem marca/INPI, sem registro de software, sem cessão de
  direitos da base autoral. A afirmação "base é propriedade do projeto" é nua.

---

## Subcritérios

### EDD — Estágio de Desenvolvimento (Solução)
- **Objeção:** "70% do MVP" é auto-reportado, sem auditoria externa. E é 70% do
  **GerenciaLume (gestão)** — o **Copiloto**, que é o objeto da subvenção, está
  praticamente em 0%: não há nenhuma das tabelas (`copiloto_*`, `manuais`,
  `verbetes_kb`), nem retriever, nem safety-check implementados. O TRL 4–5
  declarado refere-se à gestão, não à IA fundamentada que se está pedindo verba
  para construir. Qual a evidência objetiva do estágio do **Copiloto**?
- **Risco de nota:** **4.** Cai de 5 porque a parte financiada (IA) é greenfield;
  segura em 4 pelo MVP maduro + 250 testes + piloto assinado.
- **O que falta:** (a) separar claramente "o que já existe" (GerenciaLume) de "o
  que será construído" (Copiloto), com % honesto de cada; (b) print/demonstração
  ou repositório que comprove os 250 testes e o 70%; (c) registrar empresa-piloto
  assinada como evidência de validação em ambiente relevante (sustenta TRL).
- **Prioridade:** Baixa (consolidar evidência; não reabrir).

### PDT — Potencial Diferencial Tecnológico (Solução · peso 2x dentro de S)
- **Objeção:** O próprio pitch admite que o modelo de IA é commodity. O moat
  declarado tem 3 camadas e **as duas mais fortes são frágeis hoje**: (1) a base
  autoral NBR depende **integralmente da UFCG, que não está formalizada e é
  condicional a ganhar este edital** — circularidade pura; (2) o efeito de rede
  em manuais só liga na **v2** (compartilhamento entre clientes), fora do escopo
  Centelha, e ainda depende de parecer jurídico. Resta a "integração ao fluxo da
  OS", que um concorrente com CMMS replica. Por que o diferencial não desmorona
  se a UFCG não vier?
- **Risco de nota:** **3.** Conceito é forte e defensável no papel, mas a
  evidência de defensabilidade é condicional/futura.
- **O que falta:** (a) Plano B para a base autoral caso a UFCG não se concretize
  (ex.: engenheiro consultor cedendo verbetes); (b) carta de anuência de
  professor/departamento da UFCG **antes de submeter**, quebrando a circularidade;
  (c) evidência de que ≥1 manual já foi indexado e gerou resposta citável (prova
  de conceito da camada técnica).
- **Prioridade:** **Alta** (peso 2x em S; é o coração da tese tecnológica).

### PI — Potencial de Impacto socioambiental (Impacto)
> ⚠ Não confundir com Propriedade Intelectual (ver bloco transversal abaixo).
- **Objeção:** A narrativa de impacto (segurança elétrica via LOTO obrigatório,
  conformidade NBR, mortes por choque) é forte, mas **100% dos números são
  hipóteses a validar** (redução 30–50% de diagnóstico, LOTO >95%, retorno -20%).
  O pitch é honesto sobre isso (Slide 5), o que é bom — mas o avaliador pergunta:
  qual a base mínima que sustenta que esse impacto é *plausível*, e não otimismo?
- **Risco de nota:** **4.** Impacto social claro e alinhado a dor real; perde o 5
  por depender de medições futuras e por o vínculo "uso do copiloto → vida salva"
  ser narrativo.
- **O que falta:** (a) 1–2 fontes citáveis (ABRACOPEL, MTE) já no ledger de
  evidências, com números; (b) baseline da empresa-piloto, mesmo que parcial, que
  ancore as hipóteses; (c) estimativa de alcance (nº técnicos/OS/ano) que
  dimensione o impacto agregado.
- **Prioridade:** Baixa (consolidar; já está forte).

### EX — Externalidades (Impacto)
- **Objeção:** As externalidades destacadas — formação de RH UFCG, ancoragem
  regional no NE, descentralização da inovação — **dependem todas da parceria
  UFCG condicional**. Se a parceria não vier, sobra emprego de 1 dev júnior. Qual
  externalidade sobrevive sem a UFCG?
- **Risco de nota:** **3–4.** Boa narrativa regional/acadêmica, mas exposta ao
  mesmo risco de circularidade.
- **O que falta:** Externalidades que não dependam exclusivamente da UFCG
  (geração de empregos diretos, fornecedores locais, capacitação de técnicos da
  empresa-piloto, contribuição replicável a outras normas — NR-10, NBR 14039).
- **Prioridade:** Baixa.

### FV — Fatores de Viabilidade / Valor ao cliente (Mercado)
- **Objeção:** O valor é descrito, mas **a disposição a pagar nunca foi
  validada** — nem uma entrevista de cliente citada além do piloto. E o valor
  entregue **difere radicalmente conforme o segmento indefinido**: para a PME de
  geradores o ROI é tempo de diagnóstico/retrabalho; para o autônomo é outra
  coisa. Sem fixar o segmento, "valor" é abstrato. Quem paga, quanto, e por quê
  comprovadamente?
- **Risco de nota:** **2–3.** Proposta de valor articulada, mas sem prova de
  demanda paga e sem segmento fixo.
- **O que falta:** (a) **decidir o beachhead** (recomendação: PME de geradores);
  (b) 5–10 entrevistas de descoberta com o ICP confirmando dor e WTP; (c) carta
  de intenção de compra de 1–2 clientes além do piloto.
- **Prioridade:** **Alta** (M tem peso elevado; foi gap explícito do Avaliador 1).

### PE — Potencial de Escala (Mercado)
- **Objeção:** A escala se apoia em **efeito de rede que só existe na v2**
  (compartilhamento de manuais) e em "custo marginal ~zero" que não se sustenta
  enquanto bolsistas humanos produzem verbetes um a um. O motor de aquisição não
  está definido: é PLG (faz sentido p/ autônomo) ou venda consultiva (faz sentido
  p/ PME)? Isso segue do segmento — que está indefinido. Como escala, concretamente?
- **Risco de nota:** **2–3.** Tese de escala plausível no longo prazo, mas o
  mecanismo nos 12 meses é vago e contradiz o custo de curadoria humana.
- **O que falta:** (a) modelo de aquisição coerente com o segmento; (b) curva de
  custo marginal real (infra + IA por consulta — o pitch tem R$7k IA / R$4,3k
  infra, dá pra derivar custo/consulta); (c) gatilho e cronograma do efeito de
  rede (quando a v2 liga, sob qual parecer jurídico).
- **Prioridade:** **Alta.**

### MN — Modelo de Negócio (Consistência ⚠ peso 2x · eliminatório < 2)
- **Objeção:** **Não existe modelo de negócio decidido.** Pricing em aberto, sem
  unit economics, sem CAC, sem LTV, sem projeção de receita. O ticket R$300–800
  é hipótese solta. Para um critério **eliminatório**, isto é o furo mais
  perigoso: um avaliador rigoroso pode dar **1–2 aqui e eliminar o projeto.** Como
  o negócio ganha dinheiro, com que margem, e por que é sustentável?
- **Risco de nota:** **2** (perigo real de 1). É o gargalo eliminatório.
- **O que falta:** (a) modelo de cobrança definido (assinatura/empresa? por
  técnico? por OS? freemium?); (b) unit economics com custo/consulta de IA real;
  (c) CAC estimado por canal e payback; (d) projeção de receita 12–36 meses
  amarrada ao SOM (30–100 clientes); (e) sensibilidade a churn.
- **Prioridade:** **Crítica.**

### CF — Cronograma Físico (Consistência ⚠ peso 2x)
- **Objeção:** O roadmap (Slide 16) tem 4 trimestres com entregas, o que é bom —
  mas é **superficial e quase 100% técnico-acadêmico**. Não há marcos
  **comerciais** (quando começa a prospecção paga, metas de clientes, validação
  de pricing). O T4 menciona "prospecção de 3–5 clientes" como item solto, sem
  funil nem responsável. O time enxuto (founder + júnior 20h) consegue entregar
  gerador **e** subestação + IA + piloto em 12 meses? Onde está o caminho crítico?
- **Risco de nota:** **3.** Estrutura existe, falta granularidade e a dimensão
  comercial; risco de execução do time enxuto subdimensionado.
- **O que falta:** (a) cronograma com marcos verificáveis mensais/quinzenais e
  dependências; (b) inserir trilha comercial (descoberta → pricing → primeiros
  contratos); (c) caminho crítico e folgas; (d) alocação de quem faz o quê.
- **Prioridade:** **Alta** (peso 2x; compõe o eliminatório).

### O — Orçamento (Consistência ⚠ peso 2x)
- **Objeção:** Orçamento detalhado (Slide 17), mas com **dois buracos fatais para
  a coerência:** (1) **nenhuma rubrica para o reforço comercial** que os dois
  avaliadores exigiram — o orçamento desmente a intenção de fortalecer mercado;
  (2) **nenhuma rubrica de PI** (registro de marca/software, parecer jurídico).
  Além disso, R$50k dos R$135k são bolsas CNPq **externas e condicionais** à
  parceria UFCG não-formalizada — se não vierem, o projeto perde a curadoria da
  base. O orçamento está alinhado a cronograma e equipe? Não totalmente.
- **Risco de nota:** **3.** Bem-estruturado nos recursos diretos, incoerente com
  as próprias prioridades de negócio e dependente de verba externa condicional.
- **O que falta:** (a) rubrica/contrapartida para perfil comercial (mesmo que
  advisor + pequena verba de growth/pesquisa de mercado); (b) rubrica de PI
  (INPI marca + software, ~baixo custo); (c) deixar explícito o plano se as
  bolsas CNPq não saírem; (d) amarrar cada rubrica a um marco do cronograma.
- **Prioridade:** **Alta** (peso 2x; compõe o eliminatório).

### DT — Domínio Técnico da equipe (Equipe)
- **Objeção:** Domínio técnico do founder é claro, mas **concentrado nele** —
  risco de bus factor 1. O segundo dev é júnior, 20h/semana. O domínio de IA
  (retriever híbrido, pgvector, avaliação de qualidade) está **terceirizado para
  um mestrando da UFCG que ainda não existe** (parceria condicional). Quem garante
  a competência de IA se a UFCG não vier?
- **Risco de nota:** **3–4.** Founder competente e stack coerente; perde por
  concentração e por a expertise de IA depender da parceria condicional.
- **O que falta:** (a) evidência do track record do founder (GitHub, entregas);
  (b) plano de mitigação de bus factor; (c) confirmar quem detém a expertise de
  IA independentemente da UFCG.
- **Prioridade:** Média (consolidar).

### CE — Capacidade de Execução (Equipe)
- **Objeção:** **Lacuna comercial não endereçada** — o ponto nº1 dos dois
  pareceres segue 100% aberto: nenhuma pessoa real de mercado/vendas/estratégia.
  Soma-se a isso time enxuto e dependência de contratações futuras (bolsistas +
  2º dev) ainda não formalizadas. A capacidade de **executar a parte de negócio**
  (que é justamente onde a proposta é fraca) não está coberta por ninguém.
- **Risco de nota:** **2–3.** Capacidade técnica de execução existe; capacidade
  comercial de execução é zero hoje.
- **O que falta:** (a) advisor/mentor comercial com **carta de intenção** antes
  de submeter (caminho mais rápido em 7 semanas); (b) cronograma de contratações
  com gatilhos; (c) demonstrar que o founder tem banda para a frente comercial ou
  que ela está delegada.
- **Prioridade:** **Crítica** (gap explícito dos 2 avaliadores; compõe E e
  pressiona CP).

---

## Bloco transversal — Propriedade Intelectual (jurídica)
> Não é subcritério pontuado isolado, mas **dobra em CP, M e PDT** e foi cobrança
> direta do Avaliador 1. Estado atual: **ZERO**.
- **Objeção:** Setor competitivo e tech-based sem **nenhuma** proteção: marca
  "Lumio"/"GerenciaLume" não depositada no INPI; software não registrado; e a
  base autoral NBR — apresentada como "propriedade do projeto" e principal moat —
  **não tem cessão de direitos dos bolsistas** que a produzirão. Se um bolsista
  detém direito autoral sobre o verbete que escreveu, o moat não é seu.
- **O que falta:** (a) depósito de marca no INPI (custo baixo, sinal forte);
  (b) registro de programa de computador no INPI; (c) cláusula de cessão de
  direitos/PI nos termos de bolsa e no convênio UFCG; (d) estratégia de PI de 1
  página (o que proteger, como, quando) — fecha o parecer do Avaliador 1.
- **Prioridade:** **Alta** (barata de resolver, alto retorno de percepção,
  cobrança explícita).

---

## TOP 5 ataques mais perigosos (ordenados por dano à nota)
1. **MN sem modelo de negócio/pricing/unit economics** — atinge o critério
   **eliminatório** (CP, peso 2x). Risco de nota 1–2 → eliminação. *O furo nº1.*
2. **Equipe comercial inexistente (abstrata)** — gap explícito dos 2 avaliadores;
   derruba CE e pressiona CP. Não evoluiu desde a Fase 1.
3. **Beachhead indefinido (autônomo/MEI × PME)** — incoerência que contamina FV,
   PE, MN e GTM; o produto v1 nem atende o autônomo. Derruba M e a coerência (CP).
4. **Circularidade da UFCG** — o moat (base autoral) e parte de equipe/impacto
   dependem de uma parceria condicional a ganhar o próprio edital. Atinge PDT
   (peso 2x em S), EX, DT.
5. **PI = zero** — sem registro e com base autoral não assegurada; barato de
   resolver, mas hoje é munição direta em CP, M e PDT.

---

## Backlog priorizado (vira as próximas sessões)
1. **[Crítica · MN]** Definir modelo de negócio: cobrança, unit economics com
   custo/consulta de IA real, CAC/payback por canal, projeção de receita 12–36m.
   → `04-consistencia/MN.md`
2. **[Crítica · GTM/M]** **Decidir beachhead** (recomendação: PME de geradores) e
   construir GTM: posicionamento, canais, funil, pricing inicial. → `03-mercado/GTM.md`
3. **[Crítica · CE]** Conseguir advisor/mentor comercial com **carta de intenção**
   antes de submeter; desenhar plano de contratações com gatilhos. → `05-equipe/CE.md`
4. **[Alta · O]** Refazer orçamento: incluir rubrica comercial + rubrica de PI;
   explicitar plano se bolsas CNPq não saírem; amarrar rubricas a marcos.
   → `04-consistencia/O.md`
5. **[Alta · PI jurídica]** Estratégia de PI de 1 página + iniciar depósito de
   marca/software no INPI + cláusula de cessão de direitos. → `06-pi-juridico/`
6. **[Alta · PDT]** Quebrar a circularidade UFCG: carta de anuência de professor
   + Plano B para a base autoral. → `01-solucao/PDT.md`
7. **[Alta · FV]** 5–10 entrevistas de descoberta com o ICP + carta(s) de intenção
   de compra. → `03-mercado/FV.md`
8. **[Alta · PE]** Motor de aquisição coerente com o segmento + curva de custo
   marginal + gatilho do efeito de rede. → `03-mercado/PE.md`
9. **[Alta · CF]** Cronograma granular com marcos comerciais + caminho crítico.
   → `04-consistencia/CF.md`
10. **[Baixa · EDD/PI/EX/DT]** Consolidar evidências já fortes: separar
    GerenciaLume×Copiloto, ancorar números no ledger, mitigar bus factor.
