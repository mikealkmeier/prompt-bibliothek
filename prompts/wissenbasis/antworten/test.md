# Wie visualisierst du die Teamstruktur und Verantwortlichkeiten (z.B. Organigramm, RACI-Matrix)?

Das Organigram für SAP Platform Management sieht wie folgt aus:

```mermaid
graph TB
  GT[Group Technology – Leitung: Jörg Narr]
  CCC[SAP Corporate Competence Center – Leitung: Christina Schönung]
  PLM[SAP Platform Management – Leitung: Micha Altmeyer]
  SE_MF[System Engineer – Marco Fricker]
  SE_RS[System Engineer – Rudolf Schnider]
  SE_US[System Engineer – Ulf Seiffert]
  SE_RR[System Engineer – Rubén David Reyes Blanco]
  SWE_TA[Software Engineer – Tansu Ahmedova]
  PRA_TS[Praktikant – Tanischa Seiffert]
  SE_PH[System Engineer – Philippe Haller]

  GT --> CCC
  CCC --> PLM
  PLM --> SE_MF
  PLM --> SE_RS
  PLM --> SE_US
  PLM --> SE_RR
  PLM --> SWE_TA
  PLM --> PRA_TS
  PLM --> SE_PH

```

```mermaid
flowchart TB
  %% Ebenen als Subgraphs
  subgraph GT[Group Technology]
    JN[Jörg Narr – Leitung]
  end

  subgraph CCC[SAP Corporate Competence Center]
    CS[Christina Schönung – Leitung]
  end

  subgraph PLM[SAP PLM (Platform Management)]
    MA[Micha Altmeyer – Teamleitung]
    MF[Marco Fricker – System Engineer]
    RS[Rudolf Schnider – System Engineer]
    US[Ulf Seiffert – System Engineer]
    RR[Rubén David Reyes Blanco – System Engineer]
    TA[Tansu Ahmedova – Software Engineer]
    TS[Tanischa Seiffert – Praktikant]
    PH[Philippe Haller – System Engineer]
  end

  %% Berichtslinien
  JN --> CS
  CS --> MA
  MA --> MF
  MA --> RS
  MA --> US
  MA --> RR
  MA --> TA
  MA --> TS
  MA --> PH

  %% Optionales Styling
  classDef lead fill:#e8f4ff,stroke:#2b6cb0,color:#1a365d;
  class JN,CS,MA lead;
```
