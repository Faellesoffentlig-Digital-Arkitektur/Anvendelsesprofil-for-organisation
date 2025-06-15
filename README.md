# Basisprofil for organisation
Basisprofilen for organisation er en anvendelsesprofil med fokus på organisationer og organisatoriske forhold. Profilens formål er at gøre udveksling af organisationsdata mellem it-systemer mere præcis og entydig ved at anvende entydige metadata og struktur til beskrivelse af udvekslede data. 
---
title: Animal example
---
classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }
