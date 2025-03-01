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

%%{init: {
  "theme": "default",
  "themeCSS": [
    ".er.relationshipLabel { fill: black; }", 
    ".er.relationshipLabelBox { fill: white; }", 
    ".er.entityBox { fill: lightgray; }",
    "[id^=entity-some] .er.entityBox { fill: lightgreen;} ",
    "[id^=entity-mytable] .er.entityBox { fill: powderblue;} ",
    "[id^=entity-anothertable] .er.entityBox { fill: pink;} "
    ]
}}%%
