# III. Cadrage

- [III.1 Analyse de l’existant](#iii1-analyse-de-lexistant)
- [III.2 Critique de l’existant](#iii2-critique-de-lexistant)
- [III.3 Définition des trajectoires](#iii3-définition-des-trajectoires)
- [III.4 Choix de la trajectoire cible](#iii4-choix-de-la-trajectoire-cible)

---

## III.1 Analyse de l’existant
- Explication : Definit toutes les actifs de chaque plan du SI dans le périmètre et leur état actuel
- Notion :
  - [Périmètre](#remarque-)

    - Si le projet couvre une majeur partie du SI, alors il faut définir le périmètre/zone qui ne doit pas être impacté
    - Si le projet couvre une mineur partie du SI, alors il faut définir le périmètre/zone qui seront impacté
      
    | Ce qui doit être inclu dans les analyses  |
    |:------------------------------------------|
    | Dépendances entre actifs                  |
    | Processus métiers associés                |
    | Niveaux de criticité                      |
    | Contraintes actuelles                     |

    - Lister et classer les Actifs selon le plan vue précédemment à l'étape [Présentation général dans la partie I.5 Périmètre du projet](https://gitlab.com/noxumbris/project-01-management-plan/-/tree/main/template-complete/1.%20Pr%C3%A9sentation%20g%C3%A9n%C3%A9rale?ref_type=heads#i5-p%C3%A9rim%C3%A8tre-du-projet)

    |ID     |Actif SI                       |quantité   |Fonction                                       |Plan de la rsesource   |
    |:------|:------------------------------|:----------|:----------------------------------------------|-----------------------|
    |RSC1   |Serveur QNAP TS-464            |x2         |Stockage/Sauvegarde de fichier                 |matériel               |
    |RSC2   |Licence VMWare ESXi 9.0        |x4         |Mutualise les ressources via la virtualisation |OS                     |
    |RSC3   |Licence Suite E3 Microsoft 365 |x20        |Application metier pour les Users              |applicatif             |
    |...    |...                            |...        |...                                            |...                    |
    |RSC(n) |(actif)                        |x(n)       |(fonction)                                     |(plan)                 |

---

## III.2 Critique de l’existant
- Explication : Definit les risques /menace /problèmes que posent ou peut poser chaque actif
- Notion :
  - [Périmètre](#remarque-)

  | Critique de risque sur axes | Ce qui peut concrétement être             |
  |:----------------------------|:------------------------------------------|
  | Risques opérationnels       | pannes, obsolescence, SPOF                |
  | Risques de sécurité         | vulnérabilités, mauvaise segmentation     |
  | Risques organisationnels    | manque de compétences, gouvernance floue  |
  | Risques financiers          | coûts cachés, maintenance excessive       |
  | Risques réglementaires      | RGPD, conformité                          |

---

## III.3 Définition des trajectoires
- Explication : Définit les mesures de mitigation, les solutions et bonnes pratiques possible pour chaque critique de l'existant
- Notion :
  - [Périmètre](#remarque-)

  | Niveaux de trajectoire  | Ce qui peut concrétement être               |
  |:------------------------|:--------------------------------------------|
  | Minimal                 | quick wins, corrections urgentes            |
  | Intermediaire           | améliorations structurantes                 |
  | Ambitieuse              | refonte, modernisation, cloud, Zero Trust…  |

  - Mise en pratique :

  | ID  | Trajectoire | coûts | délais  | impacts   | risques résiduels | dépendances |
  |:----|:------------|:------|:--------|:----------|:------------------|:------------|
  | T1  | ...         | ... € | ... j   | ...       | ...               | ...         |
  | T2  | ...         | ... € | ... j   | ...       | ...               | ...         |
  

---

## III.4 Choix de la trajectoire cible
- Explication : Etudie les contrainte des trajectoire pour definir le choix de la tragéctoire la plus cohérente de chaque critique de l'existant
- Notion :
  - [Périmètre](#remarque-)

  - choisir une trajectoire parmi plusieurs options en utilisant le SWOT (FFOM en version francais)
  
  - Mise en pratique :

  |ID Trajectoire |Force  |Faiblesse  |Opportunité  |Menace |
  |:--------------|:------|:----------|:------------|:------|
  |T1             |...    |...        |...          |...    |
  |T2             |...    |...        |...          |...    |
  |...            |...    |...        |...          |...    |
  |T(n)           |...    |...        |...          |...    |

---

### Remarque :

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