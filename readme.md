# Analyse et Explication Automatique des Décisions de Crédit Immobilier grâce aux Transformers et aux LLM

## Description

Ce projet explore comment les modèles Transformers, utilisés dans les Large Language Models (LLM) comme GPT, Mistral ou Llama, peuvent être appliqués au secteur bancaire pour améliorer :

l’analyse des demandes de crédit immobilier,

la compréhension des décisions (accord ou refus),

l’explicabilité des modèles,

la transparence vis-à-vis des clients et des conseillers.

Nous développons un Proof of Concept (PoC) combinant :

un modèle de scoring (Machine Learning classique),

un module d’explication automatique basé sur un LLM,

une analyse théorique du modèle Transformer, cœur des IA génératives modernes.

## Objectifs

Comprendre le fonctionnement interne du Transformer (self-attention, multi-head attention…).

Construire un modèle prédictif simple pour l’attribution des crédits.

Utiliser un LLM pour générer des explications textuelles des décisions du modèle.

Montrer concrètement comment l’IA générative peut aider à la prise de décision bancaire.

Préparer un environnement technique reproductible en Python.

## Équipe projet

Projet réalisé dans le cadre du Cycle Ingénieur Big Data.

'''markdown
Nom	
Akle Kénan         Responsable technique : PoC, scoring, intégration API
Da-Silva Hermila   Veille technique : Transformers & architectures IA
Dedegbe Sarah      Données : préparation et nettoyage du dataset
Kounou Modjisola   Rédaction & rapport
Tiamiyou Safir	   Démo, interface & visualisation
'''

## Structure du dépôt

 '''markdown
credit-transformer-project/
│
├── notebooks/                # Jupyter Notebooks d'analyse
│   ├── S1_setup_environment.ipynb
│   ├── S2_data_preparation.ipynb
│   ├── S3_credit_scoring_model.ipynb
│   ├── S4_llm_explanations.ipynb
│   └── S5_final_demo.ipynb
│
├── data/
│   ├── raw/                  # Données brutes (origine Kaggle/UCI)
│   └── processed/            # Données nettoyées et prêtes pour ML
│
├── src/                      # Scripts Python réutilisables
│   ├── model_training.py
│   ├── credit_explainer.py
│   └── utils.py
│
├── reports/
│   ├── veille/               # Documents de recherche
│   └── rapport_final/        # Rapport complet du projet
│
├── requirements.txt          # Dépendances Python
└── README.md                 # Ce fichier
'''


## Technologies utilisées

Python 3.10+

Pandas / NumPy

Scikit-learn (scoring de crédit)

OpenAI ou Mistral API (LLM pour explication)

Jupyter Notebook (analyse & PoC)

Matplotlib / Seaborn (visualisation)

Streamlit (optionnel – interface de démo)

## Fonctionnement du PoC

Le Proof of Concept repose sur un pipeline à 3 étapes :

Entrée des données du client
(revenu, apport, durée, âge, taux d’endettement, historique…)

Prédiction du modèle ML
→ “Crédit accordé” ou “Crédit refusé”

Explication générée par le LLM
Exemple :

“Le crédit est refusé car le taux d’endettement dépasse 40 % et l’apport est insuffisant.”

Ce pipeline combine modèle prédictif + modèle génératif.

## Objectifs pédagogiques atteints

Compréhension de l’architecture Transformer.

Approche hybride ML + IA générative.

Manipulation de données financières simulées.

Construction d’un PoC professionnel.

Travail d'équipe structuré (veille, code, rapport, démo).