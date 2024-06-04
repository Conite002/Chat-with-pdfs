# Application de Discussion MultiPDF


## Introduction
------------
L'Application de Discussion MultiPDF est une application Python qui permet de dialoguer avec plusieurs documents PDF. Vous pouvez poser des questions en langage naturel sur les PDFs, et l'application fournira des réponses pertinentes basées sur le contenu des documents. Cette app utilise un modèle de langage pour générer des réponses précises à vos questions. Veuillez noter que l'app ne répondra qu'aux questions relatives aux PDFs chargés.

## Fonctionnement
------------

![Diagramme de l'Application de Discussion MultiPDF](./docs/PDF-LangChain.jpg)

L'application suit ces étapes pour fournir des réponses à vos questions :

1. Chargement des PDF : L'app lit plusieurs documents PDF et en extrait le contenu textuel.

2. Fragmentation du Texte : Le texte extrait est divisé en petits blocs plus faciles à traiter.

3. Modèle de Langage : L'application utilise un modèle de langage pour générer des représentations vectorielles (embeddings) des blocs de texte.

4. Correspondance de Similitude : Lorsque vous posez une question, l'app compare celle-ci avec les blocs de texte et identifie les plus semblables sémantiquement.

5. Génération de Réponse : Les blocs sélectionnés sont transmis au modèle de langage, qui génère une réponse basée sur le contenu pertinent des PDFs.

## Dépendances et Installation
----------------------------
Pour installer l'Application de Discussion MultiPDF, veuillez suivre ces étapes :

1. Clonez le dépôt sur votre machine locale.

2. Installez les dépendances requises en exécutant la commande suivante :


3. Obtenez une clé API d'OpenAI et ajoutez-la au fichier `.env` dans le répertoire du projet.
```commandline
OPENAI_API_KEY=votre_cle_api_secrete
```

## Utilisation
-----
Pour utiliser l'Application de Discussion MultiPDF, suivez ces étapes :


      npm install
      npm run start


## Contribution
------------
Ce dépôt est destiné à des fins éducatives et n'accepte pas de contributions supplémentaires. Il sert de matériel de soutien pour un tutoriel YouTube qui montre comment construire ce projet. N'hésitez pas à utiliser et à améliorer l'application selon vos propres besoins.
