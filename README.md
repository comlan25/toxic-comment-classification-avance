# ⚠️ Détection Avancée de Commentaires Toxiques (NLP)

Ce projet constitue la **suite évolutive** du projet `toxic-comment-classification`. Alors que la première version se concentrait sur des modèles de Machine Learning classiques (TF-IDF, SVM, Random Forest), cette itération adopte une **approche beaucoup plus avancée** intégrant le Deep Learning et les Large Language Models (LLM).

## Évolution du Projet
Par rapport à la version initiale, ce dépôt introduit :
* **Vecteurs de mots contextuels** (Word Embeddings pré-entraînés).
* **Modèles de langage transformeurs** (BERT) pour une compréhension sémantique profonde.
* **Techniques de Prompt Engineering** pour évaluer les capacités de raisonnement des modèles modernes.

## Fonctionnalités Avancées
Le notebook explore trois piliers technologiques :

1. **Vecteurs Pré-entraînés (GloVe)** : Utilisation de **GloVe (300d)** avec une Régression Logistique pour capturer les relations sémantiques entre les mots.
2. **Deep Learning (Transformers)** : Mise en œuvre de **Toxic-BERT** via Hugging Face, atteignant un niveau de précision inégalé pour la détection de nuances fines de toxicité.
3. **Prompt Engineering (LLM)** : Comparaison de stratégies **Zero-shot**, **Role prompting** et **Few-shot prompting** avec le modèle **BART-large-mnli** pour tester la classification sans réentraînement.

## Performance & Comparaison
Les résultats démontrent la supériorité des approches basées sur les Transformers par rapport au projet initial :

* **Transformers (BERT)** : Performances exceptionnelles avec une **Accuracy de 98%** et un **AUC de 0.995**.
* **GloVe + LR** : Approche robuste et rapide avec un **AUC de 0.947**.
* **Prompt Engineering** : Le **Few-shot prompting** montre une nette amélioration par rapport au Zero-shot, prouvant l'importance du contexte pour les LLM.

## Stack Technique
* Langage : Python
* NLP : NLTK, Gensim, Hugging Face Transformers
* ML : Scikit-learn
* Visualisation : Seaborn, Matplotlib

## 📊 Performance & Comparaison
## 📊 Performance & Comparaison
Les résultats démontrent la supériorité des approches basées sur les Transformers par rapport au projet initial :

* **Transformers (BERT)** : Performances exceptionnelles avec une **Accuracy de 98%** et un **AUC de 0.995**.
* **GloVe + LR** : Approche robuste et rapide avec un **AUC de 0.947**.
* **Prompt Engineering** : Le **Few-shot prompting** montre une nette amélioration par rapport au Zero-shot, prouvant l'importance du contexte pour les LLM.


## 🛠️ Installation
```bash
# Cloner le dépôt de cette version avancée
git clone [https://github.com/comlan25/toxic-comment-classification-avance.git](https://github.com/comlan25/toxic-comment-classification-avance.git)

# Installer les dépendances (inclus Transformers, Torch, Gensim)
pip install -r requirements.txt