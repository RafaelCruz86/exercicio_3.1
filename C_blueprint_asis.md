# Service Blueprint AS-IS — Balcão Virtual TRT18

**Versão:** 1.1 | **Data:** 2026-06-14
**Metodologia:** Shostack (1984) — Evidências Físicas · Ações do Cidadão · Frontstage · Backstage · Processos de Suporte
**Base:** B_relatorio_assistente_v3.md | **Decisões:** C_grill_transcript.md

---

## Legenda

**Canais (pós-bifurcação):**
- **[BV]** Balcão Virtual / Zoom
- **[CEL]** Celeste / WhatsApp
- **[PID]** PID Interno (Posto de Informação e Digitação)
- **[TRP]** TRT Presente (sala passiva em prédio TJ-GO)
- **[BVL]** Balcão Visual / Libras

**Marcações:**
- ⚠️ **FP#** = Fail Point (ponto de falha identificado)
- **[lacuna]** = dado não verificado publicamente; pendente LAI ou pesquisa primária

**Linhas divisórias Shostack:**
- `— LINHA DE INTERAÇÃO —` → separa o que o cidadão faz do que o serviço faz visivelmente
- `— LINHA DE VISIBILIDADE —` → separa o que o cidadão vê do que ocorre nos bastidores
- `— LINHA DE INTERAÇÃO INTERNA —` → separa o backstage humano dos processos tecnológicos de suporte

---

## Estrutura: Bifurcação por Canal

```
                          ┌─ [BV]  Balcão Virtual / Zoom
                          ├─ [CEL] Celeste / WhatsApp
Portal TRT18 ────────────┤─ [PID] PID Interno
(Etapa 1, canal único)    ├─ [TRP] TRT Presente
                          └─ [BVL] Balcão Visual / Libras
                                         │
                              Etapas 2–5 (swimlanes por canal)
                                         │
                                    ▼ Desfecho ▼
                     (informação obtida / protocolo / encaminhamento)
```

---

## Blueprint (tabela)

