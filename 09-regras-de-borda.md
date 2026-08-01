# Regras de Borda — o que acontece quando a vida acontece

Criado em 31/07/2026 depois da auditoria completa do programa. Sao as 12 situacoes que
**iam acontecer sem resposta escrita** — e resposta improvisada vira precedente ou briga.

> Todos os participantes sao **prestadores de servico (PJ)**. A linguagem deste playbook e a do
> regulamento seguem essa natureza: campanha de incentivo comercial, nao programa trabalhista.
> O documento juridico completo e o **Regulamento da Campanha** (repo privado, revisao do advogado).

---

## 1. Encerramento de contrato ANTES do embarque

A corrida termina em **31/12/2026**. O embarque e em **2027** (data na contratacao). No intervalo:

| Situacao | Resultado |
|----------|-----------|
| Prestador **rescinde** o contrato por iniciativa propria | Perde o premio |
| Empresa rescinde **por violacao contratual** (justa causa contratual) | Perde o premio |
| Empresa rescinde **sem violacao** (conveniencia) | **Mantem o premio conquistado** — a corrida ja tinha acabado |
| Encerramento **durante** a corrida (ate 31/12) | Perde pontuacao e nao embarca (regra ja vigente) |

> A terceira linha e a que evita litigio: quem venceu a corrida venceu. Tirar o premio de quem
> a propria empresa dispensou depois do fim e indefensavel.

## 2. Suspensao ou afastamento durante a corrida

Contrato suspenso por acordo, problema de saude documentado ou forca maior:

- A regua **pausa** — os meses parados nao contam nem a favor nem contra
- O multiplicador da entrada proporcional (`08`) e **recalculado** pelos meses efetivamente corridos
- Zona morta e reguas de minimo **nao se aplicam** a mes pausado

## 3. Ganhou mas nao pode embarcar

O premio e **personalissimo e intransferivel**. Nao converte em dinheiro em nenhuma hipotese —
conversao em dinheiro descaracteriza a campanha e vira problema tributario para todos.

- **Impossibilidade medica documentada** (propria ou de dependente direto): credito para a
  proxima edicao da campanha, se houver, OU remarcacao individual em ate 12 meses, a criterio
  da empresa — o que a agencia permitir sem custo adicional relevante
- Qualquer outro motivo: a vaga nao e cedida, nao e paga, nao acumula

## 4. Venda cancelada depois do ponto creditado

- Ponto de venda (individual) e gatilho coletivo contam **apenas cota com 1a parcela adimplida**
- Cancelamento/estorno em ate **60 dias** da venda: pontos e gatilho sao **revertidos** no
  fechamento seguinte (clawback)
- Cancelamento depois de 60 dias: nao reverte ponto individual, mas **ajusta o gatilho coletivo**
  se ainda nao disparou

## 5. Fechamento final e contestacao

| Etapa | Data |
|-------|------|
| Ultimo dia da corrida | 31/12/2026 |
| Fechamento preliminar publicado | 05/01/2027 |
| Prazo de contestacao | ate **10/01/2027** |
| Decisao final (Anthony, ultima instancia) | ate **20/01/2027** |
| Placar DEFINITIVO e imutavel | 20/01/2027 |

Contestacao: via issue no repositorio, com evidencia. Sem evidencia, nao se analisa.

## 6. Empate e arredondamento

- Arredondamento oficial: `Math.round` no ponto final de cada mes (como o coletor ja faz) —
  meio ponto sobe
- Empate exato em corte de cabine: desempata a **maior receita liquida acumulada** no ano;
  persistindo, os dois sobem

## 7. Quem entra em janeiro/2027

Contratado entre 01/01/2027 e o embarque **nao participa da edicao 2026** (a corrida ja fechou),
mas **e convidado ao embarque em cabine Interna como integracao** — a criterio da empresa e
condicionado a vaga na reserva. Nao e premio: e onboarding.

## 8. Recorrencia

A edicao 2026 e **unica e nao gera direito a edicoes futuras**. Se houver campanha 2027, sera
outro regulamento, outras metas, outra adesao. (Essa clausula protege a natureza de liberalidade
condicionada — sem ela, a recorrencia cria expectativa juridica.)

## 9. A semana do embarque

- A operacao **nao para**: Julia segue atendendo e agendando para a semana da volta
- **1 plantonista** em esquema definido pelo comercial ate 15/01 (rodizio ou acordo)
- Fevereiro/27 tera meta ajustada pela semana de ausencia — combinado antes, nao desculpa depois

## 10. Deslocamento, seguro e documentos

- Empresa cobre: cabine, taxas portuarias e **seguro-viagem** dos participantes e acompanhantes
- Cada participante cobre: deslocamento ate Santos e despesas pessoais a bordo (salvo o que o
  gatilho coletivo de 460 familias destravar)
- Documento: RG valido (menos de 10 anos) para roteiro America do Sul. Cada um responsavel pelo
  proprio e do acompanhante — sem documento, nao embarca e nao ha reembolso

## 11. Tributos

Cada prestador (PJ) e responsavel pelos proprios tributos. A empresa contrata e paga a viagem
**diretamente a agencia** — nao ha repasse em dinheiro a nenhum participante.

## 12. Penalidade grave (-50 pts) — processo

A penalidade existe desde maio e nunca foi aplicada porque nao tinha rito. Agora tem:

1. Deteccao: auditoria mensal do fechamento (Carla) ou denuncia com evidencia
2. Direito de resposta: 5 dias uteis
3. Decisao: Anthony
4. Registro: no CHANGELOG do playbook, sem detalhe pessoal

---

> Casos nao previstos: Anthony decide (regra 5 do `01`), e a decisao **vira regra escrita aqui**
> na semana seguinte — nenhum caso se decide duas vezes.
