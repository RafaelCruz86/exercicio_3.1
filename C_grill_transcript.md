# Grill Transcript — Service Blueprint AS-IS: Balcão Virtual TRT18

**Sessão:** `blueprint-asis-trt18`
**Data:** 2026-06-14
**Metodologia:** Shostack Service Blueprint (Evidências Físicas · Ações do Cidadão · Frontstage · Backstage · Processos de Suporte; linhas de interação, visibilidade e interação interna; fail points)
**Base:** B_relatorio_assistente_v3.md
**Artefatos a produzir:** C_blueprint_asis.md

---

## Regras da sessão

- Uma pergunta por rodada
- Cada pergunta inclui resposta recomendada
- Codebase explorado antes de perguntar quando possível
- Mínimo 6 rodadas antes de produzir os artefatos

---

## Rodadas

### Q1 — Jornada principal

**Pergunta:** Qual é a jornada principal do blueprint — o caminho do cidadão que acessa o Balcão Virtual diretamente pelo portal, ou uma das variantes (PID, TRT Presente, Balcão Visual)?

**Recomendado:** Jornada principal = cidadão acessa portal → localiza link da sala → entra na videochamada (Zoom) → atendido pelo servidor → obtém informação ou é encaminhado. Variantes como notas de ramificação.

**Resposta:** A jornada deve considerar todos os canais igualmente, após entrar no portal.

---

### Q2 — Estrutura dos canais

**Pergunta:** Como representar os cinco canais em paralelo — bifurcação com swimlanes ou matriz canal × etapa?

**Recomendado:** Bifurcação no ponto "selecionar canal", swimlanes paralelas por canal, convergência no desfecho.

**Resposta:** Usar bifurcação. Blueprint em formato de tabela. Mapear ≥ 5 etapas na ótica do cidadão com as cinco camadas Shostack, marcando fail points. Cada etapa/ator do blueprint deve aparecer no transcript.

---

### Q3 — 5 etapas na ótica do cidadão

**Pergunta:** Quais são as 5 etapas da jornada na ótica do cidadão?

**Proposta:**
1. Acesso ao portal (trt18.jus.br, seção de atendimento)
2. Seleção de canal (Balcão Virtual/Zoom · Celeste/WhatsApp · PID · TRT Presente · Balcão Visual)
3. Ingresso no atendimento (sala de vídeo / chat / chegada ao PID / sala passiva / link Libras)
4. Interação e solicitação (cidadão expõe demanda; atendente/sistema responde)
5. Desfecho (informação obtida / protocolo emitido / encaminhamento confirmado)

**Recomendado:** Manter as cinco exatamente — cobrem o arco completo sem sobreposição; fail points do v3 caem naturalmente nas etapas 2, 3 e 5.

**Resposta:** Etapas condizentes com a jornada. Confirmadas.

---

### Q4 — Atores do Frontstage

**Pergunta:** Quem são os atores visíveis no Frontstage em cada canal?

**Proposta:**
| Canal | Ator Frontstage |
|---|---|
| Balcão Virtual / Zoom | Servidor TRT18 em videochamada |
| Celeste / WhatsApp | Interface chatbot omnichannel Celeste (TRT18) |
| PID interno | Servidor TRT18 no PID (agendamento via SGJ) |
| TRT Presente | Servidor TRT18 na sala passiva (prédio TJ-GO) |
| Balcão Visual | Intérprete de Libras + servidor TRT18 (Divisão de Sustentabilidade, 12h–16h) |

**Recomendado:** Confirmar os cinco + adicionar portal trt18.jus.br como evidência física transversal de entrada.

**Resposta:** 5 atores confirmados. Correção: TRT Presente — sala em prédio TJ-GO, mas servidor é TRT18 (não TJ-GO).

---

### Q5 — Atores de Backstage e Processos de Suporte

**Pergunta:** Quais atores de Backstage e Processos de Suporte devem aparecer no blueprint?

**Proposta:**
| Camada | Ator/Processo | Canal(is) |
|---|---|---|
| Backstage | Equipe de TI / gestão de plataforma (Zoom/Meet) | Balcão Virtual, Balcão Visual |
| Backstage | Gestores de varas / escalas de atendimento | Todos |
| Backstage | Divisão de Sustentabilidade, Acessibilidade e Inclusão | Balcão Visual |
| Backstage | Comissão Regional PNJIID [lacuna C.4] | PID, TRT Presente |
| Processos de Suporte | Plataforma Celeste (lançada 27/05/2026) | Celeste/WhatsApp |
| Processos de Suporte | Sistema de agendamento SGJ | PID |
| Processos de Suporte | PJe (consulta processual) | Todos |
| Processos de Suporte | Parceria TJ-GO / TRF (infraestrutura física) | TRT Presente |

**Recomendado:** Incluir todos os 8; Comissão Regional marcada como [lacuna].

**Resposta:** Todos os 8 confirmados.

---

### Q6 — Fail Points

**Pergunta:** Quais fail points marcar no blueprint — e em qual etapa cada um incide?

**Proposta:**
| # | Fail Point | Etapa | Canal |
|---|---|---|---|
| FP1 | Divergência normativa Meet × Zoom (acesso à sala errada) | 3 — Ingresso | Balcão Virtual |
| FP2 | Paradoxo PID (inclusão que exige capacidade digital prévia) | 2 — Seleção | PID |
| FP3 | Janela morta Libras 8h–12h (4h sem atendimento acessível) | 3 — Ingresso | Balcão Visual |
| FP4 | Imaturidade Celeste (<1 mês em operação, risco de falha) | 4 — Interação | Celeste/WhatsApp |
| FP5 | Opacidade de fila no Zoom (sem info de espera ou posição) | 3 — Ingresso | Balcão Virtual |

**Recomendado:** Marcar todos os 5; FP1 e FP3 mais graves (governança e exclusão).

**Resposta:** Todos os 5 confirmados. Cobrem etapas do início ao fim da jornada.

---

## Entendimento Compartilhado — Decisões Bloqueadas

| # | Decisão | Valor bloqueado |
|---|---|---|
| D1 | Escopo da jornada | Portal → desfecho (todos os canais com peso igual após portal) |
| D2 | Estrutura dos canais | Bifurcação no ponto "seleção de canal"; swimlanes por canal; convergência no desfecho |
| D3 | Etapas (5) | Acesso ao portal · Seleção de canal · Ingresso · Interação e solicitação · Desfecho |
| D4 | Atores Frontstage (5) | Servidor TRT18/Zoom · Chatbot Celeste · Servidor TRT18/PID · Servidor TRT18/TRP · Intérprete Libras + Servidor TRT18 |
| D5 | Atores Backstage + Processos de Suporte (8) | TI TRT18 · Gestores de varas · Divisão de Sustentabilidade · Comissão PNJIID[lacuna] · Celeste · SGJ · PJe · Parceria TJ-GO/TRF |
| D6 | Fail Points (5) | FP1 Meet/Zoom · FP2 Paradoxo PID · FP3 Janela morta Libras · FP4 Celeste imatura · FP5 Opacidade de fila |

**Status:** Sessão completa (6/6 rodadas). Artefatos: C_blueprint_asis.md.