| Camada | **E1: Acesso ao Portal** | **E2: Seleção de Canal** | **E3: Ingresso no Atendimento** | **E4: Interação e Solicitação** | **E5: Desfecho** |
|---|---|---|---|---|---|
| **Evidências Físicas** | Portal trt18.jus.br; aba "Contato" com links por unidade ⚠️ **FP6** | Links de sala por unidade; WhatsApp 62 3222-5000 (Celeste); e-mail/tel. SGJ (PID); link Balcão Visual | [BV] Sala Zoom (link por unidade) · [CEL] Interface WhatsApp/app · [PID] Espaço físico do PID · [TRP] Sala passiva equipada · [BVL] Link sala Libras dedicada | [BV] Tela de videochamada; vídeo do servidor · [CEL] Interface de chat · [PID] Ambiente físico; servidor presente · [TRP] Sala com equipamento de vídeo · [BVL] Vídeo com intérprete e servidor | Confirmação verbal [BV/PID/TRP/BVL] · Mensagem de encerramento [CEL] · Protocolo/registro · Orientação de encaminhamento ⚠️ **FP7** |
| **Ações do Cidadão** | Acessa trt18.jus.br; navega até aba Contato / Atendimento ao Público ⚠️ **FP6** | Lê opções de canal disponíveis; seleciona conforme situação (presença, conectividade, necessidade de Libras) ⚠️ **FP2** | [BV] Clica no link da sala; aguarda na fila ⚠️ **FP5** · [CEL] Envia mensagem inicial pelo WhatsApp · [PID] Comparece na data e hora agendadas · [TRP] Acessa sala com orientação da Vara processante · [BVL] Clica no link Libras (disponível apenas 12h–16h) ⚠️ **FP3** | Expõe demanda processual; responde perguntas do servidor ou chatbot; fornece número do processo se solicitado | Recebe informação processual · e/ou obtém número de protocolo · e/ou recebe encaminhamento para canal alternativo ⚠️ **FP7** |
| ***⟵ LINHA DE INTERAÇÃO*** | *Abaixo desta linha: ações do prestador de serviço visíveis ao cidadão (frontstage)* | *Cidadão percebe o serviço mas não controla o que acontece abaixo* | *idem* | *idem* | *idem* |
| **Frontstage** | Portal trt18.jus.br como interface institucional visível | Aba "Contato" do portal; lista de unidades e canais | [BV] Servidor TRT18 em videochamada (fundo neutro; vestimenta formal — Portaria 414/2021) ⚠️ **FP1** · [CEL] Chatbot omnichannel Celeste ⚠️ **FP4** · [PID] Servidor TRT18 presencialmente · [TRP] Servidor TRT18 em sala passiva (prédio TJ-GO) · [BVL] Intérprete de Libras + servidor TRT18 (Divisão de Sustentabilidade) | [BV] Servidor TRT18 conduz atendimento por vídeo · [CEL] Chatbot / atendente Celeste responde e direciona · [PID] Servidor TRT18 atende presencialmente · [TRP] Servidor TRT18 atende remotamente via sala passiva · [BVL] Intérprete de Libras medeia; servidor TRT18 responde | Servidor / chatbot comunica resultado; emite orientação de encaminhamento se necessário |
| ***⟵ LINHA DE VISIBILIDADE*** | *Abaixo desta linha: ações invisíveis ao cidadão (backstage)* | *Cidadão não vê nem interage com o que ocorre abaixo* | *idem* | *idem* | *idem* |
| **Backstage** | Equipe de TI TRT18 (manutenção e disponibilidade do portal) | Gestores de varas (definição de escalas de atendimento); TI TRT18 (disponibilidade dos canais) | [BV] TI TRT18 / gestão da plataforma Zoom/Meet · [CEL] TI TRT18 / Celeste · [PID] Gestores de varas; Comissão Regional PNJIID **[lacuna C.4]** · [TRP] Gestores de varas · [BVL] Divisão de Sustentabilidade, Acessibilidade e Inclusão (ramais 5421/5426) | Gestores de varas (supervisão de escalas); TI TRT18 (estabilidade das plataformas); Divisão de Sustentabilidade (Balcão Visual) | Registro interno do atendimento; geração e arquivo de protocolo; notificação de encaminhamento |
| ***⟵ LINHA DE INTERAÇÃO INTERNA*** | *Abaixo desta linha: sistemas e processos tecnológicos de suporte (sem contato humano direto)* | *Contratos, plataformas e integrações que sustentam o backstage* | *idem* | *idem* | *idem* |
| **Processos de Suporte** | Hospedagem e CDN do portal trt18.jus.br; PJe (base processual de suporte) | PJe (consulta de processos); SGJ — sgj@trt18.jus.br / 62 3222-5139 (agendamento PID); Plataforma Celeste; Parceria TJ-GO/TRF (infraestrutura TRT Presente) | [BV] Plataforma Zoom / Google Meet (Portaria 414/2021) · [CEL] Plataforma Celeste (lançada 27/05/2026) · [PID] Sistema de agendamento SGJ · [TRP] Parceria TJ-GO/TRF (153 salas passivas) · [BVL] Sala Zoom dedicada (Balcão Visual) | PJe (consulta processual em tempo real durante o atendimento); Celeste (roteamento e histórico de interações); SGJ (registro de atendimento PID) | PJe; sistema de protocolo TRT18; Celeste (encerramento de ticket) |

---

## Fail Points Mapeados

