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
- Notion :

    | Matrice RACI          |
    |:----------------------|
    |Tâche                  |
    |Nom de la personne     |
    |Poste                  |
    |Rôle dans le projet    |
    |Equipe                 |
    |MOA /MOE               |

    | Rôle dans le projet   | Lettre  |
    |:----------------------|:--------|
    |Responsable            | (R)     |
    |Approuveur             | (A)     |
    |Conseiller             | (C)     |
    |Informé                | (I)     |

    |MOA (Partie Prenant)       |MOE (Equipe Projet)    |
    |:--------------------------|:----------------------|
    |RSSI                       |Architectes            |
    |DSI                        |Ops                    |
    |Fournisseurs               |Dev                    |
    |                           |DevOps                 |
    |                           |Expert                 |

    - Mise en pratique :

    |ID     |Tâche  |Nom de la personne     |Poste      |Rôle dans le projet    |Equipe |MOA /MOE   |
    |:------|:------|:----------------------|:----------|:----------------------|:------|:----------|
    |T1     |...    |John Doe               |Admin      |R                      |Ops    |MOE        |
    |T2     |...    |Jane Doe               |Dev Front  |R                      |Dev    |MOE        |
    |...    |...    |...                    |...        |...                    |...    |...        |
    |T(n)   |(tâche)|(prenom) (nom)         |(poste)    |(Role)                 |(Eqp.) |(MOA/MOE)  |

---

## II.2 Gouvernance
- Explication : 
- Notion :
    
    |Comité |Ce qui peut concrétement être              |
    |:------|:------------------------------------------|
    |COPROJ |suivi opérationnel                         |
    |COPIL  |arbitrage, décisions stratégiques          |
    |CODIR  |alignement global SI / stratégie entreprise|

---

## II.3 Méthodologie
- Explication : 
- Notion :
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
- Notion :

    | Diagramme de gantt    |
    |:----------------------|
    |tâches                 |
    |durée                  |
    |date d'échéance        |
    |estimation jours homme |

---

## II.5 Budget / Coûts
- Explication : 
- Notion :

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
- Notion :

    - Indication pour utiliser une Matrice de Risque

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

    - Mise en pratique :

    | ID    | Scénario  | Cause | Conséquence   | Impact / Criticité    | Probabilité   | Priorité (score = Impact+ P robabilité)   | Mesure mitigation |
    |:------|:----------|:------|:--------------|:----------------------|:--------------|:------------------------------------------|:------------------|
    | R1    | ...       | ...   | ...           | 2                     | 3             | 5                                         | ...               |
    | R2    | ...       | ...   | ...           | 5                     | 2             | 7                                         | ...               |
    | ...   | ...       | ...   | ...           | ...                   | ...           | ...                                       | ...               |
    | R(n)  | ...       | ...   | ...           | (1-5)                 | (1-4)         | (2-9)                                     | ...               |

    |Impact / probablilité  |Peu probable (1)   |Probable (2)   |Possible (3)   |Très probable (4)  |
    |:----------------------|:------------------|:--------------|:--------------|:------------------|
    |Négligeable (1)        |                   |               |               |                   |
    |Mineur (2)             |                   |               | R1            |                   |
    |Modéré (3)             |                   |               |               |                   |
    |Majeur (4)             |                   |               |               |                   |
    |Catastrophique (5)     |                   | R2            |               |                   |