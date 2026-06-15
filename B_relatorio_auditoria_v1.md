# Auditoria: Pesquisa sobre o Balcão Virtual TRT18 (AS-IS)

> Auditoria realizada em junho/2026 com base em fontes primárias do portal TRT18, Portaria 414/2021, notícias institucionais e normativos CNJ/CSJT.
> Não foram consideradas falhas cosméticas (formatação, estilo, ordem de seções).

---

## Resumo executivo

| Categoria | Quantidade |
|---|---|
| Erros factuais | 3 |
| Omissões relevantes (backstage / normativos) | 4 |
| Fail points não mapeados | 3 |
| Inferências mal-suportadas / fontes fracas | 3 |
| **Total** | **13** |

---

## 1. Erros Factuais

### 1.1 Plataforma primária: Google Meet, não Zoom

**Trecho do relatório auditado:**
> "O Balcão Virtual do TRT18 (Goiás) é um serviço de videoconferência (principalmente Zoom)" / "uso prioritário de Google Meet (com fallback para Zoom ou outros)"

**Justificativa:**
O relatório é contraditório internamente, e o primeiro enunciado é factualmente incorreto. A Portaria 414/2021 e a notícia de lançamento do TRT18 são explícitas: **a plataforma contratada e definida como padrão é o Google Meet**. O Zoom é mencionado como alternativa de fallback, não como plataforma primária.

A página atual de Atendimento ao Público do TRT18 descreve o Balcão Virtual como operando via Zoom — o que sugere migração posterior —, mas o relatório não verifica esse ponto e abre com uma afirmação tecnicamente errada para o período de instituição do serviço. Isso configura também um **fail point de governança não identificado** (ver seção 3.3).

**Fonte:** Notícia de lançamento TRT18 (18/03/2021); Portaria TRT 18ª SGP/SGJ nº 414/2021.

---

### 1.2 Data de lançamento da Celeste: 27/05/2026, não "~2026"

**Trecho do relatório auditado:**
> "Celeste (WhatsApp principal 62 3222-5000) atua como front omnichannel, direcionando para Balcão Virtual ou setores. (lançada ~2026)"

**Justificativa:**
A data é precisa e verificável: a Celeste foi lançada em **27 de maio de 2026**, conforme notícia publicada no portal do TRT18. Tratar como aproximada ("~2026") sugere incerteza onde ela não existe. Mais grave: o relatório usa a Celeste como referência operacional de integração sem sinalizar que a plataforma tinha menos de um mês de existência na data da pesquisa (junho/2026), o que compromete qualquer análise de maturidade do canal.

**Fonte:** TRT18, "Celeste dá boas-vindas: TRT-GO lança plataforma que integra canais e moderniza atendimento", publicado em 27/05/2026.

---

### 1.3 Balcão Visual: parceria com TRT15 é de modelo, não de provisão de intérpretes

**Trecho do relatório auditado:**
> "Balcão Visual (Libras): Parceria com TRT15 (Campinas). [...] contará com intérpretes de Libras capacitados."

**Justificativa:**
A parceria com o TRT15 se refere ao **modelo/protocolo** do serviço, não à provisão de intérpretes ou pessoal. A página oficial do Balcão Visual do TRT18 indica que o atendimento é "feito por servidores capacitados" do próprio TRT18, gerido pela **Divisão de Sustentabilidade, Acessibilidade e Inclusão** (contato: sustentabilidade@trt18.jus.br, ramais 5421/5426). O TRT15 criou o conceito e o TRT18 aderiu ao modelo — isso é diferente de uma parceria operacional em que o TRT15 fornece pessoal.

**Fonte:** Portal TRT18, página "Balcão Visual" (atualizado em 17/07/2025); notícia de lançamento do Balcão Visual no TRT18.

---

## 2. Omissões Relevantes (Backstage e Normativos)

### 2.1 Normativos dos PIDs incompletos: Portaria 437/2022 e Resolução CNJ 508/2023

**Trecho do relatório auditado:**
> "PIDs: instalados em 2022 para inclusão. Atende a Recomendação CNJ nº 130/2022."

**Justificativa:**
O relatório cita corretamente a Recomendação CNJ 130/2022, mas omite dois normativos fundamentais:

- **Portaria TRT 18ª GP/SGP nº 437/2022** (alterada pela Portaria nº 1345/2023): rege os PIDs internamente, define níveis e responsabilidades.
- **Resolução CNJ nº 508/2023**: elevou os PIDs de recomendação a **obrigação normativa**.