| # | Fail Point | Etapa | Canal | Natureza | Hipótese de Fricção |
|---|---|---|---|---|---|
| ⚠️ FP1 | **Divergência normativa Meet × Zoom** — Portaria 414/2021 define Google Meet como plataforma contratada; portal exibe links Zoom na prática; cidadão pode não conseguir acessar se configuração divergir | E3 — Ingresso | [BV] Balcão Virtual | Governança de plataforma | Falha de governança / ausência de portaria de migração (lacuna C.1) |
| ⚠️ FP2 | **Paradoxo PID** — canal destinado à inclusão digital exige agendamento prévio por e-mail ou telefone, criando barreira para o próprio público excluído digitalmente que deveria ser atendido | E2 — Seleção | [PID] PID Interno | Barreira de acesso | Exclusão digital paradoxal |
| ⚠️ FP3 | **Janela morta Libras (8h–12h)** — Balcão Visual opera apenas das 12h às 16h; usuário surdo que acessa o portal fora desse horário não encontra atendimento acessível por 4 horas do horário de funcionamento | E3 — Ingresso | [BVL] Balcão Visual | Exclusão de grupo vulnerável | Restrição de horário sem alternativa |
| ⚠️ FP4 | **Imaturidade da Celeste** — canal omnichannel lançado há menos de 1 mês na data da pesquisa (27/05/2026); risco elevado de falha de direcionamento, resposta incompleta ou indisponibilidade | E4 — Interação | [CEL] Celeste/WhatsApp | Maturidade tecnológica | Canal novo sem histórico de estabilidade verificado |
| ⚠️ FP5 | **Opacidade de fila no Balcão Virtual** — cidadão entra na sala Zoom sem nenhuma informação sobre tempo de espera ou posição na fila; ausência de gestão de expectativa gera abandono ou múltiplas tentativas | E3 — Ingresso | [BV] Balcão Virtual | Experiência do usuário | Fila invisível; sem SLA publicado |
| ⚠️ FP6 | **Link inoperante ou canal ausente no portal** — se o link da sala de vídeo de uma unidade estiver quebrado, desatualizado ou ausente na aba Contato, o cidadão não consegue iniciar a jornada; sem canal de fallback imediato visível | E1 — Acesso ao Portal | Todos os canais | Disponibilidade do portal | Ponto único de falha na entrada da jornada |
| ⚠️ FP7 | **Desfecho sem confirmação acessível ao cidadão** — em todos os canais exceto CEL, a informação prestada é verbal (vídeo ou presencial) sem registro escrito entregue ao cidadão; ausência de comprovante dificulta contestação e gera retrabalho | E5 — Desfecho | Todos os canais (especialmente [BV], [PID], [TRP], [BVL]) | Ausência de registro | Informação oral sem trilha de auditoria para o cidadão |

---

## Matriz RACI — Responsabilidades e Interações entre Atores

**Legenda RACI:**
- **R** = Responsible — executa a atividade
- **A** = Accountable — responde pelo resultado (aprova / decide)
- **C** = Consulted — é consultado antes ou durante
- **I** = Informed — é comunicado após / monitorado

**Atores (colunas):**

| Sigla | Ator |
|---|---|
| CID | Cidadão |
| TI | TI TRT18 (gestão de plataforma e portal) |
| GV | Gestores de varas (escalas e supervisão) |
| SRV | Servidores TRT18 — frontstage BV / PID / TRP |
| CEL | Chatbot / atendente Celeste — frontstage CEL |
| INT | Intérprete de Libras + Servidor TRT18 — frontstage BVL |
| DSAI | Divisão de Sustentabilidade, Acessibilidade e Inclusão |
| PNJIID | Comissão Regional PNJIID **[lacuna C.4]** |

> Processos de suporte (PJe, SGJ, Plataforma Celeste, Parceria TJ-GO/TRF) são sistemas — não recebem papel RACI, mas aparecem como dependência nas linhas relevantes.

---

### Tabela RACI por Atividade e Etapa

| Atividade | Etapa | CID | TI | GV | SRV | CEL | INT | DSAI | PNJIID |
|---|---|---|---|---|---|---|---|---|---|
| Manter portal e links de sala ativos | E1 | I | **R/A** | I | I | I | I | I | — |
| Acessar portal e navegar até aba Contato | E1 | **R** | I | — | — | — | — | — | — |
| Definir escalas de atendimento por unidade | E2 | I | C | **R/A** | C | — | — | C | C |
| Disponibilizar e publicar canais no portal | E2 | I | **R/A** | C | I | C | C | I | I |
| Selecionar canal conforme necessidade | E2 | **R** | I | I | I | I | I | I | I |
| Disponibilizar sala Zoom por unidade [BV] | E3 | I | **R/A** | C | I | — | — | — | — |
| Operar e estabilizar Plataforma Celeste [CEL] | E3 | I | **R/A** | — | — | C | — | — | — |
| Viabilizar agendamento via SGJ [PID] | E3 | C | C | C | I | — | — | — | **R/A** |
| Manter salas passivas TJ-GO operacionais [TRP] | E3 | I | C | I | — | — | — | — | **R/A** |
| Prover sala Libras e intérprete (12h–16h) [BVL] | E3 | I | C | I | — | — | **R** | **A** | — |
| Ingressar no canal de atendimento | E3 | **R** | I | I | I | I | I | I | I |
| Conduzir o atendimento ao cidadão | E4 | I | I | **A** | **R** | **R** | **R** | C | — |
| Consultar PJe durante o atendimento | E4 | I | I | I | C | C | C | — | — |
| Expor demanda e fornecer dados processuais | E4 | **R** | — | I | I | I | I | — | — |
| Supervisionar qualidade do atendimento | E4 | — | I | **R/A** | I | I | I | C | C |
| Registrar atendimento internamente | E5 | I | C | **A** | **R** | **R** | **R** | C | — |
| Emitir protocolo ou orientação de encaminhamento | E5 | I | C | **A** | **R** | **R** | **R** | — | — |
| Receber desfecho (informação / protocolo) | E5 | **R** | — | I | I | I | I | — | — |

