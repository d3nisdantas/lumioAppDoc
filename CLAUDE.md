# CLAUDE.md — Contexto do projeto (LER NO INÍCIO DE TODA SESSÃO)

> Este arquivo é a "memória de longo prazo" do projeto. Toda sessão de pesquisa
> lê este arquivo + o `INDEX.md` antes de começar. NÃO carregue todos os outros
> arquivos: leia só o `INDEX.md` e o(s) arquivo(s) do seu tópico.

## 1. O que é o Lumio Copiloto
CMMS (gestão de manutenção) especializado em manutenção elétrica, com um
**copiloto de IA embutido na Ordem de Serviço**. Arquitetura RAG: busca híbrida
sobre (a) contexto da OS, (b) base autoral de verbetes da NBR 5410 (propriedade
do projeto, produzida por bolsistas UFCG) e (c) manuais de fabricante indexados.
Toda resposta cita fonte, traz nível de confiança e exige LOTO antes de orientar
intervenção. Diferenciais: base autoral defensável, efeito de rede em manuais,
travas de segurança. Estado: ~70% do MVP de gestão pronto, +500 testes.
**Empresa-piloto: acordo de cooperação JÁ ASSINADO** (prova forte de tração).
**Parceria UFCG: AINDA NÃO formalizada** — será buscada SE o projeto vencer o
Centelha, pois é viabilizada pela verba de bolsas CNPq da premiação. ⚠ Risco de
circularidade: o moat da base autoral NBR e parte da equipe/impacto dependem
dessa parceria condicional. Mitigante a obter ANTES de submeter: carta de
anuência de professor/departamento da UFCG.

## 2. Onde estamos: Edital Centelha 3 (PB / FAPESQ) — FASE 2
- Classificado na Fase 1. Agora é o **Projeto de Fomento (Fase 2)**.
- Janela de submissão: **20/07 a 10/08/2026**.
- Execução do projeto contratado: até 12 meses.

## 3. Como a nota da Fase 2 é calculada (decorar isto)
`NOTA F2 = (S + M + E + 2*CP + I) / 6`
- **S** = (EDD + 2*PDT)/3   → Solução
- **I** = (PI + EX)/2        → Impacto socioambiental
- **M** = (FV + PE)/2        → Mercado
- **CP** = (MN + 2*CF + 2*O)/5 → Consistência da Proposta  ⚠ PESO DOBRADO
- **E** = (DT + CE)/2        → Equipe

⚠ **ELIMINATÓRIO:** nota < 2 em **CP** elimina o projeto.
Cada subcritério vale de 1 a 5.

## 4. Onde a proposta está FRACA (pareceres reais dos 2 avaliadores)
Ambos elogiaram solução, impacto e equipe técnica. As lacunas, TODAS em negócio:
1. **Go-to-market ausente** — sem posicionamento, canais, aquisição de clientes
   (CAC), estratégia de pricing nem plano de escala de operações.
2. **Equipe sem perfil comercial** — falta gente de mercado/vendas/estratégia.
3. **Propriedade Intelectual não protegida** — sem registro nem estratégia de PI.
4. (Aval. 2) Evolução depende de formalizar contratações/expansão da equipe.

→ **Regra de priorização:** a pesquisa sobre-investe em MERCADO (FV, PE, GTM),
CONSISTÊNCIA (MN, CF, O) e PI/jurídico. Solução e Impacto já estão fortes —
apenas consolidar evidências, não reabrir.

## 5. Regras para CADA sessão de pesquisa
1. Leia este `CLAUDE.md` + o `INDEX.md`. Não leia o repositório inteiro.
2. Trabalhe UM tópico por sessão. Escreva SÓ no arquivo de saída daquele tópico.
3. Toda afirmação numérica/factual → registre a fonte em `00-fontes/evidencias.md`
   (não invente números; se não achar, marque `[FONTE PENDENTE]`).
4. Ao terminar, atualize o status do tópico no `INDEX.md` e o log de decisões.
5. Saída = insumo bruto organizado (o founder escreve a submissão final).
6. Fim de tópico fechado = 1 commit (ver branches no INDEX).
