# **TP_PrédicteurAvisSteam_Hakima_Djermouni**

## **Description du projet**

Ce projet, intitulé **TP_PrédicteurAvisSteam_Hakima_Djermouni**, vise à prédire si un utilisateur de la plateforme Steam va recommander ou non un jeu en fonction de son commentaire. Le modèle utilise un jeu de données contenant les avis des utilisateurs et d'autres informations comme le titre du jeu, l'année de l'avis, et la suggestion de l'utilisateur (recommander ou non).

L'objectif principal est de construire un modèle prédictif basé sur les avis textuels des utilisateurs pour déterminer si l'utilisateur recommande le jeu.

## **Structure du projet**

Le projet se déroule en plusieurs étapes :

1. **Exploration des données** : Analyse statistique du jeu de données (nombre de mots, longueur des phrases, équilibrage des classes, etc.).
2. **Nettoyage des données** : Gestion des valeurs manquantes et normalisation des données.
3. **Modélisation** : Création et entraînement du modèle de prédiction à partir des commentaires des utilisateurs.
4. **Évaluation** : Mesure des performances du modèle avec des métriques comme l'exactitude, la précision, le rappel, etc.

## **Dépendances**

Pour exécuter ce projet, vous aurez besoin des bibliothèques Python suivantes :

- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `nltk` (pour le traitement du texte)

Vous pouvez installer ces bibliothèques en exécutant la commande suivante :

```bash
pip install pandas matplotlib seaborn scikit-learn nltk
```

## **Instructions d'utilisation**

1. **Cloner le projet** :
   Clonez ce dépôt Git sur votre machine locale en utilisant la commande suivante :
   ```bash
   git clone https://github.com/username/TP_PrédicteurAvisSteam_Hakima_Djermouni.git
   ```

2. **Ouvrir le notebook** :
   Ouvrez le fichier Jupyter Notebook (`TP_PrédicteurAvisSteam_Hakima_Djermouni`) dans Google Colaboratory ou Jupyter Lab.

3. **Exécuter le notebook** :
   Suivez les instructions dans le notebook pour charger le jeu de données, analyser les données, et entraîner les modèles.

## **Exemple d'utilisation**

Voici un exemple de la façon dont le projet utilise le jeu de données Steam pour l'exploration et la prédiction :

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Chargement des données
steam_data = pd.read_csv('chemin/vers/le/fichier/steam.csv')

# Affichage des informations du jeu de données
print(steam_data.info())

# Visualisation de la distribution des suggestions des utilisateurs
sns.countplot(data=steam_data, x='user_suggestion')
plt.show()
```

## **Contribuer**

Les contributions sont les bienvenues ! Si vous souhaitez apporter des améliorations ou ajouter de nouvelles fonctionnalités, ouvrez une issue ou soumettez une pull request.

## **Licence**

Ce projet est sous licence MIT. Pour plus d'informations, veuillez consulter le fichier `LICENSE`.

## **Auteur**

Le projet a été réalisé par **Hakima Djermouni**.
