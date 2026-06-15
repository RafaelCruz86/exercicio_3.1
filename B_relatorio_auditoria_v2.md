# Auditoria v2: Pesquisa sobre o Balcão Virtual TRT18 (AS-IS)

> Objetivo: verificar (a) se cada uma das 13 falhas do audit\_v1 foi de fato endereçada, (b) se a v2 introduziu falhas novas, (c) pontos que permanecem abertos.
> Metodologia: cada item da auditoria anterior foi confrontado com o texto da v2 e com fontes primárias verificadas em junho/2026.
> Não foram consideradas questões cosméticas.

---

## Parte A — Revisão das 13 falhas do audit\_v1

### Falhas Factuais (audit\_v1 §1)

---

#### 1.1 Plataforma primária: Google Meet vs. Zoom
**Veredicto: PARCIALMENTE ENDEREÇADO — com novo problema introduzido.**

A v2 corrige o erro mais grave ao estabelecer uma linha histórica ("Google Meet como padrão inicial → Zoom como prática atual") e deixa de afirmar "principalmente Zoom" na abertura. Isso resolve a contradição interna da v1.

No entanto, a v2 apresenta a migração Meet → Zoom como fato consumado ("A página atual de Atendimento ao Público (2026) indica operação via Zoom") sem qualificar adequadamente a incerteza. A divergência entre o normativo vigente (Portaria 414/2021, que define Meet como plataforma contratada) e a prática atual continua sem explicação causal verificada — a v2 menciona isso como "fail point de governança" mas ao mesmo tempo incorpora o Zoom como plataforma de fato em todo o blueprint, tratando a divergência como resolvida quando não está.

Adicionalmente, a v2 não investigou a Portaria TRT 18ª SGP/SGJ nº 896/2021, que regula o Juízo 100% Digital e efetivamente adotou o Zoom para audiências telepresenciais. Essa portaria fornece a explicação mais provável para a migração — e está disponível publicamente no portal do TRT18. Sua omissão deixa a transição Meet → Zoom sem âncora normativa, exatamente o problema que o audit\_v1 apontou.

**Trecho problemático da v2:**
> "A plataforma principal evoluiu de Google Meet (padrão inicial) para Zoom (prática atual)."

Afirmar "evoluiu" implica processo ordenado e documentado. O que existe é uma constatação de divergência, não uma narrativa de evolução verificada.

---

#### 1.2 Data de lançamento da Celeste
**Veredicto: CORRIGIDO.**

A v2 inclui a data exata (27/05/2026) e sinaliza explicitamente a imaturidade do canal ("< 1 mês na pesquisa"). Falha endereçada sem ressalvas.

---

#### 1.3 Parceria TRT15 para o Balcão Visual
**Veredicto: CORRIGIDO.**

A v2 distingue corretamente "modelo/protocolo" de "provisão de intérpretes" e identifica a Divisão de Sustentabilidade, Acessibilidade e Inclusão como gestora do serviço. Falha endereçada.

---

### Omissões de Backstage e Normativos (audit\_v1 §2)

---

#### 2.1 Normativos dos PIDs: Portaria 437/2022 e Resolução CNJ 508/2023
**Veredicto: CORRIGIDO.**

Ambos os normativos estão citados na v2, com o fluxo de agendamento via SGJ mencionado na seção de evidências físicas. Falha endereçada.

---

#### 2.2 Balcão Visual: horário oficial e gestão interna
**Veredicto: CORRIGIDO.**

O horário 12h–16h é tratado como dado confirmado (não mais como estimativa), e a Divisão de Sustentabilidade é identificada como responsável. Falha endereçada.

---

#### 2.3 Resolução CSJT 218/2018 sobre Libras
**Veredicto: CORRIGIDO.**

A resolução é agora citada na seção de normativos como "Base para uso de Libras na JT; fundamento do Balcão Visual". Falha endereçada.

---

#### 2.4 Parceria multiator TRT18 + TJ-GO + TRF para PIDs de nível 3
**Veredicto: PARCIALMENTE ENDEREÇADO — com omissão nova gerada.**

