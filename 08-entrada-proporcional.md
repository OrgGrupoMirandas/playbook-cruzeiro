# Entrada Proporcional — quem chega no meio do ano

Quem entra no time depois de janeiro corre menos meses. Sem correcao, essa pessoa
disputaria a mesma cabine de 1.000 pts com metade do tempo — o que na pratica significa
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

| Entra em | Meses no ano | Multiplicador | Pontos "reais" para a Suite |
|----------|--------------|---------------|-----------------------------|
| Janeiro | 12 | **1,00** | 1.000 |
| Fevereiro | 11 | **1,09** | 917 |
| Marco | 10 | **1,20** | 833 |
| Abril | 9 | **1,33** | 750 |
| Maio | 8 | **1,50** | 667 |
| Junho | 7 | **1,71** | 583 |
| Julho | 6 | **2,00** | 500 |
| Agosto | 5 | **2,40** | 417 |
| Setembro | 4 | **3,00** *(teto)* | 333 |
| Outubro | 3 | — | so caminho coletivo |
| Novembro | 2 | — | so caminho coletivo |
| Dezembro | 1 | — | so caminho coletivo |

> A linha de **maio = ×1,50** e a mesma regra que ja vale hoje para CS, Growth e COO.
> Nada muda para quem ja esta na corrida.

---

## As tres travas

### 1. Teto de 3,0
Nenhum multiplicador passa de 3,0. Sem essa trava, quem entra em dezembro teria ×12 e
poderia passar na frente de quem carregou o ano inteiro com um unico mes bom.

### 2. Piso de 4 meses
Entrou de **outubro em diante**: nao corre por cabine individual naquele ano.

- Concorre **apenas pelo caminho coletivo**, com corte proporcional:
  `200 pts × (meses ÷ 12)` — outubro 50 pts, novembro 33 pts, dezembro 17 pts
- Se embarcar pelo coletivo, entra na **cabine Interna**
- No ano seguinte comeca a corrida cheia, com multiplicador 1,00

### 3. Regra do dia 15
- Entrou **ate o dia 15** do mes: aquele mes conta como mes de participacao
- Entrou **do dia 16 em diante**: a contagem comeca no mes seguinte

---

## O corte coletivo tambem e proporcional

O minimo de 200 pts do Caminho 2 tambem escala. Nao faz sentido exigir de quem tem 5 meses
o mesmo que se exige de quem tem 12.

```
Corte coletivo = 200 × (meses ÷ 12)
```

| Entra em | Corte coletivo |
|----------|----------------|
| Janeiro | 200 pts |
| Maio | 133 pts |
| Julho | 100 pts |
| Agosto | 83 pts |
| Setembro | 67 pts |
| Outubro | 50 pts |
| Novembro | 33 pts |
| Dezembro | 17 pts |

> As faixas de cabine (Suite / Premium / Vista Mar / Interna) **nao mudam**. Quem tem
> multiplicador chega nelas com menos pontos brutos — que e exatamente o objetivo.

---

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
- Precisa de **417 pts brutos** para a Suite, nao 1.000
- Corte do caminho coletivo: **83 pts**, nao 200

---

> Duvida sobre multiplicador de alguem: Anthony decide (ultima instancia, regra 5 do `01`).
