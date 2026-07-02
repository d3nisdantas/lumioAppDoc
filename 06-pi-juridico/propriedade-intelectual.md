# PI · Propriedade Intelectual (LACUNA apontada)

## Pergunta-âncora (o que faz um avaliador dar 5)
> Que ativos proteger e como: marca (INPI), software (registro de programa de
> computador INPI), base autoral NBR 5410 (direito autoral), segredo de negócio.
> Estratégia, custo, prazo.

> ⚠ **Tudo neste arquivo é insumo a validar com advogado** na revisão externa —
> os pontos que exigem parecer jurídico formal estão marcados explicitamente.

---

## ✅ Decisões travadas (sessão grill 2026-07-02)

1. **Titularidade hoje:** não existe CNPJ. O projeto opera na pessoa física do
   founder (CPF). Marca e software serão depositados no CPF do founder agora e
   **cedidos/integralizados para a PJ** quando ela for constituída — precisa de
   instrumento formal de cessão nesse momento (⚠ exige advogado).
2. **Marca:** depositar só **"Lumio"** (marca-guarda-chuva), como **marca
   nominativa** (sem logo, pois ainda não existe identidade visual definida).
   "GerenciaLume" fica como nome de produto, sem depósito próprio por ora.
3. **Software:** registrar no INPI só o **GerenciaLume** agora (código real,
   estável, 100% escrito pelo founder — titularidade limpa). O **Copiloto** é
   greenfield (objeto financiado pela subvenção); seu registro fica como
   **marco do cronograma de 12 meses**, quando o código estabilizar.
4. **Base autoral NBR 5410:** 100% trabalho futuro dos bolsistas (nada escrito
   hoje). Regra de redação travada: verbetes são **comentário/síntese original**
   (explicação em palavras próprias, com referência ao artigo/seção da norma),
   **nunca cópia/trecho da norma**. Isso afasta risco de violação de direito
   autoral da ABNT (que detém os direitos sobre o texto da NBR 5410) e é também
   o que gera valor real do produto.
5. **Arquitetura RAG:** protegida como **segredo de negócio** (código, prompts,
   parâmetros de ranking/tuning). Publicação acadêmica do mestrando (bolsa
   CNPq) fica em **nível conceitual** (abordagem geral, metodologia de
   avaliação) — sem expor implementação. Precisa de cláusula de
   confidencialidade explícita no termo de bolsa definindo o que é publicável.
6. **Dados do piloto:** o piloto é a empresa do pai do founder (o founder
   trabalha nela hoje e vai abrir CNPJ própria, que prestará serviço para ela).
   Mesmo sendo relação familiar, **são duas pessoas jurídicas distintas** a
   partir do momento em que a PJ do founder existir — precisa de cláusula
   formal de uso de dados (titularidade, finalidade, base legal LGPD) entre as
   duas partes antes de usar dados de OS para treinar/ajustar o Copiloto.
   *(Nota de escopo: a relação familiar do piloto em si — implicação para
   EDD/GTM como "prova de tração" — não é tratada aqui por decisão do founder;
   fica fora do escopo deste tópico.)*
7. **Contrato do dev PJ (Copiloto):** ✅ já existe, com **cláusula de cessão de
   PI explícita**. Resolvido, sem ação pendente.
8. **Timing/orçamento:** marca (Lumio) + software (GerenciaLume) depositados
   **antes de submeter (10/08)**, com recurso próprio — custo baixo, sinaliza
   ação já iniciada (não só planejada) no dossiê. Cláusulas de cessão dos
   termos de bolsa, cláusula de dados do piloto e qualquer parecer jurídico
   mais amplo ficam para a **verba do edital** (§7.1 financia serviços PJ de
   assessoria jurídica e registro de PI), pois dependem de contratações que só
   acontecem se o projeto for aprovado.

---

## C1 · Inventário de ativos

