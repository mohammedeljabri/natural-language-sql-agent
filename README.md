# Natural Language SQL Agent

Interrogez n'importe quelle base de données en français, sans écrire une seule ligne de SQL.

---

## Ce que ça fait

Un manager pose une question en langage naturel. L'agent génère la requête SQL, l'exécute et restitue le résultat en quelques secondes — sans intervention technique.

```
"Quels clients ont un solde négatif ?"
        ↓
SELECT * FROM clients WHERE solde < 0 LIMIT 100;
        ↓
Tableau de résultats structuré
```

---

## Résultats observés

- Réponse en moins de 30 secondes sur machine standard
- 100% local — aucune donnée ne quitte l'infrastructure
- Fonctionne sans GPU dédié

---

## Deux modes d'utilisation

**Mode Business** — pour les décideurs
Résultat direct en tableau, sans jargon technique.

**Mode Pédagogique** — pour les équipes data et étudiants
SQL généré visible, conseils méthodologiques intégrés, comparaison de modèles.

---

## Stack technique

| Composant | Technologie |
|-----------|-------------|
| Modèle IA | Mistral / Qwen2.5-coder (local via Ollama) |
| Base de données | PostgreSQL |
| Interface | Streamlit |
| Orchestration | LangChain |
| Langage | Python 3.14 |

---

## Souveraineté des données

Conçu pour les environnements à contraintes réglementaires fortes :

- Modèle IA exécuté **100% en local**
- Zéro appel vers des APIs externes
- Compatible avec les exigences **RGPD** et **ACPR**
- Fonctionne sur un laptop standard sans GPU

---

## Cas d'usage

Ce système est directement applicable dans tout secteur manipulant des bases de données :
analyse de portefeuilles clients, suivi de conformité, reporting opérationnel, exploration de données métier.

---

## Auteur

**Mohammed El Jabri**
Data Scientist & Enseignant à l'Université de Technologie de Troyes (UTT)
Expert en agents IA appliqués aux environnements professionnels

👉 [LinkedIn](https://linkedin.com/in/mohammedeljabri)

---

*Ces approches sont directement transposables à des environnements professionnels réels.*
