# PE · Potencial de escala

## Pergunta-âncora (o que faz um avaliador dar 5)
> Mecânica de escala: PLG sem força de vendas, efeito de rede em manuais (custo marginal ~0), distribuição nacional. SAM/SOM defensáveis.

---

## TAM / SAM / SOM

### Diagrama concêntrico

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 400" width="500" height="400">
  <!-- TAM -->
  <circle cx="250" cy="200" r="180" fill="#E3F2FD" stroke="#1565C0" stroke-width="2"/>
  <text x="250" y="60" text-anchor="middle" font-size="13" fill="#1565C0" font-weight="bold">TAM</text>
  <text x="250" y="78" text-anchor="middle" font-size="11" fill="#1565C0">332.833 empresas</text>
  <text x="250" y="94" text-anchor="middle" font-size="10" fill="#1565C0">CNAE 4321-5/00 · instalação e manutenção elétrica</text>
  <text x="250" y="108" text-anchor="middle" font-size="10" fill="#1565C0">Econodata mai/2026</text>

  <!-- SAM -->
  <circle cx="250" cy="215" r="120" fill="#BBDEFB" stroke="#1976D2" stroke-width="2"/>
  <text x="250" y="148" text-anchor="middle" font-size="13" fill="#1565C0" font-weight="bold">SAM</text>
  <text x="250" y="165" text-anchor="middle" font-size="11" fill="#1565C0">~8.750–10.000 empresas</text>
  <text x="250" y="181" text-anchor="middle" font-size="10" fill="#1565C0">CNAE 3313-9/01 · manutenção de geradores</text>
  <text x="250" y="196" text-anchor="middle" font-size="10" fill="#1565C0">e motores elétricos · ≤10 funcionários</text>

  <!-- SOM 36m -->
  <circle cx="250" cy="230" r="65" fill="#90CAF9" stroke="#1976D2" stroke-width="2"/>
  <text x="250" y="222" text-anchor="middle" font-size="11" fill="#0D47A1" font-weight="bold">SOM 36m</text>
  <text x="250" y="238" text-anchor="middle" font-size="10" fill="#0D47A1">100–150 empresas</text>

  <!-- SOM 12m -->
  <circle cx="250" cy="242" r="28" fill="#1976D2" stroke="#0D47A1" stroke-width="2"/>
  <text x="250" y="239" text-anchor="middle" font-size="10" fill="white" font-weight="bold">SOM 12m</text>
  <text x="250" y="253" text-anchor="middle" font-size="9" fill="white">10 empresas</text>