| Ativo | Tipo de proteção aplicável (Brasil) | Quem detém hoje | Risco se não proteger | Ação |
|---|---|---|---|---|
| **Marca "Lumio"** | Registro de marca (INPI, nominativa) | Ninguém formalmente — uso de fato pelo founder | Terceiro registra antes e impede o uso do próprio nome do projeto | Depositar **antes de 10/08**, CPF do founder, 1 classe |
| **Marca "GerenciaLume"** | Registro de marca (INPI) — adiado | Uso de fato pelo founder | Baixo no curto prazo (nome de produto, não da empresa) | Reavaliar depósito quando/se virar nome comercial relevante |
| **Código-fonte GerenciaLume (~70% MVP)** | Direito autoral automático + registro de programa de computador (INPI) para prova de autoria/data certa | Founder (100% autoria própria, sem terceiros) | Sem registro, defesa de autoria em disputa depende só de outras provas (commits, etc.) — mais fraco | Registrar **antes de 10/08** |
| **Código-fonte Copiloto (RAG)** | Direito autoral automático (nasce com a criação); registro adiado; segredo de negócio para arquitetura/parâmetros | Dev PJ contratado, **com cessão de PI já contratual** para o founder/PJ | Baixo — cessão já resolvida; risco residual é só a divulgação acadêmica (ver item 5 abaixo) | Registrar no INPI como marco do cronograma (pós-estabilização); manter parâmetros/prompts fora de qualquer publicação |
| **Base autoral NBR 5410 (verbetes)** | Direito autoral (obra de comentário original) — **não** é o texto da norma (esse é da ABNT) | Ninguém ainda — trabalho 100% futuro dos bolsistas | Sem cláusula de cessão no termo de bolsa, o bolsista-autor pode reter direitos sobre o que escreveu; risco adicional se verbetes reproduzirem trecho da norma (violação de direito autoral da ABNT) | Cláusula de cessão de direitos no termo de bolsa (⚠ exige advogado) + regra editorial de "síntese original, nunca cópia" já travada |
| **Arquitetura/pipeline RAG (busca híbrida)** | Segredo de negócio (não há patente de software "pura" no Brasil — só como parte de processo técnico com efeito técnico, caso raro e caro) | Founder + dev PJ (sob cessão contratual) | Divulgação (ex.: dissertação de mestrado completa, repositório público) elimina a proteção por segredo | Cláusula de confidencialidade no termo de bolsa do mestrando; código do pipeline em repositório privado |
| **Dados do piloto (OS, histórico de manutenção, interações com o Copiloto)** | Proteção contratual (cláusula de uso/titularidade de dados) + LGPD (base legal para tratamento) | Empresa do pai do founder (dona dos dados operacionais hoje) | Sem cláusula, uso dos dados para treinar/ajustar o Copiloto não tem base legal documentada entre as duas PJs (a do pai e a futura do founder) — expõe a risco de disputa e a não conformidade LGPD | Redigir cláusula específica de dados/LGPD entre as duas entidades (⚠ exige advogado) antes de usar dados reais para treinar o modelo |

---

## C2 · Estratégia INPI

### Ordem de prioridade (o que fazer primeiro e por quê)

| Ordem | Item | Quando | Titular no depósito | Por quê primeiro/depois |
|---|---|---|---|---|
| 1 | Marca **"Lumio"** (nominativa, 1 classe) | Antes de 10/08 | CPF do founder | Barato, rápido de protocolar, sinal forte e imediato de PI protegida no dossiê — responde direto ao parecer dos avaliadores |
| 2 | Registro de programa de computador **GerenciaLume** | Antes de 10/08 | CPF do founder | Código já existe e é estável; processo simples (sem exame de mérito), gera prova de autoria com data certa |
| 3 | Cláusula de cessão de PI no **termo de bolsa** (base autoral + eventual código produzido por bolsistas) | Com a verba do edital, antes do 1º bolsista começar | — (cláusula contratual, não depósito) | Só existe contraparte (bolsista) se o projeto for aprovado |
| 4 | Cláusula de **dados do piloto** (LGPD) entre a empresa do pai e a futura PJ do founder | Com a verba do edital / assim que a PJ do founder existir | — (cláusula contratual) | Depende da constituição da PJ do founder |
| 5 | Registro de programa de computador **Copiloto** | Marco do cronograma de 12 meses (pós-estabilização do RAG) | PJ do founder (se já constituída) ou CPF, a definir | Código ainda não existe de fato hoje; registrar cedo travaria uma versão que será obsoleta |
| 6 | Cessão formal de marca + software do **CPF do founder para a PJ** | Assim que a PJ for constituída | — (instrumento de cessão/integralização de ativos) | Só é possível/necessário quando a PJ existir |

### Custo e prazo estimados (INPI)

