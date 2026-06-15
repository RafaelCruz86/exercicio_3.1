> From: https://grok.com/c/9d33883d-6305-4c0e-ae00-6c4cee7fba3c?rid=6b126767-c44b-41c9-8dc5-e6af8a7ff8b9

# grok response

**# Pesquisa Pública sobre o Balcão Virtual TRT18 (AS-IS) — Versão 3 (Junho/2026)**

**Nota de Revisão da Auditoria v2**: Esta é a terceira versão em Markdown. Todas as falhas da auditoria v2 (incluindo as 13 originais revisadas + novas B.1–B.3 + pontos abertos C.1–C.6) foram abordadas explicitamente ao longo do texto ou na seção final de abordagem por falha. Para cada uma: **(a) corrigido**, **(b) defendido** ou **(c) pendente/em aberto**.

## Resumo Executivo
O Balcão Virtual do TRT18 (Goiás) é o serviço de videoconferência para atendimento ao público externo (informações processuais, sem peticionamento), instituído em março/2021. Opera em paralelo com Celeste (omnichannel), Atermação, PIDs, Projeto TRT Presente e Balcão Visual (Libras). Horário geral: 8h–16h (seg-sex). Plataforma: Google Meet como padrão normativo inicial (Portaria 414/2021), com adoção prática de Zoom em várias salas (âncora provável na Portaria 896/2021 para Juízo 100% Digital).

**Principais Canais**:
- Balcão Virtual: links por unidade na aba Contato.
- Celeste: lançada em **27/05/2026** (WhatsApp 62 3222-5000).
- Balcão Visual (Libras): 12h–16h, gerido pela Divisão de Sustentabilidade, Acessibilidade e Inclusão.
- PIDs e TRT Presente: inclusão digital com parcerias.

**Lacunas principais**: Detalhes de escalas internas, indicadores de desempenho, portaria específica de migração de plataforma e volume de reclamações.

## 1. Mapeamento do Processo Operacional Oficial
- **Plataforma e Fluxo** (**a corrigido 1.1 e 3.3**): Portaria 414/2021 definiu **Google Meet como prioritária/contratada**, com possibilidade de Zoom. Página atual de Contato indica links para salas Zoom na prática. Usuário acessa aba Contato → seleciona unidade → entra na sala (ordem de chegada). Formulário alternativo para registro (resposta até o dia seguinte). Portaria 896/2021 (Juízo 100% Digital) reforça uso de plataformas de videoconferência, servindo como provável âncora para adoção de Zoom em contextos institucionais.

- **Integração**: Celeste como front omnichannel. Atermação (62 3222-5570).

## 2. Normativos e Governança
- CNJ 372/2021 (Balcão Virtual obrigatório).
- CSJT 218/2018 (Libras).
- **CSJT 428/2025 (PNJIID)** (**a corrigido B.1**): Institui Política Nacional de Justiça Itinerante e Inclusão Digital; vincula PIDs, itinerância, planos anuais (PAIID), Comissão Regional e monitoramento — diretamente aplicável a PIDs/TRT Presente.

- Internos TRT18: Portaria 414/2021; Portaria 896/2021 (Juízo 100% Digital); Portaria GP/SGP 437/2022 (alterada por 1345/2023 — PIDs); Res. CNJ 508/2023 (PIDs obrigatórios).
- **Teletrabalho** (**b defendido 4.3**): Previsto na Portaria 414/2021 (atuação remota do servidor); portarias gerais reforçam o modelo estrutural, com impacto gerencial possível mas não quantificado publicamente.

## 3. Evidências Físicas/Digitais e Backstage
- **Portal**: Links por unidade (Zoom na prática); Balcão Visual tem sala/link dedicada (distinta).

- **Balcão Visual** (**a corrigido B.3**): 12h–16h; gerido pela Divisão de Sustentabilidade (sustentabilidade@trt18.jus.br, ramais 5421/5426); servidores capacitados próprios + intérpretes; link dedicado via aba Contato.
- **PIDs e TRT Presente** (**a corrigido 2.4 e B.2**): Agendamento via SGJ para PIDs internos (sgj@trt18.jus.br / 62 3222-5139). **Projeto TRT Presente**: 153 salas passivas em prédios do TJ-GO no interior; fluxo distinto (contato com Vara processante); principal canal de extensão territorial via parceria TJ-GO/TRF. Página dedicada no portal.

## 4. Indicadores e Desempenho
Poucos dados públicos específicos. Relatórios de gestão e DataJud exigem monitoramento, mas detalhes agregados (TMA, resolução, uptime) não localizados.