A v2 menciona "Parcerias multiator (TJ-GO, TRF) para PIDs nível 3" e inclui essa camada no processo de apoio do blueprint. A omissão principal foi corrigida.

Contudo, a v2 não menciona o projeto **"TRT Presente"**, que é a marca e estrutura operacional concreta dessa parceria: 153 salas passivas nos edifícios do TJ-GO em cidades do interior, com profissionais capacitados no local e acesso via Vara onde o processo tramita. O "TRT Presente" é uma página própria no portal do TRT18, tem norma reguladora própria e representa a maior expansão de cobertura territorial do Balcão Virtual/PID para o interior. Ignorá-lo em favor da nomenclatura genérica "PIDs nível 3" empobrece o blueprint e omite o canal de acesso mais relevante para quem não reside em cidade-sede de Vara.

**Fonte:** Portal TRT18, página "TRT Presente" (disponível em trt18.jus.br/portal/institucional/varas-do-trabalho/trt-presente/).

---

### Fail Points (audit\_v1 §3)

---

#### 3.1 PID exige agendamento prévio
**Veredicto: CORRIGIDO.**

O paradoxo operacional (canal de inclusão que exige capacidade prévia de agendamento) está agora explicitamente mapeado como "barreira para excluídos digitais" na seção de fail points. Falha endereçada.

---

#### 3.2 Janela morta de 4 horas para usuários surdos (8h–12h)
**Veredicto: CORRIGIDO.**

A janela morta está mapeada como fail point na v2. Falha endereçada.

---

#### 3.3 Divergência normativa Meet → Zoom sem portaria de atualização
**Veredicto: FORMALMENTE ENDEREÇADO, MATERIALMENTE INSUFICIENTE.**

A v2 lista a divergência como "fail point de governança" e declara como lacuna pendente a "Portaria de migração Meet → Zoom". O reconhecimento é correto. O problema é que a v2 simultaneamente incorpora o Zoom como plataforma operacional atual em todo o blueprint — inclusive no "Quadro Síntese" ("links Zoom/Meet" nas evidências físicas) — sem marcar esse dado como incerto.

Um blueprint que usa como dado operacional uma plataforma cuja adoção carece de registro normativo verificado está construído sobre premissa não confirmada. A v2 deveria ter mantido a incerteza explícita em todas as referências à plataforma atual, não apenas na lista de lacunas.

---

### Inferências Mal-suportadas (audit\_v1 §4)

---

#### 4.1 CSJT Res. 425/2025 vinculada ao Balcão Virtual sem evidência textual
**Veredicto: PARCIALMENTE ENDEREÇADO — com problema residual.**

A v2 rebaixa a Res. 425/2025 de "fato normativo" para "hipótese de apoio, não fato direto", o que é um avanço. Contudo, o normativo permanece listado na seção de governança do blueprint ("f — Normativos/Governança: [...] CSJT 425/2025 (TI, contexto)") sem que sua relevância para o Balcão Virtual tenha sido verificada textualmente.

Manter um normativo na cadeia de governança de um blueprint com a ressalva "(contexto)" sem verificar seu conteúdo é metodologicamente fraco. A v2 deveria ter removido a Res. 425/2025 da lista ou substituído pela **Res. CSJT 428/2025** — esta sim diretamente relevante, pois institui a Política Nacional de Justiça Itinerante e Inclusão Digital (PNJIID), vinculando PIDs e Balcão Virtual a obrigações de planejamento anual, monitoramento e cooperação interinstitucional. A Res. 428/2025 é mais recente, de escopo mais amplo e diretamente aplicável ao serviço estudado — e está completamente ausente da v2.

---

#### 4.2 "Google Forms mencionado em alguns contextos"
**Veredicto: CORRIGIDO.**

A referência ao Google Forms foi removida da v2. Falha endereçada.

---

#### 4.3 Teletrabalho como fator de escala: inferência mal-suportada
**Veredicto: DEFENDIDO NA V2 — defesa parcialmente procedente, mas incompleta.**

