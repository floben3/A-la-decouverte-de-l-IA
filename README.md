# À la découverte de l'Intelligence Artificielle

Activité de découverte de l'Intelligence Artificielle à destination des Cordées de la réussite du collège Pierre Flamens, dans le cadre du programme Ô Talents de l'INSA Toulouse.

[![Ouvrir dans Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mefZHeN_jHU4WbfOrX6NrEKxlk2iA_42?usp=sharing)

Ce dépôt contient un notebook pédagogique et interactif pour faire découvrir plusieurs familles d'intelligence artificielle à des élèves de collège. L'activité alterne explications, manipulations guidées, visualisations et temps de réflexion critique.

## Objectifs pédagogiques

- Comprendre que l'IA n'est pas magique : elle repose sur des données, des calculs et des choix humains.
- Découvrir la différence entre IA symbolique, apprentissage automatique et apprentissage par renforcement.
- Manipuler des modèles simples pour générer du texte, entraîner un agent de jeu et reconnaître des chiffres manuscrits.
- Identifier les limites des modèles : erreurs, biais, surapprentissage, dépendance aux données.
- Ouvrir une discussion sur les impacts sociaux, écologiques et culturels de l'intelligence artificielle.

## Public visé

L'activité est conçue pour des collégiens participant aux Cordées de la réussite. Elle ne suppose pas de prérequis avancés en programmation ou en mathématiques : les notions sont introduites progressivement, avec des exemples concrets et des interfaces interactives.

## Contenu de l'activité

### 1. Génération de texte

Les élèves construisent un mini-modèle de langage basé sur des trigrammes. Ils découvrent les notions de corpus, tokenisation, contexte, probabilités et choix pondéré, puis utilisent une interface `ipywidgets` pour générer de courtes phrases.

### 2. Apprentissage par renforcement

Les élèves entraînent un agent à traverser l'environnement `FrozenLake` avec une table Q. L'atelier met en évidence l'exploration, l'exploitation, les récompenses, les essais-erreurs et la difficulté supplémentaire introduite par un environnement glissant.

### 3. Reconnaissance d'images

Les élèves utilisent le jeu de données MNIST pour entraîner un réseau de neurones capable de reconnaître des chiffres manuscrits. L'atelier introduit les pixels, la normalisation, le one-hot encoding, les couches de neurones, les poids, les biais, l'entraînement et la validation. Une interface Gradio permet ensuite de tester ses propres dessins.

### 4. Esprit critique et débat

La fin de l'activité propose une prise de recul sur les usages de l'IA dans le monde réel : biais, données personnelles, consommation énergétique, ressources naturelles, travail humain invisible, santé mentale, transformation des métiers et représentations culturelles.

## Fichiers principaux

- [`IA_introduction_ludique_Cordees_de_la_reussite.ipynb`](IA_introduction_ludique_Cordees_de_la_reussite.ipynb) : notebook principal de l'activité.

## Utilisation

### Option recommandée : Google Colab

Le plus simple est d'ouvrir directement le notebook dans Google Colab :

[Ouvrir l'activité interactive](https://colab.research.google.com/drive/1mefZHeN_jHU4WbfOrX6NrEKxlk2iA_42?usp=sharing)

Colab évite d'avoir à installer localement les dépendances lourdes, notamment TensorFlow et Gradio.

Le notebook contient aussi des cellules `pip install` prévues pour Colab. En local, il est préférable d'installer les dépendances une fois dans l'environnement virtuel, puis d'exécuter les cellules dans l'ordre.

## Points d'attention

- Les résultats peuvent varier d'une exécution à l'autre, car certains ateliers utilisent du hasard.
- L'entraînement FrozenLake en mode glissant peut parfois échouer ou progresser lentement : cela fait partie de l'activité.
- Les interfaces interactives utilisent `ipywidgets` et `gradio`.
- Les fichiers `frozen_lake8x8.pkl` et `frozen_lake8x8.png` peuvent être régénérés en relançant l'entraînement correspondant dans le notebook.

## Sources et inspirations

Les sources détaillées sont listées dans le notebook et dans la page de présentation. Elles incluent notamment des cours d'introduction à l'IA, des ressources EFELIA Côte d'Azur, des contenus de 3Blue1Brown, un tutoriel sur le Q-learning et des références pour discuter des impacts sociaux et environnementaux de l'IA.

## Contact

Activité proposée par Antoine et Florian, INSA Toulouse.

Pour toute question ou remarque : [fdelbreil@insa-toulouse.fr](mailto:fdelbreil@insa-toulouse.fr)