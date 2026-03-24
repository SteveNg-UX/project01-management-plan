# VIII. Tests

- [VIII.1 Stratégie de test](#viii1-stratégie-de-test)
- [VIII.2 Tests](#viii2-tests)
- [VIII.3 Validation du bon fonctionnement](#viii3-validation-du-bon-fonctionnement)
- [VIII.4 Documentation](#viii4-documentation)

---

### VIII.1 Stratégie de test
- Explication :
- Etape :

---

### VIII.2 Tests
- Explication :
- Etape :

    Les tests à faire sont classé selon leur type:

    |Type de test       |
    |:------------------|
    |Test unitaire      |
    |Test d'Intégration |
    |Test de Fonctionnel|
    |Test de Sécurité   |

    | ID    | Description du test                               | But du test                                           | Responsable du test   | Type de test                  |
    |-------|---------------------------------------------------|-------------------------------------------------------|-----------------------|-------------------------------|
    | TST1  | Vérifier la création d’un compte utilisateur      | S’assurer que la fonctionnalité répond au besoin MOA  | Alice A               | Test fonctionnel              |
    | TST2  | Tester la connexion avec mot de passe incorrect   | Vérifier la gestion des erreurs et messages affichés  | Bob B                 | Test fonctionnel              |
    | TST3  | Vérifier la réponse de l’API /users en JSON       | S’assurer que l’API renvoie un format conforme        | Celine C              | Test d’intégration            |
    | TST4  | Test de charge sur le module d’authentification   | Vérifier la tenue en charge sous 500 req/min          | David D               | Test technique (performance)  |
    | TST5  | Scan OWASP Top 10 sur l’application               | Identifier les vulnérabilités critiques               | Eric E                | Test sécurité (Pentest)       |
    | TST6  | Vérifier la mise à jour d’un utilisateur en base  | S’assurer que les données sont correctement persistées| Fred F                | Test d’intégration            |
    | TST7  | Test unitaire de la fonction hashPassword()       | Garantir que le hash respecte les normes de sécurité  | Goku G                | Test unitaire                 |
    | TST8  | Vérifier le déploiement automatique via CI/CD     | S’assurer que le pipeline fonctionne sans erreur      | Henry H               | Test technique (CI/CD)        |
    | TST9  | Vérifier l’accessibilité (WCAG niveau AA)         | S’assurer que l’interface est accessible              | Isidor I              | Test fonctionnel (UX)         |
    | TST10 | Test de rollback en cas d’échec de déploiement    | Vérifier la résilience du système                     | Julien J              | Test technique (Ops)          |
    |...    |...                                                |...                                                    |...                    |...                            |
    |TST(n) |(Description)                                      |(But)                                                  |(Prenom) (Nom)         |(Type)                         |

---

### VIII.3 Validation du bon fonctionnement
- Explication :
- Etape :

---

### VIII.4 Documentation
- Explication :
- Etape :