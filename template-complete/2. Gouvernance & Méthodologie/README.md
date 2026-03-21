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

    |Catégories Coût    |Ce qui peut concrétement être  |
    |:------------------|:------------------------------|
    |Coûts humains      |jours-homme                    |
    |Coûts matériels    |serveurs, licences             |
    |Coûts logiciels    |SaaS, abonnements              |
    |Coûts de services  |intégrateurs, consultants      |

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