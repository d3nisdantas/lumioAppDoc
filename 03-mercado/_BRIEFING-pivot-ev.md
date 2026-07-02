# BRIEFING pivot-EV — Mercado (FV · PE · GTM)

> Ler antes: `CLAUDE.md`, `INDEX.md`, `../_PIVOT-EV-2026-07-02.md`.
> Sessão-worker: reabrir estes três arquivos e aplicar o pivot subestação→EV.
> Regra de ouro: **geradores (beachhead) e todos os números de SAM/SOM/UE ficam
> intactos.** O pivot só troca a *segunda vertical* (aprofundamento) e reposiciona
> a instalação/EV como o vetor que abre o TAM.

---

## FV.md — Fornecimento de valor
**Preservar:** os 3 segmentos atuais (autônomo, PME geradores=beachhead, grande
operador) e todo o cálculo de ROI de geradores.

**Editar:**
1. **Linha 32** (Segmento 2, dores): remover "risco de responsabilidade civil pesa
   especialmente em **subestações**". Substituir por trabalho elétrico de alta
   consequência de forma genérica (ex.: "…pesa em intervenções de alta consequência").
   Não ancorar mais valor em subestação.
2. **Segmento 1 (autônomo):** adicionar aos "jobs" que o autônomo cada vez mais faz
   **instalação** (não só manutenção) — incluindo adequação de infraestrutura e
   instalação de carregador EV. Isso conecta o autônomo à Linha 2 sem inventar
   segmento novo.
3. **Adicionar bloco novo (não uma 4ª coluna VPC completa ainda):** "Vertical de
   aprofundamento H2 — instalação/adequação EV". Descrever a dor HIPOTÉTICA
   (projetar conforme NBR 17019/5410, gerar laudo/ART, ativar na concessionária,
   provar segurança de uma nova carga elétrica) e marcar explícito **`[VALIDAR em H1]`**
   — a VPC completa deste segmento será construída após o gate de validação. NÃO
   afirmar WTP nem dor como fato (ver `_PIVOT §6`).

## PE.md — Potencial de escala (SAM/SOM)
**Preservar:** TAM 332.833 (CNAE 4321-5), SAM ~8.750–10.000 (CNAE 3313-9/01,
geradores), SOM 10→125. **NÃO inflar SAM com EV.**

**Editar:**
1. **Linha 53 e linha 65:** no critério de corte do SAM, remover "**subestações
   BT/MT**" da lista de equipamentos. Substituir por "geradores + instalações
   elétricas de baixa tensão" (mantendo o proxy CNAE 3313-9/01 para o número).
2. **Reforçar a ponte SAM→TAM:** hoje o TAM já é "Instalação **e** Manutenção
   Elétrica". Explicitar que a **instalação/EV é o vetor que abre o caminho do SAM
   (geradores) para o TAM (CNAE 4321-5, 332k)** — é a expansão natural, ancorada na
   base autoral NBR 5410 (que É a norma de instalação BT). Isso torna o TAM crível
   em vez de aspiracional.
3. **Efeito de rede / base autoral:** notar que a base NBR 5410+17019 produzida para
   EV é reaproveitável por todo o universo de instalação — reforça custo marginal ~0.

## GTM.md — Go-to-market
**Preservar:** beachhead geradores, bullseye atual (WhatsApp+distribuidores de
geradores = testar já), pricing, funil AARRR.

**Editar:**
1. **Canal novo para a Linha 2:** adicionar **condomínios / síndicos / administradoras**
   como canal de validação e acesso da vertical EV (os ~50 condomínios). Posicionar no
   anel "TESTAR JÁ" **apenas para o experimento de validação H1** — não como canal de
   receita de software ainda.
2. **Registrar os ~50 condomínios como evidência de ACESSO a mercado** (não WTP, não
   dor comprovada — ver `_PIVOT §6`).
3. Deixar claro que o motor de aquisição do software segue sendo geradores; EV é
   experimento de descoberta em H1.

## Fontes a registrar (`00-fontes/evidencias.md`)
- NBR 17019 (recarga de VE) — buscar ano/título oficial e status. `[FONTE PENDENTE]`
- Tamanho/crescimento do mercado de instalação de carregadores EV no Brasil (frota
  EV, projeções ABVE/similar). `[FONTE PENDENTE]`
- ~50 condomínios: registrar como pipeline de acesso (origem: carteira própria).