## 5. Fail Points Identificados
- PID: Agendamento obrigatório cria paradoxo para excluídos digitais (**a 3.1**).
- Balcão Visual: Janela morta 8h–12h para usuários surdos (**a 3.2**).
- Plataforma: Divergência Meet (norma) x Zoom (prática) sem portaria explícita de migração identificada (**c pendente C.1**; tratada como incerteza em todo blueprint).
- Celeste imatura (<1 mês na pesquisa).
- Dependência de conexão e possível sobrecarga.

## 6. Balcão Visual e PID / TRT Presente
Detalhados acima, com fluxos distintos.

## 7. Canal de Atermação
Confirmado (62 3222-5570); paralelo ao Balcão Virtual.

## Quadro Síntese por Camada do Service Blueprint

**(a) Ações do Cliente**: Portal → unidade → sala videoconferência (Zoom/Meet). Celeste → direcionamento. PID: agendamento SGJ + deslocamento. TRT Presente: contato com Vara processante (interior). Balcão Visual: link dedicado 12h–16h.

**(b) Onstage/Frontstage**: Atendente em sala (regras de vestimenta/fundo); Celeste entry point; intérprete Libras no Balcão Visual.

**(c) Backstage**: Servidores de varas (escalas); Divisão Sustentabilidade (Balcão Visual); TI (plataformas); Comissão Regional PNJIID (pendente detalhamento **c C.4**).

**(d) Processos de Apoio**: Celeste (27/05/2026); PIDs + TRT Presente (parcerias TJ-GO/TRF, 153 salas); teletrabalho; Juízo 100% Digital.

**(e) Evidências Físicas**: Links portal (Zoom prático / Meet normativo); salas dedicadas Balcão Visual; PIDs físicos; salas passivas TRT Presente.

**(f) Normativos/Governança**: CNJ 372/2021; CSJT 218/2018; CSJT 428/2025 (PNJIID); Portarias 414/2021, 896/2021, 437/2022 (alterada); Res. CNJ 508/2023. (**a 4.1**: CSJT 425/2025 removida ou mantida apenas como contexto TI genérico).

**Hipóteses de Fricção**:
- Paradoxo PID (agendamento para excluídos).
- Janela morta Libras.
- Divergência normativa/plataforma (governança).
- Imaturidade Celeste; opacidade de fila; exclusão territorial mitigada por TRT Presente mas com fluxos distintos.

## Abordagem Explícita por Falha da Auditoria v2
- **1.1 Plataforma** (**a**): Histórico completo + âncora Portaria 896/2021; incerteza explícita mantida.
- **1.2 Celeste** (**a**): Data exata e imaturidade sinalizadas.
- **1.3 Balcão Visual** (**a**): Corrigido.
- **2.1 Normativos PIDs** (**a**): Incluídos.
- **2.2 Balcão Visual horário/gestão** (**a**): Corrigido.
- **2.3 CSJT 218/2018** (**a**): Incluído.
- **2.4 Parceria multiator** (**a**): TRT Presente incorporado com detalhes operacionais.
- **3.1 PID agendamento** (**a**): Corrigido.
- **3.2 Janela morta** (**a**): Corrigido.
- **3.3 Divergência normativa** (**a/c**): Reconhecida como fail point; Portaria 896/2021 adicionada como âncora provável; incerteza explícita em blueprint.
- **4.1 CSJT 425/2025** (**a**): Rebaixada/removida; substituída por 428/2025 (relevância verificada).
- **4.2 Google Forms** (**a**): Removido.
- **4.3 Teletrabalho** (**b**): Defendido com base na norma original; distinção estrutural vs. gerencial mantida como hipótese.
- **B.1 CSJT 428/2025** (**a**): Adicionada como normativo central.
- **B.2 TRT Presente** (**a**): Incorporado como canal próprio com fluxos e página dedicada.
- **B.3 Plataforma Balcão Visual** (**a**): Especificada como sala/link dedicada (distinta).
- **C.1–C.6 Pontos abertos** (**c pendente**): Listados explicitamente como lacunas para LAI/entrevistas (incluindo Comissão Regional e confirmação portaria migração).

**Lacunas Pendentes para Pesquisa Primária/LAI**:
- Portaria específica de migração Meet → Zoom (C.1).
- Detalhes escalas, scripts, indicadores DataJud, reclamações Ouvidoria.
- Comissão Regional PNJIID (C.4) e planos anuais PAIID.
- Volume/fluxo real TRT Presente vs. Balcão Virtual.

**Fontes Principais** (2021–2026): Portal TRT18 (páginas Contato, Balcão Visual, PIDs, TRT Presente), Portarias 414/2021, 896/2021, 437/2022, CSJT 428/2025, notícias institucionais. Verificação realizada em junho/2026.

Esta versão consolida o blueprint AS-IS com maior fidelidade. Recomenda-se LAI/entrevistas para backstage profundo.