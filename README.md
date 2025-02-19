# API bancária em Java
API RESTful básica para estudo de conceitos fundamentais de Java e Spring Boot

## Diagrama de classes

``` mermaid
classDiagram
    class User {
        - String name
        - Account account
        - Feature[] features
        - Card card
        - News[] news
    }
    
    class Account {
        - String number
        - String agency
        - float balance
        - float limit
    }
    
    class Card {
        - String number
        - float limit
    }
    
    class Feature {
        - String icon
        - String description
    }
    
    class News {
        - String icon
        - String description
    }
    
    User "1" *-- "1" Account
    User "1" *-- "1" Card
    User "1" *-- "n" Feature
    User "1" *-- "n" News
```
