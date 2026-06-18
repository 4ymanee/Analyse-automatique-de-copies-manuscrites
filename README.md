# AutoCorrect AI

## Description du Projet (Sujet)
Le projet **AutoCorrect AI** a pour objectif de soulager la charge de travail des enseignants en automatisant le processus fastidieux de correction des copies d'examen manuscrites. 

Grâce aux technologies d'intelligence artificielle, le système est capable de :
1. **Lire l'écriture manuscrite** via des moteurs d'OCR avancés (Tesseract, EasyOCR).
2. **Analyser et évaluer les réponses** en utilisant l'approche RAG (Retrieval-Augmented Generation) couplée à des modèles de langage de pointe (GPT-4o / LangChain), ce qui permet de comparer les réponses des étudiants à un corrigé de référence.
3. **Fournir une interface de gestion** complète : un tableau de bord pour l'enseignant (pour téléverser les sujets, les copies et suivre les statistiques de correction) et un espace pour l'étudiant (pour consulter ses résultats et les annotations sur ses copies).

En résumé, ce système vise à numériser, accélérer et standardiser la correction des examens tout en réduisant le risque d'erreur humaine.

## Fonctionnalités
- Upload de copies scannées
- OCR (Tesseract / EasyOCR)
- RAG pour la correction automatique avec LangChain et GPT-4o
- Tableau de bord enseignant et espace étudiant

## Lancement avec Docker Compose

1. Clonez ce dépôt.
2. Copiez `.env.example` vers `.env` et ajoutez votre clé API OpenAI.
3. Lancez les conteneurs :
   ```bash
   docker-compose up --build
   ```
4. Accédez au frontend sur `http://localhost:5173` et l'API sur `http://localhost:8000`.
