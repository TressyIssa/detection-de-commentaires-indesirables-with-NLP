# Détection de Spam avec NLP et Machine Learning

## Introduction

Le spam, ou courrier indésirable, est un problème omniprésent dans les communications numériques modernes. Il affecte les e-mails, les messages SMS, et même les plateformes de réseaux sociaux. Ces messages perturbent les utilisateurs, encombrent les systèmes, et peuvent servir de vecteurs pour des attaques malveillantes. L'utilisation de techniques avancées en traitement du langage naturel (NLP) permet de détecter et de filtrer ces messages avec une précision croissante.

## Problématique

Avec l'évolution constante des stratégies des spammeurs, comment concevoir un modèle NLP capable de distinguer efficacement les messages pertinents des spams tout en s'adaptant aux nouveaux types de contenu indésirable ?

## Motivation

La détection efficace de spam améliore non seulement l'expérience utilisateur mais renforce également la sécurité des systèmes de communication. Ce projet offre l'opportunité d'acquérir une expertise pratique sur des outils et des techniques essentiels en apprentissage automatique et NLP, tout en ayant un impact concret.

## Objectifs

- Prétraiter et analyser un dataset de spam en nettoyant et vectorisant les données textuelles.
- Implémenter une validation croisée pour évaluer les performances des modèles de manière rigoureuse.
- Construire et tester plusieurs modèles de classification pour détecter les messages spam, tels que Naïve Bayes, Random Forest, Arbre de décision
- Identifier et améliorer le modèle le plus performant pour garantir une précision optimale dans la détection de spam.

## Étapes du projet

### 1. Préparation des données

- Chargement et exploration du dataset.
- Nettoyage des données (suppression des caractères spéciaux, conversion en minuscules, suppression des mots vides, etc.).
- Vectorisation des données textuelles à l'aide de techniques comme TF-IDF ou CountVectorizer.

### 2. Modélisation

- Implémentation de modèles de classification :
  - Naïve Bayes.
  - Arbre de décision.
  - Forêt aléatoire (Random Forest).
- Validation croisée pour évaluer la performance des modèles.
- Utilisation de métriques telles que la matrice de confusion, la précision, le rappel et le F1-score pour analyser les résultats.

### 3. Évaluation des performances

- Comparaison des performances des modèles.
- Visualisation des matrices de confusion pour identifier les erreurs fréquentes.
- Analyse des points faibles et des biais dans les modèles.

### 4. Résultats et conclusions

- **Naïve Bayes :**

  - Précision globale : 87 %.
  - Matrice de confusion :
    ```
    [[163  39]
     [ 11 179]]
    ```
  - Rapport de classification :
    ```
    Précision    : 82 % (spam), 94 % (non-spam).
    Rappel       : 94 % (spam), 81 % (non-spam).
    ```

- **Arbre de décision :**

  - Précision globale : 90 %.
  - Matrice de confusion :
    ```
    [[194   8]
     [ 30 160]]
    ```
  - Rapport de classification :
    ```
    Précision    : 95 % (spam), 87 % (non-spam).
    Rappel       : 84 % (spam), 96 % (non-spam).
    ```

- **Random Forest :**

  - Précision globale : 90.56 %.

## Conclusion

Le modèle Naïve Bayes est le plus adapté, car il offre un rappel élevé de 94 % pour la classe des spams, indiquant qu'il identifie presque tous les spams correctement. Bien que sa précision globale soit légèrement inférieure à celle de Random Forest et Decision Tree, sa capacité à minimiser les faux négatifs en fait un choix optimal pour une tâche axée sur la détection des spams.

## Perspectives futures

- Exploration de modèles plus avancés tels que les réseaux neuronaux récurrents (RNN) ou transformateurs pour améliorer encore la précision.
- Adaptation du modèle à différents types de spam, comme les spams visuels ou les messages sur les réseaux sociaux.
- Intégration du modèle dans une application en temps réel pour filtrer automatiquement les messages.

## Installation et utilisation

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/TressyIssa/spam-detection-with-NLP.git
   ```
2. Installez les dépendances :
   ```bash
   pip install -r requirements.txt
   ```
3. Lancez le script principal :
   ```bash
   python main.py
   ```

## Contributions

Les contributions sont les bienvenues ! Veuillez ouvrir une issue ou soumettre une pull request pour proposer des améliorations.

---

Pour toute question ou suggestion, n'hésitez pas à contacter l'équipe de développement.

