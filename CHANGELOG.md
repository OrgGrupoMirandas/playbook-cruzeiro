# CHANGELOG — Cruzeiro dos Campeoes

Historico de mudancas de regra. Toda alteracao registrada aqui com data e motivo.

---

## 31/07/2026 — Growth: duas fontes (cat 0 resultado · cat 21 comportamento)

Terceiro setor revisado. A regua antiga media **uma fonte so** (cat 21) com faixas calibradas
em maio, que foi o **pico** daquele canal (988 leads).

| Mes | cat 0 | cat 21 |
|-----|-------|--------|
| Marco | 203 | 15 |
| Abril | 515 | **1.166** |
| Maio | 383 | 988 |
| Junho | 264 | 412 |
| Julho | **346** | **335** |

- A cat 21 **caiu 71%** de abril a julho; a cat 0 ficou estavel. Em julho as duas se cruzaram.
- Com zona morta em 700 e meta em 1.500, o Growth ficava em **zona morta todo mes** por
  qualquer das duas fontes. KPI que ninguem alcanca nao mede nada.
- **RESULTADO passa a ser cat 0** (topo do funil inteiro, onde o closer trabalha):
  <250 zona morta · 250-349 = 45 · 350-499 = 75 · 500-699 meta = 113 · >=700 super = 225.
- **cat 21 vira item de COMPORTAMENTO** ("Julia viva"): >=400/mes E sem queda >30% vs mes
  anterior = +30. As duas condicoes valem juntas — entregar 400 despencando de 700 nao pontua.
  Existe para a Julia nao morrer em silencio enquanto a cat 0 se sustenta por outros canais.
- Junho e julho **nao sao recalculados** (`escalaGrowth(mes)`).
- Efeito no Neriton: sai de 295 pts congelados (cabine Interna garantida) para 520 repetindo
  julho, ou ~1.010 com 520 leads cat 0 + Julia viva.
- **Comportamental de sistemas passa a ser semi-automatico:** uptime, webhook Julia→Bitrix,
  Meta Ads e entregas de sprint viram medicao do coletor; Lead Hub, Brevo e disparos seguem
  manuais ate existir fonte programatica. O comportamental vale 234 pts/mes e **nunca foi
  lancado uma unica vez** desde maio.

---

## 31/07/2026 — CS: escala nova de inadimplencia + conformidade vai para medicao automatica

Segundo setor revisado. A escala antiga foi escrita em maio com a inadimplencia em 12,9%;
julho fechou em **2,72%** — o CS batia o teto de 300 pts todo mes sem degrau acima.

- **Escala nova a partir de ago/2026:** super <=2% (225) · meta <=3% (113) · 3-6% zero ·
  >6% zona morta. Junho e julho **nao sao recalculados** — seguem pela escala antiga
  (mesma regra da promocao: mudanca de regua nao reescreve mes ja pontuado).
- Efeito: mantendo os mesmos 2,72%, o CS passa de 300 para **188 pts/mes**. Para voltar ao
  teto precisa levar a inadimplencia a <=2%. Projecao de dezembro da Kamila cai de 2.298
  para 1.738 — Suite ainda, mas conquistada em vez de automatica.
- **Conformidade:** descoberto que existe **um unico lancamento** no historico (baseline de
  maio, 99,58%) e que junho e julho reusaram esse mesmo numero — 75 pts/mes por uma medicao
  de tres meses atras. Decisao: **automatizar** via export do CS Control, nao voltar ao
  lancamento manual. Ate a automacao entrar, o comportamento atual continua.
- KPI do topo do site atualizado: teto de inadimplencia 9,8% -> 3,0%.

---

## 31/07/2026 — Gerente vale desde JULHO · trava do assistente migra para o time

Correcao das duas decisoes tomadas na mesma sessao, depois de olhar o julho real.

- **Gerente vigente a partir de julho/2026** (era agosto). Julho e o mes da promocao —
  nao fazia sentido pontuar o mes inteiro por uma regua que ja nao descrevia o cargo.
  Efeito: julho do Adrian sai de 50 pts (closer) para **110 pts** (gerente), porque o time
  fechou ~R$12,9M mesmo com a venda pessoal dele em R$3,86M.
