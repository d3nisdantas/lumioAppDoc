# PI · Potencial de impacto socioambiental positivo

## Pergunta-âncora (o que faz um avaliador dar 5)
> Impacto medível: redução de acidentes elétricos, conformidade NBR 5410, menos
> incêndios. Ligar a métricas do piloto.

## Decisões de enquadramento (grill 2026-06-25 · Track D)
- **Espinha causal mediada (defensável):** o Copiloto **não salva vidas
  diretamente**; ele eleva **conformidade e adesão a procedimento de segurança**
  (LOTO, citação de norma, nível de confiança). As **840 mortes/ano** são
  **contexto de relevância**, não KPI de entrega. O KPI mensurável é o **proxy
  controlável** (% de OS com LOTO / citação de norma). → evita o ataque "vínculo
  copiloto→vida salva é narrativo" (`99-red-team/gaps.md`, PI).
- **Duas espinhas de valor/impacto:**
  - **A · Segurança + agilidade (Copiloto):** conformidade/LOTO + **resolução
    mais rápida de defeitos**.
  - **B · Digitalização/inclusão (CMMS de baixo custo):** especialização por
    nicho mais eficaz que generalistas + rastreabilidade + custo menor (via IA) +
    profissionalização do pequeno operador.
- **Impacto negativo declarado + mitigado** (o edital exige; é o que dá nota
  alta): (1) erro/viés do modelo, (2) pegada de IA, (3) deskilling do técnico.
  O risco de "deslocamento de mão de obra júnior" é reposicionado como impacto
  **positivo** (inclusão produtiva).
- **Sem correlação ambiental forçada:** o único item de "Planeta" é a pegada de
  IA (negativo mitigado). Não se reivindica ganho ambiental por vida útil de
  equipamento (correlação não clara).
- **Circularidade UFCG dissolvida** (ver `01-solucao/PDT.md`): bolsas CNPq são
  concedidas ao projeto aprovado e não exigem convênio institucional. IES (ex.:
  UFCG) é **upside**, não pré-requisito. `*` marca o que é condicionado a vencer.

---

## Flourishing Business Canvas (versão pragmática)
> Cortes: Biophysical Stocks, Ecosystem Services, Value Co-Destruction (irrelevantes
> para SaaS em estágio inicial). Mantidos 13 blocos. `*` = planejado, **condicionado
> a vencer o Centelha**.

| Bloco | Conteúdo |
|---|---|
| 🎯 **Goals / Metas** | **Econômica:** 100–150 empresas pagantes em 36 meses; ARR ~R$180k; LTV/CAC ≥ 2,4×; sustentabilidade sem subvenção recorrente. · **Social:** elevar conformidade/segurança (% de OS com LOTO + citação de norma); formar técnicos (piloto + setor); incluir o júnior/autônomo numa operação profissionalizada. |
| 🧩 **Needs / Necessidades** | *Espinha A:* 840 mortes/ano por acidentes elétricos; intervenções sem seguir norma; diagnóstico lento e dependente de sênior. · *Espinha B:* 73% das empresas sem sistema de gestão; autônomo opera em caderno/WhatsApp/memória; plataformas generalistas cobrem mal o nicho; software de gestão caro/inacessível ao pequeno. |
| 👥 **Stakeholders** *(diretos)* | Técnicos/eletricistas (usuário); PMEs de manutenção (pagador) e autônomos; empresa-piloto (acordo assinado); bolsistas (DTI/EV elétrica + mestrando CC)*; núcleo: founder (CMMS+comercial), dev PJ, advisor B2B. |
| 🌐 **Ecosystem Actors** *(humanos influenciados, indiretos)* | Clientes finais das PMEs → instalações mais seguras; famílias/comunidade expostas → vítimas potenciais por trás das 840 mortes; reguladores/fiscalizadores (CREA, Bombeiros, MTE) → maior conformidade; seguradoras e concessionárias → menor sinistralidade; fabricantes de equipamentos → manuais indexados (semente de efeito de rede); categoria profissional → elevação do piso técnico. |
| 🤝 **Relationships / Relações** | B2B consultivo com a PME (pagador); formativo e de confiança com o técnico (usuário); co-desenvolvimento com a empresa-piloto; acadêmico com bolsistas/IES*; comunidade/conteúdo (grupos de geradores, YouTube). |
| 📡 **Channels / Canais** *(do GTM)* | Interno: WhatsApp + distribuidores de geradores; meio: referral + SEO; Free tier (freemium) como canal paralelo de entrada. |
| ⚙️ **Activities / Atividades** | Desenvolver o Copiloto RAG (retriever híbrido + pgvector + safety-check/LOTO + citação de fonte)*; curar a base autoral NBR 5410 (bolsistas)*; indexar manuais de fabricante*; **desenvolvimento de software do CMMS** (tronco geral — módulos de gestão); operação comercial (descoberta, onboarding, suporte). |
| 🧱 **Resources / Recursos** | Base autoral NBR 5410 — moat (curadoria/expansão)*; GerenciaLume (~70% MVP, +250 testes); equipe (founder, dev PJ, bolsistas*); bolsas CNPq (R$50k)* + subvenção (R$85,3k)*; empresa-piloto (validação + dados de impacto); modelos de IA commodity (~R$0,01–0,05/consulta). |
| 🔗 **Partnerships / Parcerias** | Empresa-piloto (acordo assinado); IES (ex.: UFCG) — *upside*: lab, orientação, talento*; CNPq/FAPESQ (bolsas)*; distribuidores de geradores (canal); advisor B2B (carta a formalizar). |
| 🛡️ **Governance / Governança** | LOTO obrigatório antes de orientar intervenção; toda resposta cita fonte + nível de confiança; human-in-the-loop (a IA nunca autoriza intervenção sozinha); cessão de PI nos termos de bolsa (assegura a base autoral) — *liga ao Track C*; privacidade/segurança do dado do cliente *(a detalhar)*. |
| 💎 **Value Co-Creation** *(tripé)* | *A:* diagnósticos com fonte citável; intervenções mais seguras; **resolução mais rápida de defeitos**. · *B:* gestão especializada por nicho mais eficaz que generalistas; rastreabilidade; menor custo (via IA); profissionalização do pequeno. · *Social:* formação do técnico (formativo, não substitutivo); inclusão produtiva do júnior/autônomo. |
| ✅ **Benefits / Benefícios** *(outcomes positivos)* | **Segurança:** maior adesão a LOTO/norma → redução de acidentes (impacto populacional de longo prazo; contexto das 840 mortes). · **Produtividade:** menos retrabalho/tempo administrativo → mais margem para a PME. · **Inclusão produtiva:** júnior/autônomo capacitado. · **Formalização/competitividade:** histórico digital → ganhar contratos / passar auditoria *[hipótese a validar no piloto]*. · **Formação de RH:** bolsistas + técnicos do piloto*. · **Regional:** emprego qualificado e inovação no NE *[upside com IES]*.* |
| ⚠️ **Costs / Custos** *(outcomes negativos + mitigação)* | **(1) Erro/viés do modelo em contexto crítico** → mitigação no produto: cita fonte + nível de confiança + LOTO + human-in-the-loop. · **(2) Pegada energética/carbono da IA** → mitigação: modelos commodity leves, RAG enxuto, ~R$0,01–0,05/consulta, sem treinar modelo próprio. · **(3) Dependência/deskilling do técnico** → mitigação: Copiloto **formativo** (explica e cita a norma), elevando o piso. · **Recurso público** (subvenção/bolsas): contrapartida = impacto social, formação e emprego qualificado. |

---

## Insumo bruto (síntese para a submissão)
O impacto positivo do Lumio opera em duas frentes complementares e mensuráveis:
**(A) segurança e agilidade** — o Copiloto eleva a adesão a procedimento (LOTO),
cita norma e fonte em cada diagnóstico, e acelera a resolução de defeitos,
endereçando o contexto das **840 mortes/ano** por acidentes elétricos (ABRACOPEL);
**(B) digitalização e inclusão** — o CMMS de baixo custo, especializado por nicho,
profissionaliza autônomos e PMEs (73% sem gestão), trazendo rastreabilidade,
produtividade e formalização. O impacto é medido pelo **proxy controlável** (% de
OS com LOTO/citação de norma) no piloto, não por promessa de vidas salvas. O
projeto declara e mitiga seus impactos negativos (viés de IA, pegada energética,
deskilling), com mitigações embutidas no próprio produto.

## Fontes
(registradas em `00-fontes/evidencias.md`: 840 mortes ABRACOPEL; 73% sem gestão
ABDI/SEBRAE; custo de IA por consulta; mecanismo de bolsas §6.1–6.3. Enquadramento
de circularidade: `01-solucao/PDT.md`.)
