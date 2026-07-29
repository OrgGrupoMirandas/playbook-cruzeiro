# CHANGELOG — Cruzeiro dos Campeoes

Historico de mudancas de regra. Toda alteracao registrada aqui com data e motivo.

---

## 29/07/2026 — Imobiliario e Financeiro saem · regua do Assistente · ×1,5 explicitado

**Decisoes do Anthony:**
- **Cintia (Imobiliario) e Midiane (Financeiro) nao participam** do Cruzeiro — removidas do placar
  (D1 `people.ativo=0`). Nunca tiveram tabela de pontuacao propria; ficavam no placar sem regua.
- **Meta coletiva mantida em R$400M.** Avaliada a reducao para R$200M e recusada: R$400M entrega
  60% de margem e R$9,88M de resultado, o unico patamar que sustenta a tese patrimonial.
  Analise completa em `playbook-ceo/03-metricas/03-margem-por-volume.md`.
- **Assistente de Vendas ganha regua propria** (`07-pontuacao-assistente.md`): Mateus so pontua se
  o Adrian bater R$6M liquido; com a meta batida o Adrian classifica Pouco (+25) / Medio (+55) /
  Muito (+100), com justificativa de uma linha ate o dia 28. Sem multiplicador. Teto real: Premium.
  Antes ele era pontuado como closer (setor `comercial`) e caia na zona morta de R$2M todo mes.

**Correcoes de clareza (a fonte da confusao do Neriton):**
- **×1,5 agora e explicito** nos arquivos 03, 04 e 05: toda tabela tem coluna "Base" e coluna
  "Recebe (×1,5)". O multiplicador e aplicado **por cima** da tabela — nunca esteve embutido,
  mas o playbook nao dizia.
- **CS: faixa 9,8%–15% de inadimplencia = 0 pts**, explicitado. Nao existe pontuacao parcial.
- **CS: pontuacao e de time, nao individual** — Kamila, Sara e Andrea recebem o mesmo numero.
- **Growth e COO: comportamental/margem sao lancamento manual** — sem lancamento ate o dia 28,
  o mes fecha em zero. Antes isso so estava no codigo.
- Participantes: 11 -> 8 · KPIs coletivos atualizados para julho/2026.

---

## 19/07/2026 — Mariah sai do Cruzeiro (decisao Anthony)

- Mariah Miranda participa apenas do programa Codigo 31 — nao pontua no Cruzeiro
- Removida do placar (D1 `people.ativo=0`) e da lista de closers do 02
- Participantes: 12 -> 11
- Lista de closers acertada: Adrian, Arthur, Mateus Fuentes (Cintia ja reclassificada Imobiliario em 19/07)

## 19/07/2026 — Regra 10+20 do Bonus IA (aprovada por Anthony)

- Teto 30 pts/mes dividido: +10 automaticos (15+ dias ativos no straude) + ate 20 por entrega via issue
- Straude instalado em todo o time; coleta automatica diaria no placar
- Cintia (13693) reclassificada: Imobiliario (nao closer) — pontuacao pela tabela do imobiliario
- Mateus: linha duplicada unificada (Mateus Fuentes, Assistente de Vendas)

## 19/07/2026 — Correcao de contradicoes (auditoria Carla)

- Zona morta Growth unificada em <700 leads/mes (04 dizia <1.000, contradizendo a propria tabela e o 01)
- Supermeta comercial: explicitado que os +100 SUBSTITUEM os +50 da meta (ja era assim no calculo)
- README: removido link quebrado do 07-placar-atual.md (arquivo saiu do repo publico) — placar e o site
- Participantes: 13 -> 12 (offboarding Growth 25/06)

## 22/05/2026 — Criacao do playbook

- Playbook criado e publicado no GitHub
- Regras consolidadas das sessoes de 16-17/05 e 22/05/2026

## 15/05/2026 — Modelo hibrido de penalidades aprovado

- KPI nao batido = nao ganha pontos (nao desconta)
- Zona morta vendas: < R$2M = 0 pts total do mes
- Penalidade grave unica (-50 pts): abandono lead >72h ou falsificacao CRM

## 16-17/05/2026 — Calibracao geral do sistema

- CS simplificado para 2 KPIs (inadimplencia + conformidade)
- Growth KPI mudou de receita para leads/mes
- Valor LIQUIDO como base de calculo dos closers
- Bonus IA: teto 30 pts/mes (Neriton: 5 pts)
- Inicio setores nao-comerciais: Mai/2026 com pontos 1.5x
