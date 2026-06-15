# Diagrama AS-IS — Balcão Virtual TRT18

**Metodologia:** Service Blueprint Shostack | **Base:** C_blueprint_asis.md
**Leitura:** etapas (azul) → atores e processos de suporte (amarelo) → fail points (vermelho) → desfecho (roxo)

---

```mermaid
flowchart TD
    %% ── E1: Acesso ao Portal ──────────────────────────────────────────
    TI1["TI TRT18\nportal"] --> E1
    PJe1["PJe · hospedagem"] --> E1
    E1["E1 · Acesso ao Portal\ntrt18.jus.br — aba Contato"]

    %% ── E2: Seleção de Canal ──────────────────────────────────────────
    E1 --> E2{"E2 · Seleção de Canal"}
    GEST["Gestores de varas\nescalas de atendimento"] --> E2
    E2 -.-> FP2(["⚠️ FP2 · Paradoxo PID\ninclusão exige digital\nE2 · Canal PID"])

    %% ── Bifurcação ────────────────────────────────────────────────────
    E2 -->|"Balcão Virtual"| BV3
    E2 -->|"Celeste / WhatsApp"| CEL3
    E2 -->|"PID Interno"| PID3
    E2 -->|"TRT Presente"| TRP3
    E2 -->|"Balcão Visual"| BVL3

    %% ── Canal: Balcão Virtual / Zoom ──────────────────────────────────
    BV_TI["TI TRT18\nZoom / Meet"] --> BV3
    BV3["E3-BV · Ingresso\nsala Zoom"]
    BV3 -.-> FP1(["⚠️ FP1 · Meet × Zoom\ndivergência normativa\nE3 · BV"])
    BV3 -.-> FP5(["⚠️ FP5 · Fila opaca\nsem info de espera\nE3 · BV"])
    BV3 --> BV4["E4-BV · Interação\nServidor TRT18 em vídeo"]
    BV4 --> BV5["E5-BV · Desfecho"]

    %% ── Canal: Celeste / WhatsApp ─────────────────────────────────────
    CEL_PLAT["Plataforma Celeste\nlançada 27/05/2026"] --> CEL3
    CEL3["E3-CEL · Ingresso\nWhatsApp / chat"]
    CEL3 --> CEL4["E4-CEL · Interação\nChatbot Celeste"]
    CEL4 -.-> FP4(["⚠️ FP4 · Celeste imatura\n< 1 mês em operação\nE4 · CEL"])
    CEL4 --> CEL5["E5-CEL · Desfecho"]

    %% ── Canal: PID Interno ────────────────────────────────────────────
    SGJ["Sistema SGJ\nagendamento prévio"] --> PID3
    PID3["E3-PID · Ingresso\nPID presencial"]
    PID3 --> PID4["E4-PID · Interação\nServidor TRT18 presencial"]
    PNJIID["Comissão Regional\nPNJIID [lacuna C.4]"] -.-> PID4
    PID4 --> PID5["E5-PID · Desfecho"]

    %% ── Canal: TRT Presente ───────────────────────────────────────────
    TJGO["Parceria TJ-GO / TRF\n153 salas passivas"] --> TRP3
    TRP3["E3-TRP · Ingresso\nsala passiva TJ-GO"]
    TRP3 --> TRP4["E4-TRP · Interação\nServidor TRT18\nem sala passiva"]
    TRP4 --> TRP5["E5-TRP · Desfecho"]

    %% ── Canal: Balcão Visual / Libras ─────────────────────────────────
    DSAI["Divisão de Sustentabilidade\nAcessibilidade e Inclusão"] --> BVL3
    BVL3["E3-BVL · Ingresso\nlink Libras — 12h às 16h"]
    BVL3 -.-> FP3(["⚠️ FP3 · Janela morta Libras\nindisponível 8h–12h\nE3 · BVL"])
    BVL3 --> BVL4["E4-BVL · Interação\nIntérprete de Libras\n+ Servidor TRT18"]
    BVL4 --> BVL5["E5-BVL · Desfecho"]

    %% ── PJe: processo de suporte transversal ──────────────────────────
    PJe["PJe\nconsulta processual\ntransversal"]
    PJe --> BV4
    PJe --> CEL4
    PJe --> PID4
    PJe --> TRP4
    PJe --> BVL4

    %% ── Convergência no Desfecho Final ────────────────────────────────
    BV5 & CEL5 & PID5 & TRP5 & BVL5 --> FINAL[/"Desfecho Final\nProtocolo emitido · Informação obtida\nou Encaminhamento confirmado"/]

    %% ── Estilos ───────────────────────────────────────────────────────
    classDef etapa    fill:#dbeafe,stroke:#2563eb,color:#1e3a5f
    classDef suporte  fill:#fef9c3,stroke:#ca8a04,color:#713f12
    classDef failpoint fill:#fee2e2,stroke:#dc2626,color:#7f1d1d
    classDef desfecho fill:#f3e8ff,stroke:#7c3aed,color:#2e1065

    class E1,E2,BV3,BV4,BV5,CEL3,CEL4,CEL5,PID3,PID4,PID5,TRP3,TRP4,TRP5,BVL3,BVL4,BVL5 etapa
    class TI1,PJe1,PJe,BV_TI,CEL_PLAT,SGJ,TJGO,DSAI,GEST,PNJIID suporte
    class FP1,FP2,FP3,FP4,FP5 failpoint
    class FINAL desfecho
```

---

## Legenda

| Cor | Significado |
|---|---|
| Azul | Etapas da jornada (E1–E5) na ótica do cidadão |
| Amarelo | Atores de backstage e processos de suporte |
| Vermelho | Fail points (⚠️ FP1–FP5) — setas tracejadas indicam o ponto de falha |
| Roxo | Desfecho final convergente |

## Leitura do Diagrama

| Elemento | Interpretação |
|---|---|
| Seta sólida `→` | Fluxo normal da jornada ou ação de suporte |
| Seta tracejada `-.->` | Relação de falha potencial ou ator não confirmado [lacuna] |
| Nó de decisão `{ }` | Ponto de bifurcação (E2: seleção de canal) |
| Nó paralelo `[/ /]` | Desfecho convergente (todos os canais chegam aqui) |
| `[lacuna C.4]` | Ator previsto normativamente mas não verificado publicamente |

## Fail Points — Resumo Posicional

| FP | Posição no Diagrama | Canal |
|---|---|---|
| FP1 Meet × Zoom | E3-BV → saída tracejada | Balcão Virtual |
| FP2 Paradoxo PID | E2 → saída tracejada | PID Interno |
| FP3 Janela morta Libras | E3-BVL → saída tracejada | Balcão Visual |
| FP4 Celeste imatura | E4-CEL → saída tracejada | Celeste/WhatsApp |
| FP5 Fila opaca | E3-BV → saída tracejada | Balcão Virtual |
