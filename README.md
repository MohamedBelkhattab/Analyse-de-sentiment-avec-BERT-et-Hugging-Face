
# Analyse de Sentiments avec BERT

Ce projet consiste à entraîner un modèle BERT pour effectuer une **classification de sentiments** à partir de textes. Le modèle est entraîné sur un sous-ensemble des données pour **réduire le temps d'entraînement** tout en conservant les performances de base.

---

##  Contenu du projet

- `sentiment_analysis_bert.ipynb` — Notebook Jupyter principal contenant le code d'entraînement, de validation et d'affichage.
- `README.md` — Fichier de documentation du projet.

---

##  Environnement de développement

Ce projet a été développé dans un environnement Python. Voici les dépendances principales :

###  Versions recommandées
- Python : >=3.8
- Jupyter Notebook

###  Librairies utilisées

Vous pouvez installer les dépendances avec :

```bash
pip install torch transformers scikit-learn pandas matplotlib seaborn
```

Liste des bibliothèques :
- `torch` – pour le deep learning avec PyTorch
- `transformers` – pour utiliser BERT de HuggingFace
- `pandas` – pour manipuler les données
- `matplotlib`, `seaborn` – pour les visualisations
- `scikit-learn` – pour la métrique d’évaluation

---

##  Fonctionnalités du code

Le notebook contient les étapes suivantes :

1. **Chargement des données** : chargement d’un sous-ensemble du dataset pour accélérer l'entraînement.
2. **Prétraitement des textes** : nettoyage, encodage avec le tokenizer BERT.
3. **Construction du modèle** : utilisation de `BertForSequenceClassification`.
4. **Entraînement** : boucle d’apprentissage avec visualisation de la perte (`loss`) et/ou de la précision.
5. **Évaluation** : affichage d’une matrice de confusion et d’un graphique des probabilités par classe.
6. **Visualisations** : courbe de perte ou de précision, heatmap, barplot.

---

##  Remarques

- Le notebook est annoté avec des titres et des commentaires pour faciliter la compréhension, même si vous avez un niveau débutant.
- L'entraînement est fait sur un **petit échantillon de données** pour gagner du temps lors des tests et de l'apprentissage.
- Certaines parties du code peuvent être modifiées pour afficher soit la `loss`, soit la `précision`, selon le besoin.

---

##  Exécution du projet

Vous pouvez lancer le projet avec :

```bash
jupyter notebook sentiment_analysis_bert.ipynb
```

---

##  Auteur
Mphamed Belkhattab & Mouad Ainouz

Projet réalisé dans le cadre d’un apprentissage personnel sur les modèles NLP et le fine-tuning de BERT.
