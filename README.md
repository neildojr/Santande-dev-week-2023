# Santande Dev Week-2023
Java RESTful API criada para a Santander Dev Week

## Diagrama de Classes

```mermaid
classDiagram
    class Usuario {
        - String name
        - Account account
        - List<Feature> feature
        - Card card
        - List<News> news
    }
    class Account {
        - String number
        - String agency
        - Double balance
        - Double limite
    }
    class Feature {
        - String icon
        - String description
    }
    class Card {
        - String number
        - Double limit
    }
    class News {
        - String icon
        - String description
    }

    Usuario "1" *--> "1" Account
    Usuario "1" *--> "N" Feature
    Usuario "1" *--> "1" Card
    Usuario "1" *--> "N" News
```
