# Pontuacao — Growth (Neriton)

Inicio: Mai/2026 — pontos **×1,5** para compensar os 8 meses vs 12 do comercial.

> **Como ler as tabelas:** a coluna "Base" e o valor do playbook; o ×1,5 e aplicado **por cima** dela.
> A coluna "Recebe" ja e o numero final que entra no placar.

O Growth controla o **volume de entrada**. Nao faz sentido cobrar por receita — isso e papel do closer.

---

## Duas fontes, dois papeis (a partir de AGOSTO/2026)

| Fonte | O que mede | Papel na regua |
|-------|-----------|----------------|
| **Bitrix cat 0** (Inside Sales) | Topo do funil inteiro — onde o closer trabalha | **RESULTADO** |
| **Bitrix cat 21** (Julia) | O canal da Julia esta vivo? | **COMPORTAMENTO** |

---

## RESULTADO — leads/mes na cat 0

| Leads/mes | Base | **Recebe (×1,5)** |
|-----------|------|-------------------|
| < 250 (zona morta) | 0 | **0 pts** |
| 250 – 349 | 30 | **45 pts** |
| 350 – 499 (base) | 50 | **75 pts** |
| 500 – 699 (meta) | 75 | **113 pts** |
| >= 700 (supermeta) | 150 | **225 pts** |

## COMPORTAMENTO — Julia viva (cat 21)

| Condicao | Base | **Recebe (×1,5)** |
|----------|------|-------------------|
| cat 21 >= 400 no mes **e** sem queda > 30% vs mes anterior | 20 | **30 pts** |
| Abaixo de 400 **ou** queda > 30% | 0 | **0 pts** |

> As duas condicoes valem juntas: entregar 400 despencando de 700 nao pontua. O item existe para
> que a Julia nao morra em silencio enquanto a cat 0 se sustenta por outros canais.

---

## Por que a regua mudou (31/07/2026)

A regua antiga tinha **uma fonte so** — a cat 21 — com faixas calibradas em **maio**, que foi o
**pico** desse canal (988 leads). O que aconteceu com cada fonte:

| Mes | cat 0 | cat 21 |
|-----|-------|--------|
| Marco | 203 | 15 |
| Abril | 515 | **1.166** |
| Maio | 383 | 988 |
| Junho | 264 | 412 |
| **Julho** | **346** | **335** |

- A **cat 21 caiu 71%** de abril a julho. E mal existia em marco (15) — nasceu quando a Julia escalou.
- A **cat 0 ficou estavel** (203–515, media ~340).
- Em julho **elas se cruzaram**: 346 contra 335.

Com a regua antiga (zona morta <700, meta 1.500) o Growth ficava em **zona morta todo mes**, por
qualquer das duas fontes. Um KPI que ninguem alcanca nao mede nada — so desmotiva.

Medir o Growth so pela cat 21 tambem era medi-lo por **um canal especifico** em vez do topo do
funil inteiro. Por isso a cat 0 virou o resultado e a cat 21 virou item de comportamento.

### Escala anterior — vale ate JULHO/2026

| Leads/mes (cat 21) | Base |
|--------------------|------|
| < 700 (zona morta) | 0 |
| 700 – 999 | 30 |
| 1.000 – 1.499 | 50 |
| 1.500 – 1.699 | 75 |
| >= 1.700 | 150 |

Junho e julho **nao sao recalculados** — mudanca de regua nao reescreve mes ja pontuado.

---

## COMPORTAMENTO — Sistemas

| Acao | Base | **Recebe (×1,5)** | Como e medido |
|------|------|-------------------|---------------|
| Uptime sistemas >= 99% | 20 | **30 pts** | 🔜 automatico (UptimeRobot) |
| Julia→Bitrix webhook cobertura >= 80% | 15 | **23 pts** | 🔜 automatico |
| Meta Ads rodando sem interrupcao | 15 | **23 pts** | 🔜 automatico (API Meta) |
| Entregas de sprint no prazo | 20 | **30 pts** | 🔜 automatico (GitHub) |
| Lead Hub sync 100% sem falha no mes | 20 | **30 pts** | manual |
| Brevo flows ativos e disparando (6 flows) | 20 | **30 pts** | manual |
| Disparos Brevo/Arara no prazo | 15 | **23 pts** | manual |
| Mes com TODOS comportamentais 100% | 30 | **45 pts** | derivado |

**Decisao de 31/07/2026:** os quatro primeiros itens passam a ser **medidos pelo coletor**, nao
lancados a mao. Os tres restantes seguem manuais ate existir fonte programatica.

> **Por que:** o comportamental vale ate 234 pts/mes e **nunca foi lancado uma unica vez**. O
> Neriton esta congelado em 295 pts desde maio. Com o resultado em zona morta pela regua antiga,
> o comportamental era a unica coisa que podia tira-lo da cabine Interna — e era justamente a
> parte que dependia de alguem digitar.

---

## Trava Growth

Se comportamento < 50% dos KPIs no mes, resultado pontua pela metade.

---

> Para detalhes sobre bonus financeiro, consultar o playbook-neriton.
