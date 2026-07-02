# Handoff — Lumio Copiloto · Track C (PI jurídica)

**Data:** 2026-06-25
**Sessão anterior:** Track B completo (Pricing, Unit economics, Scoring) — commit `e427038`
**Próxima sessão:** Track C — `06-pi-juridico/propriedade-intelectual.md`
**Branch:** `feat/grill-modelo-negocio-20260623` (ou abrir `feat/pi-juridico` a partir de `develop`)
**Working dir:** `/home/denis/projects/lumioApp/lumio-centelha-f2`

---

## Contexto do projeto

**Lumio Copiloto** é um módulo de IA conversacional (RAG sobre NBR 5410 + manuais de
fabricante) integrado ao **GerenciaLume** (CMMS de manutenção elétrica, ~70% MVP),
voltado para eletricistas brasileiros em campo. Proposta em submissão ao **Centelha 3
(FAPESQ/PB), Fase 2**. Deadline: **10/08/2026** (buffer interno 03/08).

**Por que PI agora:** os dois avaliadores apontaram **"Propriedade Intelectual não
protegida — sem registro nem estratégia de PI"** como lacuna explícita. Hoje a PI do
projeto é **zero** (nada registrado). Fechar isto reforça o critério **CP (peso
dobrado, eliminatório)** e responde diretamente ao parecer.

**Leia obrigatoriamente antes de começar:**
1. `CLAUDE.md` — regras de sessão, lacunas da proposta, critérios de avaliação
2. `INDEX.md` — dashboard de progresso e log de decisões (§2)
3. `06-pi-juridico/propriedade-intelectual.md` — arquivo de saída (ver estado atual antes de escrever)

---

## Fatos travados que importam para a PI (não reabrir)

| Fato | Detalhe | Fonte |
|---|---|---|
| **Empresa-piloto** | Acordo de cooperação **JÁ ASSINADO** (gera dados do piloto = ativo) | CLAUDE.md §1 |
| **Base autoral NBR 5410** | Verbetes produzidos por **bolsistas UFCG** → ⚠ **cessão de PI nos termos de bolsa é crítica** (quem detém o direito autoral?) | CLAUDE.md §1 |
| **Parceria UFCG** | **NÃO formalizada** — condicional a vencer o Centelha. Mitigante a obter: carta de anuência | CLAUDE.md §1 |
| **Arquitetura RAG** | Busca híbrida sobre contexto da OS + base autoral + manuais indexados | CLAUDE.md §1 |
| **Marca** | "Lumio" (copiloto) e "GerenciaLume" (CMMS) — verificar disponibilidade no INPI | — |
| **Subvenção financia PI** | Edital §7.1 financia **registro de PI** e serviços PJ (advogado) → há rubrica para isto | `00-fontes/evidencias.md` |
| **Restrição de equipe** | Sem CLT pela subvenção (dev = PJ); cessão de PI deve constar nos contratos PJ e nos termos de bolsa | INDEX §2 (2026-06-23) |

---

## O que a próxima sessão deve entregar: Track C

**Arquivo de saída único:** `06-pi-juridico/propriedade-intelectual.md`

### C1 · Inventário de ativos (SEQ 1/2) → `[SONNET]`
> "Liste todos os ativos protegíveis (marca Lumio, código/MVP, base autoral NBR 5410,
> arquitetura RAG, dados do piloto). Para cada um: tipo de proteção aplicável no Brasil.
> Gere **mapa de ativos (tabela)**. Escreva no arquivo."

Cobertura mínima esperada: marca (Lumio + GerenciaLume), código/MVP (programa de
computador), base autoral NBR 5410 (direito autoral — com a questão da cessão dos
bolsistas), arquitetura/pipeline RAG (segredo de negócio vs. patente de software no
Brasil), dados do piloto (proteção contratual + LGPD). Para cada ativo: tipo de
proteção, quem detém hoje, risco se não proteger.

### C2 · Estratégia INPI (SEQ 2/2) → `[OPUS]`
> "Defina estratégia, ordem, custo e prazo de proteção via INPI (marca + registro de
> programa de computador), direito autoral da base e segredo de negócio. Marque o que
> exige advogado. Complete o arquivo. ⚠ valida com advogado na revisão externa."

Cobertura mínima: ordem de prioridade (o que registrar primeiro e por quê), custo e
prazo estimados por item (taxas INPI atuais), o que é segredo de negócio (não
registrar) vs. o que registrar, cláusulas de cessão de PI a inserir nos contratos PJ
e termos de bolsa, e marcar claramente os pontos que **exigem advogado** (a subvenção
§7.1 cobre isto). Toda afirmação de custo/prazo de INPI → registrar fonte em
`00-fontes/evidencias.md` (não inventar taxas).

---

## Dados de suporte disponíveis

| Arquivo | Conteúdo relevante |
|---|---|
| `CLAUDE.md` | Ativos do projeto (base autoral, RAG, piloto, UFCG condicional) |
| `00-fontes/evidencias.md` | Subvenção §7.1 financia registro de PI; ledger de fontes |
| `99-red-team/gaps.md` | "PI zero" como TOP-5 risco; ângulos de ataque do avaliador |
| `../lumio-copiloto_v2.md` | Pitch completo (descrição de produto e arquitetura) |

---

## Regras de sessão (do CLAUDE.md)

1. Leia `CLAUDE.md` + `INDEX.md` antes de começar. Não leia o repositório inteiro.
2. Trabalhe UM tópico por sessão. Escreva SÓ no arquivo de saída do tópico.
3. Toda afirmação numérica/factual (taxa INPI, prazo) → registre a fonte em
   `00-fontes/evidencias.md`. Se não achar, marque `[FONTE PENDENTE]`.
4. Ao terminar, atualize o status do tópico no `INDEX.md` e o log de decisões.
5. Saída = insumo bruto organizado (o founder escreve a submissão final).
6. ⚠ Tudo aqui é **insumo a validar com advogado** na revisão externa — marcar
   explicitamente o que exige parecer jurídico.

---

## Próxima ação imediata

```
Leia CLAUDE.md e INDEX.md. Depois leia 06-pi-juridico/propriedade-intelectual.md
(estado atual). Em seguida execute C1 [SONNET] (inventário de ativos) e, na sequência,
C2 [OPUS] (estratégia INPI). Registre toda taxa/prazo no ledger de evidências.
```
