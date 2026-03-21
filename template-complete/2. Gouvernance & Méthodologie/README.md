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

    | Matrice RACI  |
    |--------------:|
    |Tâche          |
    |Equipe         |
    |Rôle           |

    | Rôle        |
    |------------:|
    |Responsable  |
    |Approuveur   |
    |Conseiller   |
    |Informé      |

---

## II.2 Gouvernance
- Explication : 
- Notion :
    - **COPROJ**
    - **COPIL**
    - **CODIR**

---

## II.3 Méthodologie
- Explication : 
- Notion :
    - Catégorie Cycle Sequentielle

      | Cycle   |
      |--------:|
      |V        |
      |Waerfall |

    - Catégorie Cycle Iteratif

      | Cycle   |
      |--------:|
      |Agile    |
      |Lean     |

      | Méthode |
      |--------:|
      |Kanban   |
      |Scrum    |

      | Culture |
      |--------:|
      |DevOps   |
      |Scrum    |

---

## II.4 Planning
- Explication : 
- Notion :

    | Diagramme de gantt    |
    |----------------------:|
    |tâches                 |
    |durée                  |
    |date d'échéance        |
    |estimation jours homme |

---

## II.5 Budget / Coûts
- Explication : 
- Notion :

---

## II.6 Analyse des risques
- Explication : 
- Notion :

    - Matrice de Risque

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


    - Indication

    | Impact        | score |
    |--------------:|-------|
    |Négligeable    |1      |
    |Mineur         |2      |
    |Modéré         |3      |
    |Majeur         |4      |
    |Catastrophique |5      |

    | probable event  | score |
    |----------------:|-------|
    |Peu probable     |1      |
    |Probable         |2      |
    |Possible         |3      |
    |Très probable    |4      |

    | Type de mesure mitigation |
    |--------------------------:|
    | Préventives               |
    | Correctives               |