| Item | Custo | Prazo | Fonte |
|---|---|---|---|
| Pedido de registro de marca, pessoa física, 1 classe, com desconto de 50% | **≈ R$ 440/classe** (R$ 880 sem desconto) | Proteção vale a partir do depósito; concessão final em média **8–18 meses** (pode chegar a 24 se houver oposição/exigência) | Ver `00-fontes/evidencias.md` — confirmar valor exato no e-INPI no momento do depósito |
| Registro de programa de computador (código de serviço 730/e-INPI) | **≈ R$ 185** | Certificado emitido rapidamente após conferência da documentação — dias a poucas semanas quando não há pendência | Ver `00-fontes/evidencias.md` — confirmar valor exato no e-INPI no momento do depósito |
| Cláusulas contratuais (termo de bolsa, cessão PJ, dados do piloto) | Não é taxa INPI — custo de assessoria jurídica, coberto pela subvenção §7.1 | Depende da disponibilidade do advogado contratado | Edital Centelha 3, §7.1 |

> ⚠ Os valores de taxa INPI acima vêm de fontes secundárias (escritórios
> especializados) cruzadas entre si, não do PDF oficial da tabela de
> retribuições (bloqueado para acesso automatizado nesta sessão). **Confirmar
> o valor exato diretamente no sistema e-INPI (gov.br/inpi) no momento do
> depósito**, antes de programar o desembolso.

### O que é segredo de negócio (não registrar) vs. o que registrar

- **Registrar:** marca (Lumio); código-fonte já estável (GerenciaLume, depois
  Copiloto); base autoral NBR 5410 nasce protegida por direito autoral
  automaticamente (registro de obra literária no INPI/Biblioteca Nacional é
  opcional, não prioritário — o valor está mais na cessão contratual dos
  bolsistas do que no registro formal do texto).
- **Manter como segredo de negócio (não registrar/publicar):** arquitetura
  detalhada do pipeline RAG, prompts, parâmetros de ranking/tuning, lógica de
  scoring de confiança das respostas. Depende de as pessoas com acesso
  (dev PJ, mestrando, founder) estarem sob cláusula de confidencialidade —
  sem isso, segredo de negócio não se sustenta juridicamente.

### Cláusulas de cessão de PI a inserir nos contratos (⚠ exige advogado)

1. **Termo de bolsa (CNPq/FAPESQ, recrutamento pelo coordenador):** cláusula de
   cessão de direitos patrimoniais sobre verbetes/conteúdo produzido +
   confidencialidade sobre o pipeline RAG + regra de que dissertação/artigo
   publicável fica em nível conceitual (sem expor implementação).
2. **Contrato entre a empresa do pai (piloto) e a futura PJ do founder:**
   cláusula de titularidade/uso de dados operacionais (OS, histórico), base
   legal LGPD para tratamento, finalidade restrita (melhoria do Copiloto),
   e regra de anonimização de dados de técnicos quando aplicável.
3. **Instrumento de cessão CPF → PJ do founder:** quando a empresa for
   constituída, formalizar a transferência/integralização da marca e dos
   registros de software depositados no CPF para a PJ (⚠ evita disputa
   futura, especialmente se houver sócios).
4. **Contrato do dev PJ:** ✅ já resolvido — cláusula de cessão de PI já
   existe no contrato assinado.

### O que exige advogado (não fazer sozinho)

- Redação das cláusulas de cessão (termo de bolsa, dados do piloto, cessão
  CPF→PJ).
- Definição da(s) classe(s) INPI corretas para a marca "Lumio" (recomendação
  inicial: classe 42 — NCL, software/SaaS/serviços de tecnologia — a validar).
- Qualquer decisão sobre se vale registrar a base autoral como obra literária
  (opcional) ou se a cessão contratual já é suficiente.
- Constituição da PJ do founder e modelo societário (impacta quem é o titular
  final de tudo acima).

---

## Fontes
(registrar em `00-fontes/evidencias.md`)
- Sessão grill 2026-07-02 (Track C): decisões de titularidade, marca, software,
  base autoral, segredo de negócio, dados do piloto — founder.
- Taxas e prazos INPI (marca e programa de computador): ver ledger de
  evidências — fontes secundárias, **confirmar valor exato no e-INPI antes do
  desembolso**.
- Edital Centelha 3, §7.1 — subvenção financia registro de PI e assessoria
  jurídica PJ.
