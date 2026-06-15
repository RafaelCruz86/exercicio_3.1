> From: https://grok.com/c/9d33883d-6305-4c0e-ae00-6c4cee7fba3c?rid=abb51432-7d75-42fb-9077-e2307449447e

# grok response

**Resumo da Pesquisa Pública sobre o Balcão Virtual TRT18 (AS-IS).**

O Balcão Virtual do TRT18 (Goiás) é um serviço de videoconferência (principalmente Zoom) para atendimento ao público sem deslocamento físico, instituído em 2021 em resposta à Resolução CNJ 372/2021. Ele opera em paralelo com outros canais como WhatsApp/Celeste (omnichannel), telefone, e-mail, PID (Pontos de Inclusão Digital) e Balcão Visual (Libras). O foco é informações processuais, com escalas por unidade judiciária (varas, CEJUSCs etc.).

**1. Mapeamento do Processo Operacional Oficial**

- **Site Oficial e Fluxo**: Acessível via https://www.trt18.jus.br/portal/fale-conosco/ ou atendimento-ao-publico. Usuário clica no ícone da unidade desejada para entrar na sala Zoom. Horário padrão: 8h-16h (seg-sex), sem agendamento prévio (por ordem de chegada, similar ao balcão físico). Há formulário alternativo para registrar nome, processo e contato se não conseguir atendimento imediato; unidade responde até o dia seguinte.

- **Portaria Reguladora Interna**: PORTARIA TRT 18ª SGP/SGJ Nº 414/2021 (17/03/2021). Define operação similar ao presencial (exceto peticionamento), uso prioritário de Google Meet (com fallback para Zoom ou outros), vestimenta adequada, fundo institucional. Atendente deve chamar especialista se necessário ou agendar. Não se aplica a gabinetes de magistrados.

- **Integração com Outros Canais**: Celeste (WhatsApp principal 62 3222-5000) atua como front omnichannel, direcionando para Balcão Virtual ou setores. Atermação (62 3222-5570 / atermacao@trt18.jus.br) é canal específico para ações verbais.

**Lacuna**: Poucos detalhes públicos sobre escalas internas de servidores, regras exatas de triagem na Celeste, ou organograma preciso de responsabilidades (TI/Celeste vs. varas vs. PID). Organograma geral disponível, mas não específico para o serviço.

**2. Normativos e Governança**

- **CNJ Res. 372/2021**: Obriga Balcão Virtual em todos os tribunais (exceto STF), durante horário de atendimento público, para contato imediato com setores de atendimento. Permite qualquer ferramenta de VC adequada. Exige similaridade ao presencial.

- **CSJT Res. 425/2025**: Política de Governança de TI na JT; menciona migração/uso de Zoom como plataforma oficial para audiências/sessões (contexto para Balcão). Foco em SLA/uptime e integração.

- **Internos TRT18**: Portaria 414/2021 (acima). Alinhado a resoluções CNJ sobre atendimento remoto durante pandemia e Juízo 100% Digital. PIDs instalados para inclusão digital.

- **Teletrabalho**: Há portarias autorizando, o que pode afetar escalas de atendimento (ex.: servidores em home office no Balcão).

**Lacuna**: Relatórios específicos de implementação da Res. 425/2025 ou indicadores DataJud detalhados para TRT18 não encontrados em buscas públicas recentes.

**3. Evidências Físicas/Digitais e Interface**

- **Portal**: Ícones por unidade na página Contato; links diretos para Zoom. Formulário alternativo (Google Forms mencionado em alguns contextos).

- **Celeste**: Bot/omnichannel via WhatsApp 62 3222-5000; integra canais e direciona (lançada ~2026).

- **Balcão Visual (Libras)**: Parceria com TRT15 (Campinas). Acessível via aba Contato; atendimento com intérprete. Horários limitados (ex.: 12h-16h em modelos semelhantes).

- **PID**: Pontos físicos para acesso à internet/serviço; instalados em 2022 para inclusão.

- **Divulgação**: Posts em redes, vídeos institucionais, cartazes (discurso de acessibilidade e praticidade).

**4. Indicadores e Desempenho**

