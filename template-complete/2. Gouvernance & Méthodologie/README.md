# II. Gouvernance & Méthodologie
- [II.1 Équipe projet](#ii1-équipe-projet)
- [II.2 Gouvernance](#ii2-gouvernance)
- [II.3 Méthodologie](#ii3-méthodologie)
- [II.4 Planning de tâches](#ii4-planning)
- [II.5 Budget / Coûts](#ii5-budget--coûts)
- [II.6 Analyse des risques](#ii6-analyse-des-risques)

---

## II.1 Équipe projet
- Explication : 
- Etape :
    Definir une matrice RACI avec 2 éléments :
    - Les étapes du projet
    - Les roles des équipes

    | Rôle dans le projet   | Lettre  |
    |:----------------------|:--------|
    |Responsable            | (R)     |
    |Approuveur             | (A)     |
    |Conseiller             | (C)     |
    |Informé                | (I)     |

    | Equipe            | Profile                                       |
    |:------------------|:----------------------------------------------|
    |Exploitation (Ops) |Admin Systèmes, Admin Réseau, SRE, IT Support  |
    |Sécurité (Cyber)   |RSSI, SecOps, Pentest                          |
    |Développement (Dev)|Dev Fullstack, Tech lead, QA                   |
    |Architecte (Arch)  |Architecte SI, Architecte Solution             |
    |Projet (PMO)       |Chef de projet, Product Owner, Scrum Master    |
    |Platform Ingineer  |Ingénieur DevOps                               |

    | MOA (Partie Prenant)      |MOE (Equipe Projet)    |
    |:--------------------------|:----------------------|
    |DSI                        |Ops                    |
    |RSSI                       |Cyber                  |
    |Fournisseurs               |Dev                    |
    |Utilisateurs               |Arch                   |
    |Chef de projet MOA         |PMO                    |
    |                           |Platform Ingineer      |

    - Lister les différentes étapes du projet avec le rôle des équipes :

    | Livrable / Activité               | DSI (MOA) | RSSI (MOA)    | Fournisseurs (MOA)    | Chef de projet MOA    | Dev   | Ops   | Cyber | Arch  | PMO   | Platform Eng. |
    |-----------------------------------|-----------|---------------|-----------------------|-----------------------|-------|-------|-------|-------|-------|---------------|
    | Recueil des besoins / objectifs   | A         | I             | C                     | R                     | C     | I     | I     | C     | C     | I             |
    | Spécifications fonctionnelles     | A         | I             | C                     | R                     | R     | I     | I     | C     | C     | I             |
    | Spécifications techniques         | I         | I             | C                     | C                     | R     | C     | C     | A     | C     | C             |
    | Architecture cible                | I         | C             | C                     | C                     | C     | C     | C     | A/R   | I     | C             |
    | Conception                        | I         | I             | C                     | I                     | R     | I     | C     | C     | C     | C             |
    | Deploiement                       | I         | I             | I                     | I                     | C     | C     | C     | C     | I     | R/A           |
    | Tests fonctionnels                | I         | I             | C                     | R                     | R     | I     | I     | I     | C     | I             |
    | Tests techniques / sécurité       | I         | A             | C                     | I                     | C     | C     | R     | C     | C     | C             |
    | Déploiement en production         | I         | I             | I                     | I                     | C     | R/A   | C     | C     | C     | C             |
    | Gestion du changement             | A         | C             | I                     | R                     | C     | C     | C     | C     | C     | I             |
    | Documentation finale              | A         | I             | C                     | R                     | R     | C     | C     | C     | C     | I             |
    | Clôture du projet                 | A         | I             | I                     | R                     | C     | C     | C     | C     | R     | I             |

---

## II.2 Gouvernance
- Explication : 
- Etape :
    
    |Comité |Ce qui peut concrétement être              |
    |:------|:------------------------------------------|
    |COPROJ |suivi opérationnel                         |
    |COPIL  |arbitrage, décisions stratégiques          |
    |CODIR  |alignement global SI / stratégie entreprise|

---

## II.3 Méthodologie
- Explication : 
- Etape :
    - Catégorie Cycle Sequentielle

      | Cycle   |
      |:--------|
      |V        |
      |Waterfall|

    - Catégorie Cycle Iteratif

      | Cycle   |
      |:--------|
      |Agile    |
      |Lean     |

      | Méthode |
      |:--------|
      |Kanban   |
      |Scrum    |

      | Culture |
      |:--------|
      |DevOps   |

---

## II.4 Planning
- Explication : 
- Etape :

    | Diagramme de gantt    |
    |:----------------------|
    |tâches                 |
    |durée                  |
    |date d'échéance        |
    |estimation jours homme |

---

## II.5 Budget / Coûts
- Explication : 
- Etape :

    Les coûts de chaque actif sur l'ensemble du SI seront catégorisé selon 5 critaires:
    - Le coût de l'actif
    - Le nombre d'actif
    - Le Type de Coût
    - La catégorie de dépense
    - Plan du périmètre (présenté précédemment à la l'étape [Présentation général partie I.5](https://gitlab.com/noxumbris/project-01-management-plan/-/tree/main/template-complete/1.%20Pr%C3%A9sentation%20g%C3%A9n%C3%A9rale?ref_type=heads#i5-p%C3%A9rim%C3%A8tre-du-projet))

    |Catérogie de dépense   |Desciption                                                                                         |Exemple                                                            |
    |:----------------------|:--------------------------------------------------------------------------------------------------|:------------------------------------------------------------------|
    |CAPEX                  |Dépenses Capitales donc des dépenses initials important pour un investissement sur de long terme   |Achat de materiel, Achat des locaux                                |
    |OPEX                   |Dépense d'Exploitation donc des dépenses quotidiennes pour la maintenance du SI                    |Abonnement logiciels Saas, Factures d'energie, Salaires mensuels   |

    |Type de Coût       |Ce qui peut concrétement être  |
    |:------------------|:------------------------------|
    |Coûts humains      |jours-homme                    |
    |Coûts matériels    |serveurs, licences             |
    |Coûts logiciels    |SaaS, abonnements              |
    |Coûts de services  |intégrateurs, consultants      |

    - Listing et classement des actifs

    |ID     |Actif                      |Coût           |quantité   |Type de Coût   |Catérogie de dépense   |Plan du périmètre  |
    |:------|:--------------------------|:--------------|:----------|:--------------|:----------------------|:------------------|
    |CT1    |QNAP TS-464                |634€ HT        |x2         |matériels      |CAPEX                  |matériel           |
    |CT2    |Licence Win2025 Standard   |672,05€ HT     |x5         |matériels      |CAPEX                  |OS                 |
    |CT3    |Licence E3 Microsoft 365   |34,90€ HT /mois|x20        |logiciels      |OPEX                   |applicatif         |
    |...    |...                        |...            |...        |...            |...                    |...                |
    |CT(n)  |(composant du SI)          |(n)€           |x(n)       |(type)         |(CAPEX/OPEX)           |(périmètre)        |

    - Calcule de coût total de possession et de retour sur investissement

    |Evaluation globale |Ce qui peut concrétement être                                  |
    |:------------------|:--------------------------------------------------------------|
    |TCO                |mesure coût total de possession (ce que vous dépensez)         |
    |ROI                |mesure le rendement de cet investissement (ce que vous gagnez) |

---

## II.6 Analyse des risques
- Explication : 
- Etape :

    Les risques, menace et défaut sont définit sur 2 critères
    - L'impact sur l'infra du SI
    - La probabilité qu'il puisse arrivé

    | Impact        | score |
    |:--------------|:------|
    |Négligeable    |1      |
    |Mineur         |2      |
    |Modéré         |3      |
    |Majeur         |4      |
    |Catastrophique |5      |

    | probable event  | score |
    |:----------------|:------|
    |Peu probable     |1      |
    |Probable         |2      |
    |Possible         |3      |
    |Très probable    |4      |

    | Type de mesure mitigation |
    |:--------------------------|
    | Préventives               |
    | Correctives               |

    - Identifier, lister et qualifier les risques dans un tableau des risques

    | ID    | Scénario                  | Cause                                     | Conséquence                                           | Impact / Criticité    | Probabilité   | Priorité (score = Impact+ P robabilité)   | Mesure mitigation                         |
    |:------|:--------------------------|:------------------------------------------|:------------------------------------------------------|:----------------------|:--------------|:------------------------------------------|:------------------------------------------|
    |RSK1   |température ambiant élevé  |absence de dispositif de refroidissement   | appareils en surchauffe                               |4                      |3              |7                                          |Ajouter un dispositif de refroidissement   |
    |RSK2   |OS obsolète                |fin de support de la version de l'OS       | future vulnérabilités non patché                      |4                      |4              |9                                          |Faire un upgrade de l'OS                   |
    |RSK3   |indisponibilité serveur app|un seul serveur app                        | users bloqués pour l'utilisation de l'app du serveur  |3                      |2              |5                                          |Ajouter de la redondance                   |
    | ...   | ...                       | ...                                       | ...                                                   | ...                   | ...           | ...                                       | ...                                       |
    |RSK(n) | (situation)               | (cause)                                   | (conséquence)                                         |(1-5)                  |(1-4)          |(2-9)                                      |(solution)                                 |

    - Classer ensuite les risques en fonction des ordre de priorité dans une matrice de risque

    |Impact / probablilité  |Peu probable (1)   |Probable (2)   |Possible (3)   |Très probable (4)  |
    |:----------------------|:------------------|:--------------|:--------------|:------------------|
    |Négligeable (1)        |                   |               |               |                   |
    |Mineur (2)             |                   |               |               |                   |
    |Modéré (3)             |                   | RSK3          |               |                   |
    |Majeur (4)             |                   |               | R1            | R2                |
    |Catastrophique (5)     |                   |               |               |                   |