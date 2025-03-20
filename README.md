###Diagrama de Classes 

--- mermaid

classDiagram
    class User {
        - string name
    }
    
    class Account {
        - string number
        - string agency
        - float balance
        - float limit
    }
    
    class Card {
        - string number
        - float limit
    }
    
    class Feature {
        - string icon
        - string description
    }
    
    class News {
        - string icon
        - string description
    }

    User --> Account
    User --> Card
    User --> "0..*" Feature
    User --> "0..*" News
