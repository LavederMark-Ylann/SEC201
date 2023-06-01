```mermaid
graph LR
    Protocole --> Réseau
    TCP --> Protocole
    IP --> TCP
    HTTP --> Protocole
    Requête --> HTTP
    Réponse --> HTTP

    Équipement --> Réseau
    Routage --> Équipement
    Switch --> Routage
    Sécurité --> Équipement
    Pare-feu --> Sécurité

    Léger --> Client
    Navigateur[Navigateur web] --> Léger
    Lourd --> Client
    Logiciel --> Lourd

    Frontal[Serveur web] --> Serveur
    BDD[Serveur de base de données] --> Serveur
    Cache[Serveur cache] --> Serveur

```