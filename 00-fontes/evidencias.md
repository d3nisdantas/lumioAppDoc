# Evidências e Fontes (ledger compartilhado)

> Toda afirmação numérica/factual de qualquer tópico é registrada AQUI com fonte.
> Separar coleta de fonte da síntese evita números inventados — avaliadores
> exigem "dados consistentes". Formato por linha:
> `| afirmação | número | fonte (link/doc) | data acesso | usado em |`

| Afirmação | Valor | Fonte | Acesso | Usado em |
|---|---|---|---|---|
| Empresas ativas no setor (CNAE 43.21-5) | 332 mil | Econodata 2026 | — | M, GTM |
| % sem sistema de gestão | 73% | ABDI/SEBRAE | — | M, Impacto |
| Pesquisa de mercado própria — utilidade do copiloto nota 4–5 | 7 de 9 | `03-mercado/pesquisa.csv` | 2026-06 | FV, GTM, MN |
| Pesquisa própria — respondentes que atuam com geradores | 7 de 9 | `03-mercado/pesquisa.csv` | 2026-06 | GTM, FV |
| Pesquisa própria — disposição a pagar (indivíduo) | "Até R$30" (4); "Nada" (2); "R$31–80" (1); "R$200+" (2) | `03-mercado/pesquisa.csv` | 2026-06 | MN, FV |
| Pesquisa própria — formato de cobrança preferido | mensalidade fixa (4) > sob demanda (3) > por equipamento (1) | `03-mercado/pesquisa.csv` | 2026-06 | MN |
| ⚠ RESSALVA — viés de seleção da pesquisa | divulgada em grupo de educação sobre geradores; n=9 | `03-mercado/pesquisa.csv` | 2026-06 | usar como APETITE, não como dimensionamento de mercado |
| ⚠ Paradoxo do pagador na amostra | os 2 que pagariam R$200+ = 1 RT (achou dispensável, nota 2) + 1 funcionário (não decide compra) | `03-mercado/pesquisa.csv` | 2026-06 | MN, GTM |
| Bolsas Centelha — valor e mecanismo | até R$50.000 via Acordo FAPESQ↔CNPq (DTI/EV/SET), concedidas ao projeto aprovado | Edital Centelha 3, §6.1–6.3 | 2026-06 | O, EX, PDT |
| Subvenção econômica — teto e itens financiáveis | até R$85.333; pró-labore sócio ≤30%; serviços PJ (consultoria/plano de negócio/marketing/anúncios/registro de PI); material de consumo (software) | Edital Centelha 3, §7.1 (a–h) | 2026-06 | O, CE, MN, PI-jurídica |
| Custo de IA por consulta (modelos commodity via API) | R$0,01–0,05 | estimativa founder (DeepSeek/Qwen) | 2026-06 | MN — `[VALIDAR]` |
| Custo-de-servir fixo mensal (vector DB+hosting+monitor.) | R$400–800 | estimativa própria | 2026-06 | MN — `[VALIDAR]` |
| Custo-de-servir variável/usuário (pago / free) | R$2,50 / R$1,80 | estimativa própria (IA+infra) | 2026-06 | MN — `[VALIDAR]` |
| LTV / LTV-CAC (churn base 5%/mês, ARPA R$120) | LTV R$2.400; 2,4× (network), 11,1× (distrib.) | modelo próprio `unit-economics.csv` | 2026-06 | MN, GTM |
| CAC blended por ano (mix 80/20→30/70) | R$843 → R$608 → R$451 | modelo próprio | 2026-06 | MN |
| ARR run-rate anos 1–3 (10→40→125 empresas) | R$14,4k → R$57,6k → R$180k | modelo próprio (SOM-ancorado) | 2026-06 | MN |
| Conversão freemium Free→pago (premissa) | ~4%/ano a partir do ano 2 | premissa própria | 2026-06 | MN — `[VALIDAR]` |
| Base do teto de 30% do pró-labore | valor da subvenção (R$85.333) | Edital Centelha 3, §7.1.g (confirmado no texto) | 2026-07-02 | O |
| Valores unitários de bolsa (DTI/mestrado) | `[VALIDAR: tabela FAPESQ/CNPq do edital]` | edital — não localizado nesta sessão | 2026-07-02 | O |
| Founder — formação e experiência | Eng. Elétrica (UFCG); 10 anos eng. software embarcado | declaração do founder (grill) | 2026-07-02 | DT, CE |
| Founder — MVP construído solo | CMMS ~70% + 500+ testes; GitHub + deploy Railway | declaração do founder; repo/URL `[FONTE PENDENTE]` | 2026-07-02 | DT |
| Dev PJ — perfil | júnior, 1 ano, recém-formado; já na equipe (pago pelo founder) | declaração do founder | 2026-07-02 | DT, CE |
| Base autoral NBR — estado | 100% a construir (nenhum verbete pronto) | declaração do founder | 2026-07-02 | DT, PDT |
| Founder — dedicação ao Lumio | 15h/semana (mantém outro emprego) | declaração do founder | 2026-07-02 | CE, O |
| (adicionar...) | | `[FONTE PENDENTE]` | | |