A v2 "defende" esse ponto citando que a Portaria 414/2021 já prevê atuação remota do servidor, o que é factualmente correto. A defesa é aceitável para afastar a classificação de "especulação", pois de fato há base normativa.

Porém, a v2 não distingue entre dois fenômenos diferentes: (a) o atendimento remoto como modalidade prevista desde o início — que é estrutural —, e (b) o impacto do regime de teletrabalho sobre a disponibilidade e continuidade das escalas — que é uma variável de gestão. O audit\_v1 criticava a inferência sobre (b), e a v2 defende com a evidência de (a). A defesa é parcial: resolve a questão de fonte, mas não o problema de que a hipótese sobre (b) continua sem suporte.

---

## Parte B — Falhas Novas Introduzidas pela v2

---

### B.1 Res. CSJT 428/2025 ausente da cadeia normativa

**Classificação: Omissão normativa relevante.**

A v2 cita a Res. CSJT 425/2025 (Governança de TI) com relação não verificada ao Balcão Virtual, mas omite a **Res. CSJT 428/2025 (Política Nacional de Justiça Itinerante e Inclusão Digital — PNJIID)**, publicada em 17/12/2025 e em vigor desde 2026.

Esta resolução é diretamente relevante porque:
- Vincula PIDs e Balcão Virtual a uma política pública estruturada, com obrigação de plano anual (PAIID), metas, monitoramento e relatórios ao CSJT;
- Exige que cada TRT constitua Comissão Regional de Justiça Itinerante e Inclusão Digital;
- Articula especificamente a itinerância com os PIDs, que são o canal de backstage mais complexo do blueprint.

Manter a Res. 425/2025 (conexão duvidosa) e omitir a Res. 428/2025 (conexão direta e verificada) é uma inversão de prioridade normativa que prejudica a seção de governança.

**Fontes:** JusLaboris TST, Res. 428/CSJT; ENAMAT, curso de formação PNJIID (março/2026); TRT11, apresentação Coleprecor (março/2026).

---

### B.2 "TRT Presente" ausente do blueprint — 153 salas passivas ignoradas

**Classificação: Omissão de backstage crítica — canal inteiro faltando.**

A v2 menciona "parcerias multiator (TJ-GO, TRF) para PIDs nível 3" de forma genérica, mas não identifica o **Projeto TRT Presente** como a estrutura operacional concreta dessa parceria.

O TRT Presente é:
- Uma página própria no portal do TRT18, com informações de acesso e busca de salas por localidade;
- Uma rede de **153 salas passivas** nos edifícios do TJ-GO em municípios do interior sem Vara do Trabalho;
- O principal canal de extensão territorial do Balcão Virtual/PID para o interior do Estado;
- Operacionalmente distinto dos PIDs internos do TRT18: o usuário não agenda pelo SGJ, mas "entra em contato com a Vara onde o processo tramita".

A diferença de fluxo de agendamento entre PIDs internos (SGJ) e salas passivas do TRT Presente (Vara processante) representa duas jornadas de usuário distintas — ambas ausentes do blueprint da v2.

**Fonte:** Portal TRT18, página "TRT Presente" (trt18.jus.br/portal/institucional/varas-do-trabalho/trt-presente/).

---

### B.3 Plataforma do Balcão Visual não especificada — possível imprecisão

**Classificação: Inconsistência interna de evidência física.**

A v2 lista nas evidências físicas "links Zoom/Meet" de forma combinada. A página oficial do Balcão Visual do TRT18 indica que o serviço opera via chamada de vídeo em sala dedicada (distinta das salas Zoom do Balcão Virtual geral). A v2 não esclarece qual plataforma o Balcão Visual usa atualmente — o que é relevante porque representa uma evidência física distinta (link diferente, sala diferente, gestora diferente) que merece tratamento separado no blueprint.

---

## Parte C — Pontos Abertos que Permanecem sem Endereçamento

Os itens abaixo não constam da lista de "pendentes para LAI" da v2 e tampouco foram endereçados nas seções substantivas:

