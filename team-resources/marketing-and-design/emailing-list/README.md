# 📧 Emailing List

Emailing lists are VERY important for promoting our show! Do note, however, that we tend to divide up this task. Design and Promotion should figure out the _what_ and _when_ of the email. Technical generally figures out the _how_.

```mermaid
flowchart LR
    subgraph Design&Promotion
        direction TB
        A["Timeline"]
        B["Determine Content"]
        C["Graphic Design"]
        A --> B --> C
    end
    subgraph Technical
        direction TB
        D["Code HTML"]
        E["Send"]
        D --> E
    end
    C -.-> D
```
