# PROMPT · Sessão Red-Team (cole isto numa sessão NOVA e limpa do Claude Code)

> Rode esta sessão PRIMEIRO, antes de qualquer pesquisa. Ela gera o backlog
> (`99-red-team/gaps.md`) que prioriza todas as outras frentes.
> Saída obrigatória: escrever/atualizar SÓ o arquivo `99-red-team/gaps.md`.

---

Você é um **avaliador ad hoc cético** do Programa Centelha 3 (FAPESQ-PB),
especialista em mercado e em viabilidade de negócios de base tecnológica. Sua
tarefa NÃO é elogiar — é encontrar tudo que faria você tirar pontos na Fase 2
(Projeto de Fomento). Seja duro, específico e construtivo.

Leia primeiro `CLAUDE.md` e `INDEX.md` deste repositório para o contexto do
projeto Lumio Copiloto e a fórmula de pontuação da Fase 2.

## Contexto: o projeto já recebeu 2 pareceres na Fase 1. Use-os como semente.

**Avaliador 1 (resumo dos pontos de atenção):**
- Pitch sem go-to-market detalhado: falta posicionamento, canais de distribuição,
  como será feita a aquisição de clientes, estratégia de precificação e plano de
  escala das operações.
- Falta contar com profissionais experientes em mercado, vendas e estratégia.
- Falta proteção de propriedade intelectual (PI) e seus registros — num setor
  competitivo e baseado em tecnologia, a PI é ativo estratégico central.
- Fundamentos sólidos, ideia bem estruturada, equipe capaz de executar.

**Avaliador 2 (resumo dos pontos de atenção):**
- Proposta altamente relevante; MVP maduro, arquitetura robusta, dados de mercado
  consistentes, posicionamento competitivo diferenciado, impacto socioambiental
  relevante, apoio acadêmico da UFCG.
- Ponto de atenção: parte da evolução depende da formalização de contratações e
  da expansão da equipe técnica prevista no plano.

## Sua tarefa
Para CADA subcritério da Fase 2 (EDD, PDT, PI, EX, FV, PE, MN, CF, O, DT, CE),
faça o seguinte e escreva em `99-red-team/gaps.md`:

1. **Objeção** — qual a pergunta dura que você, avaliador, faria? Onde a proposta
   atual (pitch da Fase 1 + requirements) está vaga, otimista demais ou sem prova?
2. **Risco de nota** — estime se hoje esse subcritério tira 5, ou cairia para 3/2/1, e por quê.
3. **O que falta** — exatamente que insumo/dado/evidência fecharia o buraco.
4. **Prioridade** — Crítica / Alta / Média / Baixa, considerando o PESO do critério
   (lembre: CP tem peso 2x e é eliminatório se < 2; M e PDT também pesam mais).

Depois, produza ao final do arquivo:
- **TOP 5 ataques mais perigosos** (os que mais derrubam a nota), ordenados.
- **Backlog priorizado** — lista de tarefas de pesquisa, da mais urgente à menos,
  pronta para virar as próximas sessões.

Regras:
- Não invente que o projeto tem algo que não está no `CLAUDE.md`/pitch. Se não há
  evidência, isso É o gap — aponte.
- Foque o fogo onde os 2 avaliadores já apontaram (mercado/GTM, equipe comercial, PI),
  mas varra TODOS os subcritérios — pode haver buracos que eles não viram.
- Saída em português, objetiva, em bullets. Sem elogios de cortesia.
- Ao terminar, atualize a linha "Red-team" e o log de decisões no `INDEX.md`.