Poucos dados públicos específicos. Estatísticas gerais de gestão/estatísticas no site TRT18 (volume atendimentos, metas CNJ/CSJT). Não localizados relatórios detalhados de TMA (tempo médio atendimento), resolução no 1º contato ou uptime Zoom/Celeste para Balcão. Metas CNJ via DataJud exigem indicadores.

**Lacuna grande**: Ausência de relatórios públicos recentes de desempenho específicos do Balcão Virtual.

**5. Fail Points e Vozes Críticas**

- **Reclamações Ouvidoria**: Canal ativo (https://www.trt18.jus.br/portal/ouvidoria/), com relatórios estatísticos. Não há dados agregados públicos destacando Balcão/Zoom como problema principal nas buscas.

- **Outros**: Buscas por reclamações específicas (indisponibilidade Zoom, filas, Celeste) não retornaram matérias ou ofícios públicos massivos recentes sobre TRT18. Comparações com outros TRTs mostram desafios comuns (Zoom Fatigue, sobrecarga, exclusão digital). PIDs visam mitigar acesso. OAB-GO e sindicatos não têm manifestações públicas recentes destacadas sobre o serviço.

- **Hipóteses de Fricção**: Opacidade de fila (sem agendamento visível), dependência de conexão/internet, limitação de intérpretes Libras, possível sobrecarga de servidores em horários de pico, integração Celeste-PJe-Zoom.

**Lacuna**: Poucos relatos públicos críticos ou estatísticas de falhas; necessário LAI ou entrevistas para profundidade.

**6. Balcão Visual e PID**

- **Libras**: Parceria TRT15; protocolo via portal, ordem de chegada ou agendamento limitado. Foco em acessibilidade.

- **PID**: Unidades físicas para usuários sem internet; apoio ao Balcão Virtual.

**7. Canal de Atermação**

Confirmado: WhatsApp/Telefone (62) 3222-5570, e-mail atermacao@trt18.jus.br. Articula-se como canal paralelo/específico para propositura de ações verbais; pode encaminhar para Balcão se necessário. Horário 8h-16h.

### Quadro Síntese por Camada do Service Blueprint

**(a) Ações do Cliente**: Acesso portal → escolher unidade → Zoom (ou WhatsApp Celeste → direcionamento) ou PID físico. Formulário fallback. Para Libras: Balcão Visual. Atermação via WhatsApp específico.

**(b) Onstage/Frontstage**: Atendente em sala Zoom (vestimenta/fundo institucional), conversa em tempo real, possível transferência para especialista. Celeste como entry point amigável.

**(c) Backstage**: Servidores de varas/PID designados por escalas (gestores de vara); TI gerencia Celeste/Zoom; integração com PJe. Parceria TRT15 para Libras.

**(d) Processos de Apoio**: Omnichannel Celeste, formulário alternativo, PIDs, teletrabalho. Governança via portarias e resoluções CNJ/CSJT.

**(e) Evidências Físicas**: Ícones/links no portal, salas Zoom institucionais, PIDs físicos, cartazes/redes sociais.

**(f) Normativos/Governança**: CNJ 372/2021, Portaria TRT18 414/2021, CSJT 425/2025 (TI), portarias teletrabalho.

**Hipóteses de Fricção Conectadas**:
- Exclusão digital (mitigada por PID, mas limitada).
- Opacidade/espera (sem fila visível, dependência de ordem de chegada).
- Zoom Fatigue/sobrecarga servidores.
- Restrição informacional (servidores limitados a informações, não atos processuais complexos).
- Integração canais (Celeste → Balcão).

**Lacunas Principais para Pesquisa Primária/LAI**:
- Detalhes operacionais internos (escalas, scripts de atendimento, regras Celeste, volume/filas reais).
- Indicadores de desempenho (uptime, TMA, resolução, reclamações específicas).
- Fail points internos (indisponibilidades, integração PJe/Zoom, sobrecarga).
- Responsabilidades exatas TI vs. varas vs. Corregedoria.
- Relatos de usuários/sindicatos/OAB mais profundos.

Fontes principais: Site TRT18 (2021-2026), Portaria 414/2021, Res. CNJ 372, notícias institucionais. Pesquisa realizada em junho/2026; recomendo verificação de atualizações. Esta base alimenta o Blueprint AS-IS; complemente com entrevistas.