# Task 3 — Secure Coding Review

**CodeAlpha — Cyber Security Internship**
**Auteur :** Sarah Boucherou

## Objectif

Auditer un module d'authentification (login) écrit en Python afin d'identifier
des vulnérabilités de sécurité courantes, évaluer leur sévérité, et proposer des
recommandations de correction conformes aux bonnes pratiques de secure coding
(OWASP Top 10).

## Méthodologie

- Lecture manuelle ligne par ligne du code source.
- Recherche des vulnérabilités classiques : injection, gestion des mots de passe,
  validation des entrées, gestion des erreurs, secrets en dur.
- Référence aux catégories de l'OWASP Top 10 (2021).
- Proposition d'un correctif pour chaque vulnérabilité identifiée.

## Vulnérabilités identifiées

| Vulnérabilité | Sévérité | Recommandation |
|---|---|---|
| SQL Injection | Critique | Requêtes paramétrées (prepared statements) |
| Mot de passe stocké en clair | Élevée | Hachage avec bcrypt / argon2 |
| Clé secrète codée en dur | Élevée | Variables d'environnement |
| Absence de gestion des erreurs | Moyenne | try/except + logs + message générique |

## Contenu du dépôt

- `Secure_Coding_Review.docx` — le rapport complet avec le code vulnérable
  analysé, l'explication détaillée de chaque faille, et le code corrigé.

## Ce que j'ai appris

- Reconnaître les vulnérabilités de sécurité les plus courantes dans du code Python.
- Utiliser les catégories OWASP Top 10 pour classifier les risques.
- Rédiger un rapport d'audit de sécurité structuré (sévérité, risque, correctif).
- Écrire du code sécurisé : requêtes paramétrées, hachage de mots de passe,
  gestion propre des secrets et des erreurs.
