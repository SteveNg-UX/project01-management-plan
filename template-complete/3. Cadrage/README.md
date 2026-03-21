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

  | Ce qui doit être inclu dans les analyses  |
  |:------------------------------------------|
  | Dépendances entre actifs                  |
  | Processus métiers associés                |
  | Niveaux de criticité                      |
  | Contraintes actuelles                     |

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