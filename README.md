# gestion_courrier
Conception :
    - Service :
        Id
        Nom

    - Role :
        Id
        Nom

    - User :
        Id
        Nom
        Prenom
        IdService
        IdRole

    - Courrier :
        Id
        Reference
        Object
        Commentaire
        isFromInterne (interne/ externe)
        Expediteur (if !isFromInterne)
        IdServiceExpediteur (if isFromInterne)
        Coursier (Livreur)

    - CourrierDestinataire :
        Id
        IdCourrier
        IdServiceDestinataire

    - MouvementCourrier :
        Id
        IdUser
        action (reception) ?
        flag
        statut
        DateHeureAction

    - ModifCourrier :
        Id
        IdCourrier
        IdUserModif
        DateHeureAction
        LastValue/ NewValue

    
Fonctionnalités :
    - Back office :

    - Front office :
