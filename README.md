# automatic_classification

La première partie de ce projet revient à effectuer une étude de faisabilité d'un moteur de classification de biens de consommation, afin d'attribuer automatiquement la catégorie de chaque produit. Pour cela, les descriptions textuelles et les images des articles seront analysées. Cependant, avant de pouvoir analyser les données, il est nécessaire de réaliser un prétraitement et une extraction de features. 

Dans le but d'extraire les features texte, les approches suivantes seront employées :
- deux de type "bag-of-words" : comptage simple de mots et Tf-idf.
- trois de type word/sentence embedding : Word2Vec, BERT et USE.

Pour extraire les features image, deux algorithmes seront exploités :
- un de type SIFT.
- un de type CNN Transfer Learning.

Une fois la faisabilité de regrouper automatiquement des articles de même catégorie démontrée, la seconde partie du projet sera entamée. Cette dernière consiste à réaliser une classification supervisée à partir des images.

Les données utilisées sont téléchargeables [ici](https://s3-eu-west-1.amazonaws.com/static.oc-static.com/prod/courses/files/Parcours_data_scientist/Projet+-+Textimage+DAS+V2/Dataset+projet+pre%CC%81traitement+textes+images.zip).

## Description du répertoire

**Fichiers :**
- **_classification.ipynb_** est le notebook Jupyter proposant différentes approches pour la classification supervisée des images.
- **_df_cleaned.csv_** contient les données nettoyées, après prétraitement et feature extraction.
- **_pretraitement_feature_extraction_faisabilite.ipynb_** est le notebook Jupyter permettant le prétraitement et l'extraction des features, ainsi que l'étude de faisabilité du moteur de classification.
- **_requirements.txt_** contient la liste des packages utilisés pour la réalisation du projet.

## Installation

Le projet a été réalisé sur un environnement Python 3.6.15. Les packages peuvent être installés grâce à la ligne de commande suivante :

`pip install -r requirements.txt`
