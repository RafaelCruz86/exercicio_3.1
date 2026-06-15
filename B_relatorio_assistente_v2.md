> From: https://grok.com/c/9d33883d-6305-4c0e-ae00-6c4cee7fba3c?rid=d3d1ec82-fbb4-4047-a8c9-b459faad63ed

# grok response

**Nova Versão Corrigida: Pesquisa Pública sobre o Balcão Virtual TRT18 (AS-IS) — Junho/2026.**

Esta versão revisada aborda **todas** as 13 falhas identificadas na auditoria. Para cada uma, indico explicitamente a abordagem adotada: **(a) corrigido**, **(b) defendido** ou **(c) pendente**. O foco permanece em backstage, normativos, evidências e fail points para alimentar o Service Blueprint.

### Resumo Executivo
O Balcão Virtual do TRT18 é o canal de videoconferência para atendimento ao público externo (informações processuais), instituído em março/2021 pela Portaria TRT 18ª SGP/SGJ Nº 414/2021. Opera em paralelo com Celeste (omnichannel WhatsApp), Atermação, PID e Balcão Visual (Libras). Horário geral: 8h-16h (seg-sex). A plataforma principal evoluiu de Google Meet (padrão inicial) para Zoom (prática atual).

**1. Mapeamento do Processo Operacional Oficial**  
- **Plataforma e Fluxo** (a corrigido 1.1): A Portaria 414/2021 definiu **Google Meet como plataforma prioritária/contratada**, com fallback para Zoom ou outros. A página atual de Atendimento ao Público (2026) indica operação via **Zoom** (ícones por unidade na aba Contato; clique direto na sala). Usuário seleciona unidade → entra na sala (ordem de chegada). Formulário alternativo para registro de dados (nome, processo, contato); resposta até o dia seguinte.

  
- **Integração Canais**: Celeste (lançada **27/05/2026**) como front omnichannel (WhatsApp 62 3222-5000). Atermação (62 3222-5570).  
- **Lacuna** (c pendente): Detalhes de escalas internas, triagem na Celeste e organograma específico Balcão/PID/TI.

**2. Normativos e Governança** (a corrigido várias omissões)  
- **CNJ Res. 372/2021**: Obrigatório; similar ao presencial.  
- **CSJT Res. 218/2018** (a corrigido 2.3): Base para uso de Libras na JT; fundamento do Balcão Visual.  
- **CSJT Res. 425/2025** (c pendente 4.1): Política de Governança TI-JT; conexão ao Balcão Virtual não verificada textualmente (contexto de plataformas/SLA mantido como hipótese de apoio, não fato direto).  
- **Internos TRT18**: Portaria 414/2021 (Meet prioritário); Portaria GP/SGP 437/2022 (alterada por 1345/2023) para PIDs. Res. CNJ 508/2023 eleva PIDs a obrigação. Parcerias multiator (TJ-GO, TRF) para PIDs nível 3.
  
- **Teletrabalho** (b defendido 4.3): Portaria 414/2021 prevê explicitamente atuação remota do servidor; portarias gerais de teletrabalho reforçam o modelo (não mera especulação).  
- **Balcão Visual** (a corrigido): Gerido pela Divisão de Sustentabilidade, Acessibilidade e Inclusão (sustentabilidade@trt18.jus.br, ramais 5421/5426); servidores próprios capacitados. Parceria TRT15 refere-se ao modelo/protocolo, não provisão de intérpretes.

**3. Evidências Físicas/Digitais**  
- Portal: Links Zoom por unidade; formulário alternativo (sem confirmação "Google Forms" — removido). Balcão Visual: link Meet dedicado, 12h-16h.  
- PIDs: Agendamento obrigatório via SGJ (sgj@trt18.jus.br / 62 3222-5139). Parceria TJ-GO/TRF para nível 3 no interior.

**4. Indicadores**: Poucos públicos específicos. Lacunas persistem (c pendente).

**5. Fail Points Identificados** (a corrigido todos 3 + novos)  
- **PID**: Agendamento prévio obrigatório cria barreira para excluídos digitais (paradoxo crítico).  
- **Balcão Visual**: Horário 12h-16h gera **janela morta 8h-12h** para usuários surdos (sem Libras no Balcão padrão).  
- **Plataforma**: Divergência Meet (norma 2021) x Zoom (prática 2026) sem portaria pública de atualização identificada — fail point de governança.  
- Outros: Dependência de conexão; integração Celeste (nova, <1 mês na pesquisa); possível sobrecarga.

**6. Balcão Visual e PID**: Detalhados acima.  
**7. Atermação**: Confirmado; canal paralelo para ações verbais.

### Quadro Síntese por Camada do Service Blueprint

**(a) Ações do Cliente**: Portal → unidade → Zoom (ou formulário). Celeste/WhatsApp → direcionamento. PID: agendamento SGJ + deslocamento. Balcão Visual: link específico (12h-16h). Atermação WhatsApp.

**(b) Onstage/Frontstage**: Atendente em sala (vestimenta/fundo institucional); possível transferência. Celeste como entry point.

**(c) Backstage**: Servidores varas/PID (escalas por gestores); Divisão Sustentabilidade gerencia Balcão Visual; TI gerencia Celeste/Zoom. Parceria TRT15 (modelo).

**(d) Processos de Apoio**: Omnichannel Celeste (lançada 27/05/2026); PIDs com agendamento SGJ + parcerias multiator (TJ-GO/TRF); teletrabalho previsto.

**(e) Evidências Físicas**: Ícones/links portal; salas Zoom/Meet; PIDs físicos; cartazes/redes.

**(f) Normativos/Governança**: CNJ 372/2021; CSJT 218/2018 (Libras); Portaria 414/2021; Portaria 437/2022 (PIDs, alterada 1345/2023); Res. CNJ 508/2023; CSJT 425/2025 (TI, contexto).

**Hipóteses de Fricção Conectadas**:  
- Exclusão digital agravada por agendamento PID.  
- Janela morta Libras (8h-12h).  
- Divergência normativa/plataforma (governança).  
- Opacidade de fila/espera; Celeste imatura; Zoom Fatigue/sobrecarga; restrição informacional.

**Lacunas Principais (Pendentes para LAI/Entrevistas)**:  
- Portaria de migração Meet → Zoom.  
- Escalas internas, scripts, volume/filas reais, indicadores DataJud específicos.  
- Reclamações Ouvidoria detalhadas sobre Balcão/Celeste/PID.  
- Integração PJe/Zoom/Celeste e uptime/SLA.  
- Responsabilidades exatas TI vs. varas vs. Divisão Sustentabilidade.

**Abordagem por Falha da Auditoria (Resumo)**:  
- **1.1 Plataforma** (a): Corrigido com histórico Meet → Zoom atual.  
- **1.2 Celeste** (a): Data exata 27/05/2026 incluída; imaturidade sinalizada.  
- **1.3 Balcão Visual** (a): Parceria = modelo; servidores próprios + divisão responsável.  
- **2.1-2.4 Normativos/PIDs** (a): Adicionados Portarias 437/2022+1345/2023, Res. 508/2023, parcerias, gestão interna, agendamento.  
- **3.1-3.3 Fail Points** (a): Todos mapeados explicitamente (agendamento PID, janela morta, divergência normativa).  
- **4.1-4.3 Inferências** (a/c/b): CSJT 425 pendente textual; Google Forms removido; teletrabalho defendido pela norma original.

Esta versão fortalece a fidelidade ao AS-IS. Recomenda-se complementação via LAI/entrevistas para backstage profundo. Fontes principais: portal TRT18 (2021-2026), portarias citadas, notícias institucionais.