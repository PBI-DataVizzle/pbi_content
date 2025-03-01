# pbi_content
 My PowerBI Content

### mermaid

```mermaid
graph LR
    A[Start] --> B[Process AI Data]
    B --> C[Train Model]
    C --> D[Deploy Model]
    D --> E[Monitor Results]
    E --> F[Refine Model]
    F --> C
```

### vegalite

```mermaid
erDiagram
    CUSTOMER }|..|{ DELIVERY-ADDRESS : has
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER ||--o{ INVOICE : "liable for"
    DELIVERY-ADDRESS ||--o{ ORDER : receives
    INVOICE ||--|{ ORDER : covers
    ORDER ||--|{ ORDER-ITEM : includes
    PRODUCT-CATEGORY ||--|{ PRODUCT : contains
    PRODUCT ||--o{ ORDER-ITEM : "ordered in"
```

```mermaid
erDiagram LR
    User {
        Int id PK
        String username
        Int serverId FK
    }

    Server {
        Int id PK
        String serverName
    }

    Server ||--o{ User : has
```


```mermaid
graph TB
     sq[Square shape] --> ci((Circle shape))
subgraph A
         od>Odd shape]-- Two line<br/>edge comment --> ro
         di{Diamond with <br/> line break} -.-> ro(Rounded<br>square<br>shape)
         di==>ro2(Rounded square shape)
     end
%% Notice that no text in shape are added here instead that is appended further down
     e --> od3>Really long text with linebreak<br>in an Odd shape]
%% Comments after double percent signs
     e((Inner / circle<br>and some odd <br>special characters)) --> f(,.?!+-*ز)
cyr[Cyrillic]-->cyr2((Circle shape Начало));
classDef green fill:#9f6,stroke:#333,stroke-width:2px;
     classDef orange fill:#f96,stroke:#333,stroke-width:4px;
     class sq,e green
     class di orange
```

```mermaid
    gitGraph
      commit
      commit
      branch develop
      checkout develop
      commit
      commit
      checkout main
      merge develop
      commit
      commit
```
