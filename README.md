# chatbot_RAG
Assistant RAG sur Documents Personnalisés
Introduction
Ce projet implémente un système de Retrieval Augmented Generation (RAG) qui permet de converser avec des documents PDF personnalisés. L'assistant utilise la puissance des modèles de langage d'OpenAI pour générer des réponses contextuellement riches, en s'appuyant sur les informations extraites de vos propres fichiers.

Fonctionnalités
Chargement facile de PDF: Intégrez un ou plusieurs documents PDF à votre base de connaissances.
Recherche sémantique: Récupération intelligente des passages les plus pertinents de vos documents grâce à ChromaDB.
Génération augmentée: Utilisation de modèles OpenAI (GPT-4o) pour formuler des réponses précises basées sur le contexte récupéré.
Interface utilisateur interactive: Une interface Gradio conviviale pour poser vos questions et obtenir des réponses instantanées.
Technologies Utilisées
Python
OpenAI API: Pour la génération de texte.
ChromaDB: Base de données vectorielle pour le stockage et la récupération sémantique des embeddings.
Sentence Transformers: Pour la création d'embeddings (vecteurs sémantiques) des documents.
PyPDF2: Pour l'extraction de texte à partir de documents PDF.
Gradio: Pour la création d'une interface utilisateur web rapide et facile.
Comment Utiliser (localement)
1. Cloner le dépôt
git clone https://github.com/[VOTRE_NOM_UTILISATEUR]/[NOM_DE_VOTRE_REPO].git
cd [NOM_DE_VOTRE_REPO]
2. Installer les dépendances
pip install -r requirements.txt
# Ou manuellement: pip install openai chromadb sentence-transformers pypdf gradio
3. Configurer votre clé API OpenAI
Créez un fichier .env à la racine du projet et ajoutez votre clé API OpenAI:

OPENAI_API_KEY="votre_clé_api_openai_ici"
4. Placer vos documents PDF
Placez les fichiers PDF que vous souhaitez interroger dans le dossier data/ (ou adaptez le chemin dans le code).

5. Exécuter l'application
python app.py # ou le nom de votre script principal
Accédez à l'interface via l'URL locale fournie par Gradio.

Structure du Projet (Exemple)
.gitignore
README.md
app.py
requirements.txt
data/
├── document1.pdf
└── document2.pdf
rag_db/ # Dossier généré par ChromaDB
Contributeurs
Aronn Yaël Léonard KABORÉ
