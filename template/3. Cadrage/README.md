# III. Cadrage

- [III.1 Analyse de l’existant](#iii1-analyse-de-lexistant)
- [III.2 Critique de l’existant](#iii2-critique-de-lexistant)
- [III.3 Définition des trajectoires](#iii3-définition-des-trajectoires)
- [III.4 Choix de la trajectoire cible](#iii4-choix-de-la-trajectoire-cible)

---

## III.1 Analyse de l’existant
- Explication : Definit toutes les actifs de chaque plan du SI dans le périmètre et leur état actuel
- Etape :
    - Si le projet couvre une majeur partie du SI, alors il faut définir le périmètre/zone qui ne doit pas être impacté
    - Si le projet couvre une mineur partie du SI, alors il faut définir le périmètre/zone qui seront impacté
    
    | Ce qui doit être inclu dans les analyses  |
    |:------------------------------------------|
    | Dépendances entre actifs                  |
    | Processus métiers associés                |
    | Niveaux de criticité                      |
    | Contraintes actuelles                     |

    - Lister et classer dans un tableau les actifs selon le plan vue précédemment à l'étape [Présentation général dans la partie I.5 Périmètre du projet](https://gitlab.com/noxumbris/project-01-management-plan/-/tree/main/template-complete/1.%20Pr%C3%A9sentation%20g%C3%A9n%C3%A9rale?ref_type=heads#i5-p%C3%A9rim%C3%A8tre-du-projet)

    |ID     |Actif SI                       |quantité   |Fonction                                       |Plan de la rsesource   |
    |:------|:------------------------------|:----------|:----------------------------------------------|-----------------------|
    |RSC1   |Serveur QNAP TS-464            |x1         |Stockage/Sauvegarde de fichier                 |matériel               |
    |RSC2   |Licence VMWare ESXi 6.0        |x4         |Mutualise les ressources via la virtualisation |OS                     |
    |RSC3   |Licence Suite E3 Microsoft 365 |x20        |Application metier pour les Users              |applicatif             |
    |...    |...                            |...        |...                                            |...                    |
    |RSC(n) |(actif)                        |x(n)       |(fonction)                                     |(plan)                 |

---

## III.2 Critique de l’existant
- Explication : Definit les risques /menace /problèmes que posent ou peut poser chaque actif
- Etape :
  
  Associer les actifs du tableau lister à l'étape [précédemment](#iii1-analyse-de-lexistant) aux risques du tableau vue à l'étape [Présentation général dans la partie I.5 Périmètre du projet](https://gitlab.com/noxumbris/project-01-management-plan/-/tree/main/template-complete/1.%20Pr%C3%A9sentation%20g%C3%A9n%C3%A9rale?ref_type=heads#i5-p%C3%A9rim%C3%A8tre-du-projet)
  Catégorisé les risque selon les axes

  | Axes de Risque              | Ce qui peut concrétement être             |
  |:----------------------------|:------------------------------------------|
  | Risques opérationnels       | pannes, obsolescence, SPOF, compatibilité |
  | Risques de sécurité         | vulnérabilités, mauvaise segmentation     |
  | Risques organisationnels    | manque de compétences, gouvernance floue  |
  | Risques financiers          | coûts cachés, maintenance excessive       |
  | Risques réglementaires      | RGPD, conformité                          |

  | ID Actif  | ID Risque | Axe de Risque           |
  |:----------|:----------|:------------------------|
  |RSC1       |RSK3       |opérationnels            |
  |RSC2       |RSK2       |opérationnels, sécurité  |
  |...        |...        |...                      |
  |RSC(n)     |RSK(n)     |(Axes)                   |

---

## III.3 Définition des trajectoires
- Explication : Définit les mesures de mitigation, les solutions et bonnes pratiques possible pour chaque critique de l'existant
- Etape :

  - Les trajectoires sont définient selon différents niveaux

  | Niveaux de trajectoire  | Ce qui peut concrétement être               |
  |:------------------------|:--------------------------------------------|
  | Minimal                 | quick wins, corrections urgentes            |
  | Intermediaire           | améliorations structurantes                 |
  | Ambitieuse              | refonte, modernisation, cloud, Zero Trust…  |

  - Par rapport aux associations des actifs/risques vue [précédemment]((#iii2-critique-de-lexistant)), proposer différente trajectoire plus précis que ceux des Mesure mitigation du tableau des risques vue à l'étape [Présentation général dans la partie I.5 Périmètre du projet](https://gitlab.com/noxumbris/project-01-management-plan/-/tree/main/template-complete/1.%20Pr%C3%A9sentation%20g%C3%A9n%C3%A9rale?ref_type=heads#i5-p%C3%A9rim%C3%A8tre-du-projet)

  |ID   | ID Actif  | ID Risque | Trajectoire                                               | coûts     | délais    | impacts                 | risques résiduels               | dépendances                           |
  |:----|:----------|:----------|:----------------------------------------------------------|:----------|:----------|:------------------------|:--------------------------------|:--------------------------------------|
  |TJ1  |RSC2       |RSK2       |Ajout de second serveur et clusterisation                  |modéré     |1 semaine  |Disponibilité            |complexité, configuration        |financière                             |
  |TJ2  |RSC1       |RSK3       |Upgrade de version de l'OS vers en plus récent (ESXi 9.0)  |fort       |2 semaine  |sécurité, compatibilité  |dépendance matériel              |compatibilité                          |
  |TJ3  |RSC1       |RSK3       |Remplacement pour modèle de serveur récent                 |fort       |1 mois     |Fiabilité + performance  |financier, migration             |financière, delais livraison, migration|
  |TJ4  |RSC1       |RSK3       |Migration Solution VMWare ESXi vers un autre Hyperviseur   |modéré     |2 semaine  |dépendance tiers         |migration, organisationnels      |formation, compatibilité               |
  |...  |...        |...        |...                                                        |...        |... (temps)|...                      |...                              |...                                    |
  |TJ(n)|RSC(n)     |RSK(n)     |(possibilité)                                              |(coûts)    |(n) (temps)|impacts                  |(risques résiduels)              |(dépendances)                          |

---

## III.4 Choix de la trajectoire cible
- Explication : Etudie les contrainte des trajectoire pour definir le choix de la tragéctoire la plus cohérente de chaque critique de l'existant
- Etape :

  - choisir une trajectoire parmi plusieurs options en utilisant le SWOT (FFOM en version francais)
  - Mise en pratique :

  |ID Trajectoire |Force                      |Faiblesse              |Opportunité                          |Menace                                 |
  |:--------------|:--------------------------|:----------------------|:------------------------------------|:--------------------------------------|
  |TJ1            |Tolérance aux pannes       |Complexité maîtrise    |Amélioration SLA                     |Configuration                          |
  |TJ2            |Sécurité, Compatibilité    |Dépendance au matériel |Alignement sur versions supportées   |Interruption                           |
  |TJ3            |Fiabilité, performance     |Coût élevé, delai      |Modernisation                        |Hausse de prix, retard                 |
  |TJ4            |Coût, independance éditeur |maitrise et formation  |Standardisation, simplicification SI |Compatibilité, résistance au changement|
  |...            |...                        |...                    |...                                  |...                                    |
  |TJ(n)          |...                        |...                    |...                                  |...                                    |