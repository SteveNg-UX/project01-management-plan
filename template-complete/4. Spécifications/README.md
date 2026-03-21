# IV. Spécifications

-  [IV.1 Exigences fonctionnelles](#iv1-exigences-fonctionnelles)
-  [IV.2 Exigences techniques](#iv2-exigences-techniques)
-  [IV.3 Contraintes](#iv3-contraintes)
-  [IV.4 Étude de marché / Benchmark solutions](#iv4-étude-de-marché--benchmark-solutions)

---

### IV.1 Exigences fonctionnelles
- Explication : Décrivent ce que le système doit faire
- Notion :
    - fonctionnalités attendues
    - comportements du système
    - interactions utilisateur
    - règles métiers
    - cas d’usage

    - Mise en pratique sur la descrition des exigences:

    |ID         |Description    |Critère d’acceptation  |
    |:----------|---------------|-----------------------|
    |EXGF1      |...            |Test sur ... OK        |
    |EXGF2      |...            |Check sur ... OK       |
    |...        |...            |...                    |
    |EXGF(n)    |que doit faire |Test sur (fonction) OK |

    - Mise en pratique sur la priorisation des exigences (méthode MSCW):

    |Must (critique)    |Should (important) |Could (confort)    |Won't (négligeable)    |
    |:------------------|-------------------|-------------------|-----------------------|
    |EXGT2              |EXGT1              |                   |                       |
    |                   |                   |                   |                       |

---

### IV.2 Exigences techniques
- Explication : Décrivent ce que le système doit être
- Notion :
    - performances
    - sécurité
    - compatibilité
    - architecture
    - normes techniques
    - intégrations

    - Mise en pratique sur la descrition des exigences:

    |ID         |Description    |Critère d’acceptation  |
    |:----------|---------------|-----------------------|
    |EXGT1      |...            |Test sur ... OK        |
    |EXGT2      |...            |Check sur ... OK       |
    |...        |...            |...                    |
    |EXGT(n)    |que doit faire |Test sur (fonction) OK |

    - Mise en pratique sur la priorisation des exigences (méthode MSCW):

    |Must (critique)    |Should (important) |Could (confort)    |Won't (négligeable)    |
    |:------------------|-------------------|-------------------|-----------------------|
    |EXGT2              |                   |EXGT1              |                       |
    |                   |                   |                   |                       |

---

### IV.3 Contraintes
- Explication : Décrivent ce que le système doit respecter
- Notion :
    - contraintes réglementaires
    - contraintes organisationnelles
    - contraintes budgétaires
    - contraintes de planning
    - contraintes d’infrastructure

---

### IV.4 Étude de marché / Benchmark solutions
- Explication :
- Notion :
    - Se baser sur des référence d'analyse fiable : Magic Quadrant Gartner, Wave Report Forrester...etc
    - Les retours d'expérience : Reddit, StackOverflow, Github Issue...etc

    - Mise en pratique sur la descrition des benchmarks :
    
    |Technologie    |Fonction   |Leadership |Coût (TCO) |Performance    |Sécurité   |Simplicité |Intégraation avec le SI    |Support    |Innovation |
    |---------------|-----------|-----------|-----------|---------------|-----------|-----------|---------------------------|-----------|-----------|
    |tech 1         |stockage   |fort       |...€       |fort           |fort       |complexe   |bonne                      |bonne      |fort       |
    |tech 2         |hypervisor |fort       |open-source|fort           |fort       |facile     |bonne                      |aucun      |modéré     |
    |...            |...        |...        |...        |...            |...        |...        |...                        |...        |...        |
    |(techno)       |fonction   |?          |(n) €      |?              |?          |?          |?                          |?          |?          |