</svg>
```

---

### TAM — Total Addressable Market

**332.833 empresas** ativas no CNAE 4321-5/00 (Instalação e Manutenção Elétrica) no Brasil.
Fonte: Econodata, mai/2026. Confirma o número utilizado no pitch v1.1.

Este é o teto do mercado que o Lumio pode alcançar em 5–10 anos, quando o produto expandir de geradores para o eletricista e mantenedor em geral (Fase 3).

---

### SAM — Serviceable Addressable Market

**Critério de corte:** empresas com foco em **manutenção recorrente** de **equipamentos de grande porte** (geradores, subestações BT/MT, painéis industriais), com **2–10 funcionários**, onde existe separação entre pagador (dono/gestor) e usuário (técnico) — o que viabiliza o modelo B2B.

**CNAE específico:** 3313-9/01 — Manutenção e Reparação de Geradores, Transformadores e Motores Elétricos.

| Dado | Valor | Fonte |
|---|---|---|
| Total de empresas no CNAE 3313-9/01 | 12.489–12.509 | Econodata, mai/2026 |
| Estimativa com ≤10 funcionários (70–80%) | ~8.750–10.000 | Proporção Receita Federal 2024 |
| Estimativa focadas em geradores diesel (30–40%) | 2.600–4.000 | Triangulação (sem fonte direta) |

⚠ *Os percentuais de corte são estimativas declaradas — dado direto de faixa de pessoal por subclasse CNAE não disponível publicamente sem acesso interativo ao SIDRA/CEMPRE. Método declarado explicitamente na proposta.*

**SAM adotado na proposta:** ~8.750–10.000 empresas (CNAE 3313-9/01, ≤10 funcionários). O corte por tipo de equipamento (geradores + subestações BT/MT) é o critério qualitativo; o CNAE 3313-9/01 é o proxy quantitativo verificável.

---

### SOM — Serviceable Obtainable Market

| Horizonte | Meta | % do SAM | Observação |
|---|---|---|---|
| **12 meses (Centelha)** | **10 empresas** | 0,1% | Meta comprometida com a subvenção |
| 24 meses | 40–60 empresas | 0,5% | Pós-Centelha, com referral estruturado |
| **36 meses** | **100–150 empresas** | ~1–1,5% | SOM declarado na proposta |

**Premissas do SOM de 12 meses:**
- Empresa-piloto (acordo assinado) conta como cliente pagante a partir do **mês 1 pós-resultado** — o CMMS já está ~70% pronto e é o único CMMS do mercado focado no nicho de geradores.
- O Copiloto entra como upgrade competitivo no H2, aprofundando a proposta de valor.
- Time de vendas: founder + advisor B2B. Canal: WhatsApp técnicos + distribuidores de geradores.
- 10 empresas × 3 assentos × R$40/mês = **MRR R$1.200 ao fim do mês 12**.

---

## Mecânica de escala (o que o avaliador quer ver)

**1. Custo marginal próximo de zero em manuais.**
Cada manual de fabricante indexado serve todos os clientes que mantêm aquele modelo de equipamento. Na v2 (pós-Centelha), com compartilhamento voluntário entre clientes, cada novo manual enviado por um cliente enriquece a inteligência do copiloto para todos — crescimento de valor sem crescimento proporcional de custo.

**2. Base de conhecimento autoral que acumula valor.**
Os verbetes da NBR 5410 produzidos pelos bolsistas são propriedade do projeto (cessão nos termos de bolsa). Cada verbete adicionado aumenta a qualidade das respostas para todos os clientes, sem custo por usuário adicional.

**3. Efeito de rede em diagnósticos.**
O histórico acumulado de consultas (padrões de falha por modelo de equipamento) vira dado proprietário para calibrar o sistema ao longo do tempo — ativo que concorrentes entrantes não têm.

**4. CMMS como base de retenção.**
Empresa que migra histórico de OS, equipamentos e contratos para o GerenciaLume cria switching cost real. O Copiloto aprofunda esse lock-in ao associar diagnósticos ao histórico do equipamento.

---

## Contexto de mercado

- **Crescimento do setor:** Cummins Brasil registrou crescimento de +25% nas vendas de grupos geradores em 2024, com projeção de +20% para 2025. (Fonte: EaeMaq, abr/2025)
- **Rede de distribuição:** Stemac (50 operações em 24 estados) e Sotreq/Cat (50 filiais) somam mais de 100 pontos de atendimento — potencial canal de parceria para o Lumio.
- **Mercado global:** USD 26,86 bilhões em 2026, projeção USD 36,24 bi em 2031 (CAGR 6,18%). Brasil projetado como maior mercado da América do Sul. (Fonte: Mordor Intelligence, jan/2026)
- **Custo humano que justifica o produto:** 840 mortes por acidentes elétricos no Brasil em 2024. (Fonte: ABRACOPEL, Anuário 2025)

---

## Fontes
Registradas em `00-fontes/evidencias.md`:
- Econodata CNAE 4321-5/00: https://www.econodata.com.br/consulta-cnae/f4321500-instalacao-e-manutencao-eletrica (mai/2026)
- Econodata CNAE 3313-9/01: https://www.econodata.com.br/consulta-cnae/C3313901-MANUTENCAO-E-REPARACAO-DE-GERADORES-TRANSFORMADORES-E-MOTORES-ELETRICOS (mai/2026)
- Cummins +25% geradores 2024: https://eaemaq.com.br/noticias-do-mercado/com-vendas-de-grupos-geradores-em-alta-cummins-brasil-cresce-mais-de-25-em-2024-e-mantem-projecao-positiva-para-2025/ (abr/2025)
- ABRACOPEL acidentes 2024: https://abracopel.org/estatisticas/ (2025)
- Mordor Intelligence geradores: https://www.mordorintelligence.com/pt/industry-reports/diesel-generator-market (jan/2026)
- Stemac 50 operações: https://www.stemac.com.br (jun/2026)
- Sotreq 50 filiais: https://www.sotreq.com.br/energia-page (jun/2026)