- **Promocao nao reescreve mes antigo.** Colunas `setor_desde` e `setor_anterior` no D1 +
  `setorVigente()` no coletor: junho e anteriores continuam sendo pontuados como closer,
  qualquer que seja o recalculo. Sem isso, um backfill apagaria os 140 pts corretos de junho.
- **Trava do assistente migra de "Adrian >= R$6M pessoal" para "time >= R$12M"** (`07`).
  Com a promocao, o proprio Adrian deixou de ser medido por venda pessoal — em julho ele fez
  R$3,86M e pela regra antiga o Mateus zeraria num mes em que o time bateu a meta. Agora
  assistente, gerente e time perseguem **um numero so**.
- Junho (R$17,3M) e julho (~R$12,9M) estao **destravados** para o Mateus — falta o Adrian
  lancar a classificacao dos dois meses.
- Site ganhou o **capitulo 09 (Assistente)**, que nunca existiu — o Mateus nao conseguia ler
  a propria regua em lugar nenhum.

---

## 31/07/2026 — Comercial passa a ter tres reguas (gerente, closer, ramp-up)

Contexto: Adrian promovido a gerente comercial em teste em 01/07 e Pedro Pasin entrou
como closer no mesmo dia. Uma regua so nao servia para tres papeis diferentes.

- **Gerente (Adrian)** — vigente a partir de **ago/2026**. Venda propria com **peso 0,5**
  (R$1M = +5 · mes >= R$6M = +25) e resultado do time com peso cheio (time >= R$12M = +60 ·
  >= R$20M = +120 · CR medio do time pela tabela cheia · nenhum closer na zona morta = +30).
  Zona morta: time somado abaixo de R$6M zera o mes. Os **790 pts de jan-jul sao mantidos**.
- **Ramp-up (closer novo)** — degraus nos 3 primeiros meses: mes 1-2 piso R$1M / meta R$2M (+25) ·
  mes 3 piso R$1,5M / meta R$4M (+40) · mes 4+ regua cheia. R$1M = +10 e close rate valem
  desde o mes 1, sem degrau.
- **Pedro Pasin** cadastrado: Bitrix 37087, entrada 2026-07 => multiplicador **x2,00**,
  Suite em **500 pts**, corte coletivo **100 pts**. Julho real: R$2,05M, CR 7,1%, 5 vendas.
- Mateus Fuentes fica **fora** do agregado do time (assistente, sem carteira propria — o CR
  zerado dele derrubaria o CR do time).
- Site: capitulos 07 (Gerente) e 08 (Ramp-up) · coletor: `gerentePoints()`, `degrauRampUp()`,
  `mesDeCasa()` em `scoring.mjs` · D1: Pedro cadastrado e Adrian movido para setor `gerente`.

---

## 31/07/2026 — Entrada proporcional (novo capitulo 08)

Quem entra no time depois de janeiro passa a ter multiplicador proporcional, em vez de
"0 pontos e boa sorte". A regra ja existia na pratica (o ×1,5 dos setores que comecaram em
maio) mas nunca foi escrita como formula geral — logo nao servia para contratacao nova.

- **Formula unica:** `multiplicador = 12 ÷ meses de participacao no ano`.
  Reproduz exatamente o vigente: janeiro ×1,00 · maio ×1,50 (12÷8). Nada muda para quem ja corre.
- **Teto de 3,0** (setembro) — impede que quem entra em dezembro passe na frente de quem carregou o ano.
- **Piso de 4 meses** — entrou de outubro em diante nao corre por cabine individual; so caminho
  coletivo, corte proporcional, cabine Interna. Corrida cheia comeca em janeiro seguinte.
- **Regra do dia 15** — entrou ate o dia 15, o mes conta; do 16 em diante comeca no mes seguinte.
- **Corte coletivo tambem escala:** `200 × (meses ÷ 12)`.
- **Excecoes com multiplicador 1,00:** assistente de vendas (regua ja final), bonus IA (teto e
  mensal) e penalidades (erro grave custa igual para todos).
- **Saida/mudanca de funcao** documentada: muda de setor mantem pontos e passa a pontuar pela
  tabela nova, sem recalcular multiplicador.
- Regra 3 das gerais reescrita · site (capitulo 03 das Regras) · coletor (`scoring.mjs` +
  coluna `mes_entrada` no D1) atualizados junto.

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
