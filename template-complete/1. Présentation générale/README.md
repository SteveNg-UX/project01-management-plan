# I. Présentation générale
- [I.1 Client](#i1-client)
- [I.2 Contexte](#i2-contexte)
- [I.3 Problématique](#i3-problématique)
- [I.4 Besoins / Objectifs](#i4-besoins--objectifs)
- [I.5 Périmètre du projet](#i5-périmètre-du-projet)
- [I.6 Livrables attendus](#i6-livrables-attendus)

---

## I.1 Client
- Explication : presente le client concerné par le projet
- Etape :

    Présenter l'entreprise client comprend 3 élements:
    - Info général
    - Type d'entreprise
    - Secteur d'activité

    | Element           | Valeur                                |
    |:----------------- |:------------------------------------- |
    |Entreprise         | (Nom)                                 |
    |Effectif           | (N) Personnels                        |
    |Chiffre d'Affaire  | (N) € /ans                            |
    |Type               | (type)                                |
    |Lieux              | (Adresse, Ville, Département, Pays)   |
    |Année d'existance  | (N) Ans                               |
    |Secteur d'activité | (Spécialité)                          |

    |Type d'Entreprise  |Nom Complet                        |Effectif   |Chiffre d'Affaire      |
    |:----------------- |:--------------------------------- |:--------- |:--------------------- |
    |TPE                | Très Petit Entreprise             | < 10      | <= 2M € /ans          |
    |PME                | Petit Moyen Entreprise            | 10-249    | 2M € - 50M € /ans     |
    |ETI                | Entreprise Taille Intermédiaire   | 250-4999  | 50M € - 1,5Md € /ans  |
    |GE                 | Grande Entreprise                 | >= 5000   | > 1,5Md € /ans        |

    |Secteur d'Activité                                     |
    |:------------------------------------------------------|
    |Agriculture                                            |
    |Armées, sécurité et défense publique                   |
    |Bâtiment - Travaux publics                             |
    |Commerce et distribution                               |
    |Emploi public                                          |
    |Énergie                                                |
    |Hôtellerie - Restauration (HCRB)                       |
    |Industrie                                              |
    |Industrie agroalimentaire                              |
    |Industrie automobile                                   |
    |Industrie pharmaceutique                               |
    |Industrie textile                                      |
    |Luxe                                                   |
    |Maritime et fluvial                                    |
    |Numérique et télécommunications                        |
    |Santé humaine, action sociale, services à la personne  |
    |Services automobiles                                   |
    |Tourisme                                               |
    |Transport - Logistique                                 |

---

## I.2 Contexte
- Explication : expliquer la situation / etat actuelle
- Etape :

    Présenter le contexte du client comprend 3 élements:

    | Présenter le contexte                                     |
    |:----------------------------------------------------------|
    | Etat initial du SI                                        |
    | Etat actuelle du SI                                       |
    | Plans d’analyse                                           |

    | Plans d’analyse   |
    |:------------------|
    | Politique         |
    | Économique        |
    | Socioculturel     |
    | Technologique     |
    | Écologique        |
    | Légal             |

---

## I.3 Problématique
- Explication : exprimer le problème dont le SI fait face

| Caracteristique                   |
|:----------------------------------|
| Unique                            |
| Formulée sous forme de question   |
| Liée à un enjeu métier ou SI      |

---

## I.4 Besoins / Objectifs
- Explication : exprime ce qu’il faut pour répondre au problèmatique
- Etape :

    Les besoins et les obectifs sont définit selon les critaires suivant :

    | Caracteristique       | Detail                                                                |
    |:--------------------- |:--------------------------------------------------------------------- |
    | Besoins fonctionnels  | ce que l’utilisateur veut faire                                       |
    | Besoins techniques    | performance, sécurité…                                                |

    | Besoin Fonctionnel        |
    |:--------------------------|
    | Ce que veut faire le User |

    | Besoins Techniques    | Description                                           | Exemple                                                   |
    |:----------------------|:------------------------------------------------------|:----------------------------------------------------------|
    | Disponibilité         |Le service doit être accessible quand on en a besoin   |99,9 % de dispo                                            |
    | Sécurité              |Protéger les données et les accès                      |Authentification forte                                     |
    | Fiabilité             |Fonctionner sans erreur ni panne                       |Taux d’incidents faible                                    |
    | Performance           |Répondre vite et supporter la charge                   |Temps de réponse < 200 ms                                  |
    | Flexibilité           |S’adapter facilement aux changements                   |Ajouter une nouvelle fonctionnalité sans casser l’existant |
    | Agilité               |Permettre des évolutions rapides                       |Déploiements fréquents                                     |
    | Durabilité            |Rester viable et maintenable dans le temps             |Techno supportée 5+ ans                                    |
    | Economie              |Optimiser les coûts de développement et d’exploitation |Mutualisation des Actifs                                   |
    
    | Objectifs SMART   | Description                                   | Exemple                                   |
    |:------------------|:----------------------------------------------|:------------------------------------------|
    | Spécifique        |Définir précisément ce que l’on veut atteindre |Une authentification forte pour les users  |
    | Mesurable         |Pouvoir vérifier l’atteinte de l’objectif      |95 % des connexions doivent utiliser la PKI|
    | Atteignable       |Objectif réaliste selon les moyens disponibles |Équipe de 3 devs + 1 PO                    |
    | Réaliste          |Cohérent avec le contexte et les contraintes   |Budget validé par la DSI                   |
    | Temporel          |Définir une échéance claire                    |Déploiement prévu en 3 mois                |

    Lister les besoins et les classer

    | ID    | Description Besoin Fonctionnel                    | Description Besoin Technique      | Spécifique                | Mesurable                 | Atteignable           | Réaliste          | Temporel  |
    |:------|:--------------------------------------------------|:----------------------------------|:--------------------------|:--------------------------|:----------------------|:------------------|:----------|
    |B1     |Renforcer la sécurité des accès wifi               |Déploiment de portail captif       |Authentification renforcée |100% des accès via portail |Actifs réseau dispo    |Infra compatible   |1 mois     |
    |B2     |Sécuriser l’accès aux applis métier                |Déploiment MFA                     |Authentification forte     |95 % des connexions via MFA|Équipe sécurité dispo  |Budget validé      |3 semaine  |
    |B3     |Sécuriser l’accès aux données internes             |Gestion des accès (AGDLP)          |Contrôle d’accès structuré |100 % des groupes conformes|Équipe sécurité dispo  |Admins formés      |2 mois     |
    |...    |...                                                |...                                |...                        |...                        |...                    |...                |...        |
    |B(n)   |(besoin tech)                                      |(besoin tech)                      |(objectif)                 |(n)%                       |(Actifs actuel)        |(contrainte actuel)|(n) (temps)|

---

## I.5 Périmètre du projet
- Explication : definit les limites/zones de resource de l'infra SI sur laquelle le projet impactera
- Etape :

    - Le périmètre/zone d'intervention est définit sur différent plan, il faut expliquer sur quel plan le projet impactera

    | Plan du périmètre                         | Ce qui peut concrétement être               |
    |:------------------------------------------|:--------------------------------------------|
    | Sur le plan fonctionnel                   | Besoins métiers, processus, cas d’usage     |
    | Sur le plan applicatif                    | Applications, interconnexions, versions     |
    | Sur le plan OS                            | Systèmes d’exploitation, patching, support  |
    | Sur le plan matériel                      | Serveurs, stockage, postes, virtualisation  |
    | Sur le plan réseau                        | LAN, WAN, sécurité, segmentation            |
    | Sur le plan de gouvernance / stratégie    | Rôles, responsabilités, politiques, normes  |
    | Sécurité                                  | IAM, SOC, PRA/PCA, conformité               |
    | Données                                   | Qualité, stockage, flux, classification     |

---

## I.6 Livrables attendus
- Explication : ce que l’équipe doit produire pour prouver que l’objectif est atteint

| Type de Livrables     |
|:----------------------|
| Documents             |
| Artefacts techniques  |
| Environnements        |
| Résultats             |

| Ex de Documents       |
|:----------------------|
| cadrage               |
| spécifications        |

| Ex d'Artefacts techniques |
|:--------------------------|
| maquettes                 |
| scripts                   |

| Ex d'Environnements   |
|:----------------------|
| dev                   |
| test                  |
| prod                  |

| Ex de Résultats           |
|:--------------------------|
| tests validés             |
| migration effectuée       |