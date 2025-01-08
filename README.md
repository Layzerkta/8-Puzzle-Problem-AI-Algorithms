# Rapport d'Exercices sur l'IA - DIA5

Ce dépôt contient une analyse approfondie des problématiques posées dans le cadre des exercices donnés, ainsi que des solutions détaillées et argumentées. Les sujets abordés incluent des objections modernes à l'intelligence artificielle, des prédictions sur les capacités des IA modernes, ainsi que la formulation et la résolution d'un problème de recherche d'état.

## Table des matières

- [Exercice 1 : Objections et Perspectives](#exercice-1--objections-et-perspectives)
  - [Objections toujours pertinentes](#objections-toujours-pertinentes)
  - [Nouvelles objections liées aux développements récents](#nouvelles-objections-liées-aux-développements-récents)
  - [Prédictions et validations du test de Turing](#prédictions-et-validations-du-test-de-turing)
- [Exercice 2 : Problème de recherche et algorithmes](#exercice-2--problème-de-recherche-et-algorithmes)
  - [Formulation du problème](#formulation-du-problème)
  - [Taille et représentation de l'espace d'états](#taille-et-représentation-de-lespace-détats)
  - [Algorithmes de recherche](#algorithmes-de-recherche)
  - [Heuristique admissible](#heuristique-admissible)
- [Conclusion](#conclusion)

---

## Exercice 1 : Objections et Perspectives

### Objections toujours pertinentes

1. **Argument de la conscience** :  
   Une IA, même avancée, ne possède pas de conscience propre. Bien qu'elle puisse imiter un comportement humain, elle reste dénuée d'une véritable subjectivité.  
   **Critique de Turing** : L'IA n'a pas besoin d'une conscience pour imiter des comportements humains de manière efficace.

2. **Limites mathématiques** :  
   Une IA ne peut pas résoudre tous les problèmes complexes, tout comme les humains. Cette objection est toujours valide et reste un défi majeur pour les IA modernes.

### Nouvelles objections liées aux développements récents

- **Créativité et art** : Les créations des IA (images, musiques, textes) sont-elles réellement originales ou simplement des assemblages de données d'entraînement ?
- **Capacités généralistes** : Contrairement aux humains, une IA excelle dans des domaines spécifiques mais ne peut pas généraliser ses compétences à d'autres domaines.

### Prédictions et validations du test de Turing

Avec des modèles modernes comme ChatGPT, une IA pourrait avoir **50 % de chances** de réussir un test de Turing simple, surtout face à un interlocuteur peu habitué à interagir avec des IA.

---

## Exercice 2 : Problème de recherche et algorithmes

### Formulation du problème

- **États** : Configurations possibles du carré magique 3x3.
- **Actions** : Déplacements du chiffre 9 (haut, bas, gauche, droite).
- **État initial** : Configuration donnée.
- **Condition d'objectif** : La somme de chaque ligne, colonne et diagonale doit être égale à 15.

### Taille et représentation de l'espace d'états

- **Représentation** : Graphe (présence de cycles et états revisités).
- **Taille** : \( 9! \) (toutes les permutations des 9 cases).

### Algorithmes de recherche

#### Recherche en largeur (BFS)
- **Avantages** : Garantit la solution optimale.
- **Inconvénients** : Exige beaucoup de mémoire, temps d'exécution élevé.

#### Recherche en profondeur (DFS)
- **Avantages** : Faible consommation de mémoire.
- **Inconvénients** : Ne garantit pas une solution optimale et peut se perdre dans des branches inutiles.

#### Recherche avec approfondissement itératif (IDS)
- **Avantages** : Combine les forces du BFS et DFS, moins gourmande en mémoire.
- **Inconvénients** : Répète certaines explorations, ce qui réduit son efficacité.

### Heuristique admissible

Une **heuristique de Manhattan** peut être utilisée : somme des distances de chaque chiffre à sa position cible. Elle est admissible car elle ne surestime jamais le coût réel pour atteindre l'objectif.

---

## Conclusion

Ce travail illustre les forces et les limites des IA modernes ainsi que l'importance des algorithmes de recherche dans la résolution de problèmes complexes. Les objections soulevées sur la conscience, la créativité et les capacités généralistes des IA montrent qu'il reste encore un long chemin à parcourir avant d'atteindre une intelligence comparable à celle des humains.

---

## Auteur

**Maxim Quénel**  
Étudiant en Intelligence Artificielle, passionné par les défis liés à la compréhension et à l'amélioration des technologies intelligentes.
