```mermaid
graph LR
    Protocole -- utilise --> Réseau
    TCP -- est_un_type --> Protocole
    IP -- se_base --> TCP
    IPv4 -- est_une_implémentation_32bits --> IP
    IPv6 -- est_une_implémentation_64bits --> IP
    HTTP -- est_un_type --> Protocole
    Requête -- est_émise --> HTTP
    GET -- est_un_verbe --> Requête
    POST -- est_un_verbe --> Requête
    Réponse -- est_retournée --> HTTP
    200 -- est_un_code_de_retour --> Réponse
    404 -- est_un_code_de_retour --> Réponse

    Équipement -- est_connecté --> Réseau
    Routage -- est_un_type --> Équipement
    Switch -- s'occupe --> Routage
    Sécurité -- est_un_type --> Équipement
    Pare-feu -- s'occupe --> Sécurité

    Léger -- est_un_type --> Client
    Navigateur[Navigateur web] -- est_un_type --> Léger
    Chrome -- est --> Navigateur
    Firefox -- est --> Navigateur
    Lourd -- est_un_type --> Client
    Logiciel -- est_un_type --> Lourd

    Frontal[Serveur web] -- est_un_type --> Serveur
    IIS -- est --> Frontal
    Nginx -- est --> Frontal
    BDD[Serveur de base de données] -- est_un_type --> Serveur
    MySQL -- est --> BDD
    SQLServer -- est --> BDD
    Cache[Serveur cache] -- est_un_type --> Serveur
    Redis -- est --> Cache
    Memcached -- est --> Cache

```