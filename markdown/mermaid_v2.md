```mermaid
graph LR
    Protocole -- utilise --> Réseau
    TCP -- est_un_type --> Protocole
    IP -- peut_utiliser --> TCP
    IP -- est_un_type --> Protocole
    IPv4 -- est_une_implémentation_32bits --> IP
    IPv6 -- est_une_implémentation_64bits --> IP
    HTTP -- est_un_type --> Protocole
    Requête -- est_émise --> HTTP
    GET -- est_un_verbe --> Requête
    POST -- est_un_verbe --> Requête
    Réponse -- est_retournée --> HTTP
    200 -- est_un_code_de_retour --> Réponse
    404 -- est_un_code_de_retour --> Réponse

    Équipement --> Réseau
    Routage --> Équipement
    Switch --> Routage
    Sécurité --> Équipement
    Pare-feu --> Sécurité

    Chrome --> Navigateur
    Firefox --> Navigateur
    Navigateur[Navigateur web] --> Client
    Logiciel --> Client
    Client --> Réseau

    Frontal[Serveur web] --> Serveur
    IIS --> Frontal
    Nginx --> Frontal
    BDD[Serveur de base de données] --> Serveur
    MySQL --> BDD
    SQLServer --> BDD
    Cache[Serveur cache] --> Serveur
    Redis --> Cache
    Memcached --> Cache
    Serveur --> Réseau

```