Esses documentos definem o **fluxo de agendamento via SGJ** (e-mail sgj@trt18.jus.br / telefone 62 3222-5139), que é um processo de backstage crítico completamente ausente do blueprint.

**Fonte:** Portal TRT18, página "Pontos de Inclusão Digital (PIDs)" (atualizado em 26/03/2026); Portal CNJ, página "Ponto de Inclusão Digital – PID".

---

### 2.2 Balcão Visual: horário oficial tratado como estimativa; gestão interna omitida

**Trecho do relatório auditado:**
> "Balcão Visual (Libras): [...] Horários limitados (ex.: 12h-16h em modelos semelhantes)."

**Justificativa:**
O horário não é um "exemplo em modelos semelhantes" — é o horário **confirmado e publicado pelo próprio TRT18**: segunda a sexta, das 12h às 16h, exceto feriados. Apresentá-lo como estimativa introduz incerteza desnecessária onde há dado verificável.

Mais grave é a omissão do backstage: o serviço é gerido pela **Divisão de Sustentabilidade, Acessibilidade e Inclusão** (ramais 5421/5426), unidade administrativa com identidade distinta das varas e da TI. Essa linha de responsabilidade é relevante para o blueprint AS-IS.

**Fonte:** Portal TRT18, páginas "Atendimento ao Público" e "Balcão Visual" (atualizado em 17/07/2025).

---

### 2.3 Resolução CSJT 218/2018 sobre Libras ausente da cadeia normativa

**Trecho do relatório auditado:**
> [Seção "Normativos e Governança" não cita a resolução]

**Justificativa:**
A **Resolução CSJT nº 218/2018**, que dispõe sobre uso de Libras na Justiça do Trabalho para atendimento de pessoas surdas, é o normativo setorial fundador do Balcão Visual — antecede e complementa a Resolução CNJ 401/2021. Sua ausência cria uma lacuna na cadeia normativa da seção de governança, especialmente relevante para o mapeamento do Balcão Visual.

**Fonte:** Notícia de lançamento do Balcão Visual no TRT15 (TRT-15, 2023), que cita expressamente a Res. CSJT 218/2018 como base normativa do serviço.

---

### 2.4 Parceria multiator TRT18 + TJ-GO + TRF para PIDs de nível 3 ausente do backstage

**Trecho do relatório auditado:**
> "PIDs: Pontos físicos para acesso à internet/serviço; instalados em 2022 para inclusão."

**Justificativa:**
Os PIDs do TRT18 têm níveis operacionais distintos. Os de **nível 3** (que suportam atos processuais completos) resultam de um **Termo de Cooperação Técnica com o TJ-GO, TRF e outros órgãos** (firmado em abril de 2023), usando infraestrutura de prédios do TJ-GO nos municípios sem Vara do Trabalho. Esse arranjo multiator é um processo de apoio (support process) central no blueprint do atendimento no interior do Estado e está completamente omitido.

**Fonte:** TRT18, "TRT de Goiás e Tribunal de Justiça firmam parceria para facilitar acesso à Justiça no interior" (24/04/2023).

---

## 3. Fail Points Não Identificados

### 3.1 PID exige agendamento prévio — barreira invisível ao usuário

**Trecho do relatório auditado:**
> "PID: Pontos físicos para acesso à internet/serviço; instalados em 2022 para inclusão." / "Exclusão digital (mitigada por PID, mas limitada)."

**Justificativa:**
O relatório trata os PIDs como canal de acesso espontâneo, mas o portal do TRT18 é explícito: o acesso a um PID **exige agendamento prévio com a SGJ** (e-mail sgj@trt18.jus.br / telefone 62 3222-5139). Isso cria um **paradoxo operacional crítico**: o canal destinado a incluir quem não tem acesso digital exige que o usuário realize agendamento — processo que, para um excluído digital, já representa a barreira que o canal deveria eliminar.

Este é provavelmente o fail point de acessibilidade mais grave não mapeado no relatório.

**Fonte:** TRT18, "TRT de Goiás e Tribunal de Justiça firmam parceria..." (24/04/2023); Portal TRT18, página "Pontos de Inclusão Digital (PIDs)".

---

### 3.2 Janela morta de 4 horas para usuários surdos (8h–12h)

**Trecho do relatório auditado:**
> [Ausente no mapeamento de fail points]

**Justificativa:**
O Balcão Virtual geral funciona das **8h às 16h**; o Balcão Visual funciona das **12h às 16h**. Há uma **janela de quatro horas diárias** (8h–12h) em que um usuário surdo não tem canal de atendimento adaptado disponível. Se tentar acessar o Balcão Virtual padrão nesse horário, não terá suporte em Libras.

O relatório lista o horário do Balcão Visual como "limitado", mas não identifica que essa limitação cria uma lacuna operacional concreta com impacto diferenciado por tipo de usuário — o que é exatamente o tipo de fail point que um service blueprint deve capturar.

**Fonte:** Portal TRT18, páginas "Atendimento ao Público" e "Balcão Visual".

---

### 3.3 Divergência normativa não investigada: Meet → Zoom sem portaria de atualização

**Trecho do relatório auditado:**
> "Portaria TRT 18ª SGP/SGJ Nº 414/2021 [...] uso prioritário de Google Meet (com fallback para Zoom ou outros)"

**Justificativa:**
A Portaria 414/2021 define o Google Meet como plataforma contratada e padrão. A página atual de Atendimento ao Público do TRT18 descreve o Balcão Virtual como operando via Zoom. O relatório não identifica essa **divergência entre normativo e prática atual**, nem investiga se houve portaria de atualização.

Trata-se de um fail point de governança: normativo possivelmente desatualizado em relação à operação real, com implicações para SLA, suporte técnico e responsabilidade institucional.

**Fonte:** Portaria 414/2021; Portal TRT18, página "Atendimento ao Público" (atualizada em 2026).

---

## 4. Inferências Mal-Suportadas / Fontes Fracas

### 4.1 CSJT Res. 425/2025 vinculada ao Balcão Virtual sem evidência textual

**Trecho do relatório auditado:**
> "CSJT Res. 425/2025: Política de Governança de TI na JT; menciona migração/uso de Zoom como plataforma oficial para audiências/sessões (contexto para Balcão). Foco em SLA/uptime e integração."

**Justificativa:**
O relatório conecta a Res. CSJT 425/2025 ao Balcão Virtual sem demonstrar que o normativo efetivamente o menciona ou regula. A descrição é vaga ("contexto para Balcão") e a afirmação sobre "migração/uso de Zoom como plataforma oficial" não é corroborada por fonte citada. Sem acesso verificado ao texto da resolução, trata-se de **inferência especulativa apresentada como fato normativo**.

---

### 4.2 "Google Forms mencionado em alguns contextos" — fonte não identificada

**Trecho do relatório auditado:**
> "Portal: Ícones por unidade na página Contato; links diretos para Zoom. Formulário alternativo (Google Forms mencionado em alguns contextos)."

**Justificativa:**
A expressão "mencionado em alguns contextos" não constitui fonte. O portal oficial do TRT18 (página Contato, atualizada em 26/03/2026) descreve o formulário de fallback sem especificar que é Google Forms. Incluir o nome da ferramenta com essa ressalva cria uma imprecisão sem valor informativo e sem base verificável.

---

### 4.3 Teletrabalho como fator de escala: hipótese rasa e não desenvolvida

**Trecho do relatório auditado:**
> "Teletrabalho: Há portarias autorizando, o que pode afetar escalas de atendimento (ex.: servidores em home office no Balcão)."

**Justificativa:**
A existência de portarias de teletrabalho no TRT18 é fato, mas a inferência de que isso "pode afetar escalas de atendimento" do Balcão Virtual especificamente é especulação não desenvolvida. A Portaria 414/2021 já prevê expressamente que "cada sala terá pelo menos um servidor, que **poderá atuar de forma remota**" — o atendimento remoto é parte do modelo original, não uma variável inesperada do teletrabalho. A hipótese é legítima como investigação futura, mas não deve figurar como achado sem maior substância.

---

## Conclusão

As falhas mais graves para a validade do blueprint AS-IS são:

1. **Erro de plataforma** (Google Meet vs. Zoom) compromete a descrição técnica do serviço desde a sua fundação.
2. **PIDs com agendamento obrigatório omitido** inverte a lógica de inclusão do canal: o backstage real não está mapeado.
3. **Divergência normativa Meet → Zoom não investigada** deixa em aberto uma questão de governança com impacto operacional.
4. **Janela morta de 4h para usuários surdos** é o fail point de acessibilidade mais crítico ausente do mapeamento.
5. **Parceria multiator para PIDs de nível 3** é um processo de suporte inteiro faltando no blueprint do atendimento no interior.

Para completar o blueprint AS-IS com fidelidade, recomenda-se LAI sobre: portaria de migração de plataforma (se existente), escalas de atendimento por unidade, e volume de uso dos PIDs vs. Balcão Virtual direto.

---

*Auditoria realizada em junho/2026. Fontes: portal TRT18 (trt18.jus.br), Portaria 414/2021, notícias institucionais TRT18, portal CNJ.*