---

### Síntese das Responsabilidades por Ator

| Ator | Papel predominante | Etapas críticas | Observação |
|---|---|---|---|
| **CID** Cidadão | R em todas as suas próprias ações; I no backstage e suporte | E1, E2, E3, E4 (demanda), E5 (recepção) | Único R nas ações de navegação, seleção e exposição da demanda |
| **TI** TI TRT18 | R/A em infraestrutura e plataformas; C em governança | E1, E2, E3 | Ponto de responsabilidade para FP1 (Meet/Zoom), FP4 (Celeste), FP6 (portal) |
| **GV** Gestores de varas | A na entrega do serviço; R/A nas escalas | E2, E4, E5 | Accountable final pelo atendimento em todos os canais não automatizados |
| **SRV** Servidores TRT18 | R na execução do atendimento frontstage [BV/PID/TRP] | E3, E4, E5 | Respondem às escalas definidas por GV; visíveis ao cidadão |
| **CEL** Chatbot/Celeste | R no atendimento automatizado [CEL] | E3, E4, E5 | Imaturidade operacional (FP4); dependência da Plataforma Celeste |
| **INT** Intérprete + Servidor | R no atendimento mediado [BVL] | E3, E4, E5 | Restrito ao horário 12h–16h (FP3); gerido por DSAI |
| **DSAI** Div. Sustentabilidade | A no Balcão Visual; R na provisão de intérpretes e sala | E3, E5 | Única unidade gestora do BVL; ramais 5421/5426 |
| **PNJIID** Comissão Regional | A na governança PID e TRT Presente **[lacuna]** | E3 | Papel previsto pela CSJT 428/2025; não verificado publicamente |

---

## Normativos Aplicáveis

| Normativo | Relevância no Blueprint |
|---|---|
| CNJ Res. 372/2021 | Obrigatoriedade do Balcão Virtual; âncora da jornada principal |
| Portaria TRT18 414/2021 | Plataforma (Google Meet), horários, vestimenta frontstage, teletrabalho dos servidores |
| Portaria TRT18 896/2021 | Juízo 100% Digital; âncora provável da adoção do Zoom (lacuna C.1) |
| Portaria GP/SGP 437/2022 (alt. 1345/2023) | Regulação dos PIDs internos |
| CNJ Res. 508/2023 | PIDs obrigatórios |
| CSJT Res. 218/2018 | Libras na Justiça do Trabalho; base do Balcão Visual |
| CSJT Res. 428/2025 (PNJIID) | Política Nacional de Justiça Itinerante; vincula PIDs e TRT Presente a planos anuais e Comissão Regional |

---

## Lacunas para Pesquisa Primária / LAI

| Cód. | Lacuna | Impacto no Blueprint |
|---|---|---|
| C.1 | Portaria específica de migração Google Meet → Zoom | FP1 permanece sem resolução normativa |
| C.4 | Comissão Regional PNJIID do TRT18 | Ator de backstage marcado como [lacuna] no PID e TRT Presente |
| — | Escalas internas, scripts de atendimento | Backstage dos servidores de varas não detalhado |
| — | Indicadores de desempenho (TMA, taxa de resolução, uptime) | Processos de Suporte sem SLA verificado |
| — | Volume real TRT Presente vs. Balcão Virtual direto | Peso relativo dos canais no blueprint não confirmado |
