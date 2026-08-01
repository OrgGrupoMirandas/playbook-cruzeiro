# Pontuacao — CS (Customer Success)

Aplicavel a: Kamila, Sara, Andrea
Inicio: Mai/2026 — pontos **×1,5** para compensar os 8 meses vs 12 do comercial.

> **Como ler a tabela:** a coluna "Base" e o valor do playbook; o ×1,5 e aplicado **por cima** dela.
> A coluna "Recebe" ja e o numero final que entra no placar.

---

## KPIs de pontuacao — regua vigente (a partir de AGOSTO/2026)

**A inadimplencia do placar e a MEDIA MOVEL de 3 meses** (mes corrente + 2 anteriores) — nao o
mes isolado. Motivo: 2,72% esta a 0,28pp da linha de 3%; no mes isolado, um cliente internado
zeraria o mes por puro ruido (Monte Carlo de 01/08: dispararia em 80% das simulacoes).

| Acao | Condicao | **Recebe (final, ×1,5 ja aplicado)** |
|------|----------|--------------------------------------|
| Inadimplencia SUPER | media 3m <= 2% **E venda propria >= R$1M no mes** | **225 pts** (substitui a meta) |
| Inadimplencia meta | media 3m <= 3% | **113 pts** |
| Conformidade | >= 95% no mes | **75 pts** |
| Venda ativa (token) | venda propria >= R$500k no mes, com media 3m <= 3% | **+25 pts fixos** |
| Entre 3% e 6% | — | 0 pts (so conformidade) |
| Zona morta | media 3m > 6% | **0 pts no mes inteiro** |

**Maximo: 325 pts/mes.** Venda e INDIVIDUAL (carteira propria e indicacao de cotista — nunca
lead de trafego/Julia); inadimplencia e conformidade seguem de time.

### Por que a venda e GATILHO, nao moeda (decisao de 01/08/2026)

**A comissao financeira ja paga a venda — e paga bem. Ponto nao remunera o que o dinheiro
remunera.** A venda destrava a supermeta (fechadura dupla: cobrar E vender) e um token fixo.
Nao existe ponto proporcional a volume: vender R$4M vale o mesmo token que R$500k — a
diferenca vai no bolso, via comissao.

O que cada peca faz:
- **Fechadura dupla da super:** os 225 que antes vinham so de cobrar agora exigem vender junto.
  Manter o que ja existe rende 188; o teto exige as duas maos.
- **Token de R$500k:** degrau de arrancada para quem nunca vendeu (Andrea) — sem inflar nada.
- **Trava:** media 3m acima de 3% e a venda nao conta NADA. Ninguem troca cobranca por venda.

## Nao existe pontuacao parcial de inadimplencia

Entre a meta e a zona morta a pontuacao e **zero**. Ou bate a meta (na media 3m), ou nao pontua.

A **conformidade pontua separado**: da para ganhar os 75 pts mesmo com a inadimplencia fora da meta.

---

## Conformidade — em migracao para medicao automatica

**Decisao de 31/07/2026:** a conformidade passa a ser **calculada pelo coletor** a partir do
export do CS Control, como ja acontece com receita e inadimplencia. Sai do lancamento manual.

**Por que:** existe **um unico lancamento** de conformidade no historico — o baseline de maio
(99,58%). Junho e julho reusaram esse mesmo numero. Eram 75 pts/mes pagos no automatico por
uma medicao que ninguem refez desde maio.

**Enquanto a automacao nao entra**, vale o comportamento atual (herda o ultimo valor lancado).
Pendencias para fechar: mapear os processos criticos que compoem o percentual e confirmar a
fonte do export com o Neriton.

---

## Time e individuo

Inadimplencia e conformidade sao medidas do **CS inteiro** — as tres recebem o mesmo.
A **venda e individual**: quem vende destrava a propria super e o proprio token.
E a primeira parte da regua do CS que separa as tres.

---

## Por que inadimplencia e o KPI principal

Cada 1% que o CS reduz = **R$4M/ano de receita protegida**.
De 12,9% (mai) para 2,72% (jul) = mais de **R$40M/ano** de receita protegida.

---

## Interdependencia

CS depende do closer vender BEM — cliente ruim aumenta inadimplencia.
Closer depende do CS reter — inadimplencia alta reduz o valor liquido e a pontuacao do closer.

---

> Para detalhes sobre bonus financeiro mensal, consultar o playbook-cs.
