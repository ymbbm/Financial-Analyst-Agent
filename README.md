#  Financial Analyst Agent — Fine-tuning LLaMa 3 + RAG sur données SEC 10-K

Ce projet a été réalisé dans un cadre académique à CentraleSupélec, dans le cadre du cours **Intelligence Artificielle**, supervisé par **Hugues Talbot**.

L'objectif est de construire un agent capable de répondre à des questions financières en langage naturel à partir de **rapports annuels 10-K** d'entreprises cotées aux États-Unis, en combinant :

- **Fine-tuning local** de LLaMa 3 (8B Instruct) sur des données Q&A financières
- **Pipeline RAG (Retrieval-Augmented Generation)** avec base vectorielle FAISS
- **Embeddings sémantiques locaux**
- **Récupération automatique des rapports 10-K** via l'[API SEC](https://sec-api.io/)

---

##  Fonctionnalités

-  Fine-tuning du modèle LLaMa 3 à l'aide d'**Unsloth** et **LoRA**
-  Utilisation d’un jeu de données QA spécialisé sur les 10-K (Hugging Face)
-  Recherche sémantique dans les documents avec **FAISS**
-  Téléchargement dynamique des rapports 10-K récents via l'API SEC
-  Interface interactive : l’utilisateur pose une question, le modèle répond avec contexte

---

## 🗂 Structure
financial-analyst-agent/
├── notebooks/
│ └── Financial_Analyst_Agent.ipynb
├── .env 
├── requirements.txt
├── .gitignore
├── README.md

## Utilisation
1- Ouvrir le notebook notebooks/Financial_Analyst_Agent.ipynb dans Google Colab.

2- Exécuter les cellules dans l’ordre (GPU recommandé).


3- Interagir avec l’agent en posant des questions financières liées à un rapport 10-K.

## Ressources utilisées
Meta LLaMa 3 8B Instruct

Unsloth

Hugging Face Dataset — Financial QA

SEC API

FAISS

## ⚠️ Disclaimer
Ce projet a été réalisé uniquement dans un cadre académique, à l’occasion du cours d’Intelligence Artificielle encadré par Hugues Talbot à CentraleSupélec.
Il ne constitue en aucun cas un conseil en investissement. Le contenu ne doit pas être diffusé ou réutilisé sans autorisation.