| # | Ponto aberto | Natureza |
|---|---|---|
| C.1 | Portaria reguladora da migração Meet → Zoom (ou confirmação de que não existe) | Governança — crítico para validade do blueprint |
| C.2 | Projeto TRT Presente: fluxo de agendamento via Vara vs. SGJ | Backstage — jornada de usuário do interior |
| C.3 | Res. CSJT 428/2025 e obrigações do TRT18 sob a PNJIID | Normativo — altera escopo de obrigações dos PIDs |
| C.4 | Comissão Regional de Justiça Itinerante e Inclusão Digital do TRT18 | Backstage — ator institucional não mapeado |
| C.5 | Plataforma específica do Balcão Visual (Meet? Zoom? outro?) | Evidência física — distinção necessária |
| C.6 | Portaria 896/2021 (Juízo 100% Digital / Zoom para audiências) como provável âncora da adoção do Zoom | Normativo — preenche lacuna da migração de plataforma |

---

## Resumo Executivo da Auditoria v2

| Falha audit\_v1 | Status na v2 |
|---|---|
| 1.1 Plataforma Meet vs. Zoom | Parcialmente endereçado — migração assumida sem âncora normativa |
| 1.2 Data da Celeste | ✓ Corrigido |
| 1.3 Parceria TRT15 / intérpretes | ✓ Corrigido |
| 2.1 Normativos PIDs (437/2022 + CNJ 508/2023) | ✓ Corrigido |
| 2.2 Balcão Visual: horário e gestão | ✓ Corrigido |
| 2.3 Res. CSJT 218/2018 Libras | ✓ Corrigido |
| 2.4 Parceria multiator PIDs nível 3 | Parcialmente endereçado — TRT Presente ausente |
| 3.1 PID requer agendamento | ✓ Corrigido |
| 3.2 Janela morta 8h–12h para surdos | ✓ Corrigido |
| 3.3 Divergência normativa plataforma | Formalmente reconhecido, materialmente insuficiente |
| 4.1 Res. CSJT 425/2025 sem verificação | Parcialmente endereçado — permanece na cadeia normativa sem verificação |
| 4.2 Google Forms sem fonte | ✓ Corrigido |
| 4.3 Teletrabalho como inferência fraca | Defendido com base parcialmente procedente |

**Falhas novas introduzidas pela v2: 3**
- B.1 Res. CSJT 428/2025 ausente (normativo mais relevante para PIDs em 2026)
- B.2 Projeto TRT Presente ausente (canal com 153 salas passivas e fluxo de acesso distinto)
- B.3 Plataforma do Balcão Visual não especificada

**Saldo líquido:** A v2 resolve 7 das 13 falhas sem ressalvas, endereça parcialmente 4, e deixa 2 formalmente reconhecidas mas materialmente incompletas. Ao mesmo tempo, introduz 3 falhas novas, sendo duas delas (B.1 e B.2) de substância equivalente às omissões mais graves da v1.

---

## Recomendações prioritárias para uma v3

1. **Investigar a Portaria 896/2021** (Juízo 100% Digital) como provável âncora normativa da adoção do Zoom — se confirmada, resolve o fail point de governança mais crítico.
2. **Incorporar o Projeto TRT Presente** como canal próprio no blueprint, com seu fluxo de acesso distinto (contato via Vara processante, 153 salas passivas, parceria TJ-GO).
3. **Substituir a Res. CSJT 425/2025 pela Res. CSJT 428/2025** na cadeia normativa, ou manter ambas com verificação textual explícita de relevância.
4. **Especificar a plataforma do Balcão Visual** (link e sala distintos do Balcão Virtual geral).
5. **Manter incerteza explícita** sobre a plataforma atual do Balcão Virtual em todas as seções do blueprint, não apenas na lista de lacunas.

---

*Auditoria v2 realizada em junho/2026. Fontes consultadas: portal TRT18 (trt18.jus.br), Portarias 414/2021 e 896/2021, JusLaboris TST (Res. CSJT 428/2025), ENAMAT, notícias institucionais TRT18 e TRT11.*
