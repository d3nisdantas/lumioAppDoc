# BRIEFING pivot-EV — Consistência (MN · nota p/ CF)

> Ler antes: `CLAUDE.md`, `INDEX.md`, `../_PIVOT-EV-2026-07-02.md`.
> Regra de ouro: **unit economics de geradores permanecem** (ARPA R$120, churn 5%,
> LTV/CAC, SOM 10→125). NÃO refazer. O pivot mexe no **scoring de verticais (B3)** e
> na **sequência de expansão**, não no núcleo financeiro.

---

## MN.md — Modelo de Negócio

### Preservar integralmente
- B1 (Pricing Free + Equipe R$40/assento), B2 (Unit economics, `unit-economics.csv`),
  os 2 lembretes do founder (free no CAC + custo-de-servir real).

### Editar — B3 (Scoring de verticais), a mudança central
1. **Desmembrar "Solar / fotovoltaico + EV charging" (linha 179).** Estavam agrupados
   e penalizados em Fit CMMS e reuso de base ("exige NBR 16690 NOVA, não reusa 5410").
   Isso vale para **solar**, NÃO para EV:
   - **Nova linha "Instalação/adequação EV":** EV é instalação de baixa tensão →
     **REUSA a NBR 5410** + adiciona **NBR 17019** (norma nova, foco, moat). Perfil ≈
     "Instalações prediais": **Fit Copiloto/reuso de base ALTO** (🟩–🟢), **Fit CMMS
     BAIXO** (🟧2 — é projeto/instalação, não manutenção recorrente; coerente com o
     caminho leve). Mercado alto/crescente (🟩–🟢), Dor/campo alta (instalador decide
     no local), WTP `[VALIDAR]`.
   - **Manter "Solar/fotovoltaico" separada** como hipótese posterior (NBR 16690,
     baixo reuso) — não confundir com EV.
2. **Reposicionar a sequência de expansão (B3, itens 193–207):**
   - 1. Geradores — beachhead (em curso). *(inalterado)*
   - 2. **Instalação/adequação EV — TRILHA DE APROFUNDAMENTO H2 (HIPÓTESE-A-VALIDAR).**
     Substitui subestação. Forças: reuso NBR 5410 + norma nova 17019 (moat) + lab de
     ~50 condomínios + tailwind EV + abre o TAM (CNAE 4321-5). Fraqueza: **dor não
     validada** → de-riscada pelo **gate de validação H1** (5–10 instalações-lab +
     plano B de entrevistas). Marcar honestamente como hipótese, não certeza.
   - 3. Solar / demais — hipóteses posteriores.
3. **Remover subestação como "trilha comprometida / de-riscada por cliente concreto"
   (linhas 180, 190, 195–197).** O de-risco não existe mais (1 único cliente-final +
   concorrente robusto). Rebaixar subestação a "descartada nesta fase" ou removê-la
   do ranking de expansão.

### Editar — nota de unit economics do segmento EV
- Adicionar que a vertical EV terá **mini unit-economics própria após validação** (WTP
  do pagador de instalação = desconhecida). Marcar `[VALIDAR]`. NÃO mexer no modelo
  de geradores por causa disso.

### Guardar o caminho leve (não contradizer CF/O)
- Deixar explícito no MN que instalação = **tipo especial de OS** (não módulo de obra),
  para o pricing por assento continuar coerente (não vira produto de projeto separado).

---

## Nota para CF.md (quando aquela sessão iniciar — sem briefing dedicado)
O `CF.md` atual está estruturado em **subestação H2** (linhas 7–25). Ao ser
trabalhado, deve nascer já com: (a) H2 = **instalação/EV** (não subestação); (b) o
**gate de validação H1** (~mês 4–5) como marco físico entre validar e aprofundar;
(c) caminho leve (tipo-de-OS, não ERP de obra); (d) divisão de equipe do `_PIVOT §3.7`.
Ver `../_PIVOT-EV-2026-07-02.md §9`.

## Fontes (`00-fontes/evidencias.md`)
- NBR 17019 (título/ano/status). `[FONTE PENDENTE]`
- Base de norma para EV: NBR 5410 (reusada) + NBR 17019 (nova). Solar seria NBR 16690.
