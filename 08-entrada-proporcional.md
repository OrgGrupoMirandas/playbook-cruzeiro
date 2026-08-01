# Entrada Proporcional — quem chega no meio do ano

Quem entra no time depois de janeiro corre menos meses. Sem correcao, essa pessoa
disputaria as mesmas cabines (Suite 2.000) com metade do tempo — o que na pratica significa
ficar de fora antes de comecar.

A correcao ja existia no programa, mas so para os setores que comecaram em maio (o **×1,5**).
Este capitulo transforma aquilo em **formula unica**, valida para qualquer pessoa, em
qualquer mes de entrada.

---

## A formula

```
Multiplicador = 12 ÷ (meses de participacao no ano)
```

O multiplicador e aplicado **por cima** dos pontos da tabela do setor da pessoa —
exatamente como o ×1,5 ja funciona hoje para CS, Growth e COO.

| Entra em | Meses no ano | Multiplicador | Pontos brutos para a Suite (corte 2.000) |
|----------|--------------|---------------|------------------------------------------|
| Janeiro | 12 | **1,00** | 2.000 |
| Maio | 8 | **1,50** | 1.333 |
| Junho | 7 | **1,71** | 1.167 |
| Julho | 6 | **2,00** | 1.000 |
| Agosto | 5 | **2,40** | 833 |
| Setembro | 4 | **3,00** *(teto)* | 667 |
| Out–Dez | <= 3 | — | nao corre por cabine no ano (embarca pela Camada 1) |

> A linha de **maio = ×1,50** e a mesma regra que ja vale hoje para CS, Growth e COO.
> Nada muda para quem ja esta na corrida.

---

## As tres travas

### 1. Teto de 3,0
Nenhum multiplicador passa de 3,0. Sem essa trava, quem entra em dezembro teria ×12 e
poderia passar na frente de quem carregou o ano inteiro com um unico mes bom.

### 2. Piso de 4 meses
Entrou de **outubro em diante**: nao corre por cabine individual naquele ano.

- **Embarca como integracao** (Camada 1 do `10`), em cabine Interna — fora da corrida do ano
- Se o gatilho coletivo disparar, leva acompanhante como todo mundo
- No ano seguinte comeca a corrida cheia, com multiplicador 1,00

### 3. Regra do dia 15
- Entrou **ate o dia 15** do mes: aquele mes conta como mes de participacao
- Entrou **do dia 16 em diante**: a contagem comeca no mes seguinte

---

## Embarque e o piso de 1.000

O piso de embarque (`10`, Camada 1) e **1.000 pontos no placar, igual para todos** — nao precisa
de tabela por mes de entrada porque o multiplicador deste capitulo ja esta embutido nos pontos:
quem entra em setembro ganha ×3 por mes e alcanca os mesmos 1.000 fazendo o proprio trabalho.
Quem entra de outubro em diante (multiplicador 0) embarca como integracao, fora da corrida.

## Nota historica — corte coletivo (extinto em 31/07/2026)

A regra do "minimo de 200 pts para embarcar pelo coletivo" **morreu com as tres camadas**
(`10`): o embarque agora e garantido a todo contrato ativo. Este capitulo segue valendo
apenas para o **multiplicador de pontos** — que define cabine, nao embarque.

## Excecoes

| Caso | Multiplicador | Motivo |
|------|---------------|--------|
| Assistente de Vendas (`07`) | **1,00** | A regua de Pouco/Medio/Muito ja foi calibrada com valores finais |
| Bonus IA (`06`) | **1,00** | O teto e mensal (30 pts/mes) — quem entra depois ja tem menos meses para acumular |
| Penalidades (-50 pts) | **1,00** | Penalidade nao escala. Erro grave custa o mesmo para todo mundo |

---

## Saida e mudanca de funcao

| Situacao | O que acontece |
|----------|----------------|
| Desligamento | Perde a pontuacao e nao embarca (regra ja vigente) |
| Mudou de setor no meio do ano | Mantem os pontos acumulados; passa a pontuar pela tabela do setor novo. O multiplicador **nao** e recalculado — vale a data de entrada na empresa |
| Saiu do programa (ex. Cintia, Midiane 29/07) | Pontos congelados no placar historico; nao concorre a cabine |

---

## Exemplo — contratacao em agosto/2026

Closer contratado em 04/08/2026 (entrou antes do dia 15 → agosto conta).

- Meses de participacao: ago–dez = **5**
- Multiplicador: 12 ÷ 5 = **2,40**
- Vende R$4M liquidos em setembro: 40 pts (volume) × 2,40 = **96 pts**
- Precisa de **833 pts brutos** para a Suite (corte 2.000 ÷ 2,40)
- Piso de embarque: os mesmos 1.000 do placar — o multiplicador ja compensa a entrada tardia

---

> Duvida sobre multiplicador de alguem: Anthony decide (ultima instancia, regra 5 do `01`).
