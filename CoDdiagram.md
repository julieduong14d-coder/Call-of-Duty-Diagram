flowchart LR
  %% Main horizontal spine
  Confrontation --> USA["USA"]
  USA --> China["China"]
  China --> Russia["Russia"]
  Russia --> Helios["Helios"]
  Helios --> Neutrals["Neutral Countries<br/>(Switzerland, Austria, Ireland, etc.)"]

  %% Alliances as subtasks under each power
  USA -->|Allies| WA["Western Allies<br/>(NATO, US–Japan, AUKUS, Five Eyes)"]
  China -->|Alliance| SCO["SCO<br/>(Shanghai Cooperation O.)"]
  China -->|Alliance| BRICS["BRICS"]
  Russia -->|Alliance| CSTO["CSTO<br/>(Collective Security Treaty O.)"]
  Russia --> BRICS

  %% Tuck the alliance boxes neatly under the spine
  style WA    stroke:#888,stroke-width:1px,fill:#f9f,rx:4
  style SCO   stroke:#888,stroke-width:1px,fill:#f9f,rx:4
  style BRICS stroke:#888,stroke-width:1px,fill:#f9f,rx:4
  style CSTO  stroke:#888,stroke-width:1px,fill:#f9f,rx:4

  %% Shift alliances downward
  WA   ---|       | USA   
  SCO  ---|       | China 
  BRICS---|       | China, Russia
  CSTO ---|       | Russia
