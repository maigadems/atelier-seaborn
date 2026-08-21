# Atelier Seaborn — Analyse exploratoire des capteurs IoT

## Contexte

Une entreprise possède plusieurs **bâtiments** équipés de **capteurs IoT**. Chaque capteur collecte régulièrement des informations sur la température, l'humidité, la pression, la consommation énergétique, l'état du capteur, le bâtiment, la date et l'heure de la mesure.

Après avoir utilisé **NumPy** pour manipuler les données numériques, **Pandas** pour importer, nettoyer et analyser le dataset, et **Matplotlib** pour réaliser des visualisations, cet atelier utilise **Seaborn** pour réaliser une analyse exploratoire plus riche des données.

## Structure du projet

```
atelier_seaborn_iot/
│
├── data/
│   └── mesures_capteurs.csv
│
├── notebooks/
│   └── atelier_seaborn_iot.ipynb
│
├── exports/
│   ├── temperature.png
│   ├── temperature.pdf
│   └── ...
│
├── venv/                  (environnement virtuel local, non versionné)
├── requirements.txt
└── README.md
```

## Installation

Depuis la racine du dossier `atelier_seaborn_iot/` :

```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Linux / macOS

pip install -r requirements.txt
python -m ipykernel install --user --name venv --display-name "Python 3 (venv)"
```

Puis ouvrir `notebooks/atelier_seaborn_iot.ipynb` et sélectionner le kernel **Python 3 (venv)**.

## Jeu de données

Le fichier `data/mesures_capteurs.csv` contient des mesures de capteurs IoT avec les colonnes suivantes :

| Colonne | Description |
|---|---|
| `id_mesure` | identifiant unique de la mesure |
| `date_heure` | date et heure de la mesure |
| `id_capteur` | identifiant du capteur |
| `batiment` | bâtiment concerné (B001 à B004) |
| `temperature` | température mesurée (°C) |
| `humidite` | humidité mesurée (%) |
| `pression` | pression mesurée (hPa) |
| `consommation` | consommation énergétique |
| `etat` | état du capteur (`OK`, `ALERTE`, `ERREUR`) |

## Progression de l'atelier

- [x] **Setup** — structure du projet, installation, imports, chargement et vérification du DataFrame `df`
- [x] **Partie 1** — Distribution d'une variable avec `histplot()`
- [x] **Partie 2** — Distribution d'une variable avec `kdeplot()`
- [x] **Partie 3** — Distribution d'une variable avec `boxplot()`
- [x] **Partie 4** — Distribution d'une variable avec `violinplot()`
- [x] **Partie 5** — Comptage des catégories avec `countplot()`
- [x] **Partie 6** — Relation entre deux variables avec `scatterplot()`
- [x] **Partie 7** — Régression avec `regplot()`
- [ ] **Partie 8** — Régression avec `lmplot()`
- [ ] **Partie 9** — Corrélations et `heatmap()`
- [ ] **Partie 10** — Analyse multivariée avec `pairplot()`
- [ ] **Partie 11** — Sauvegarde des graphiques dans `exports/`
- [ ] **Partie 12** — Bonus

## Livrable

Ce dossier `atelier_seaborn_iot` est poussé sur un dépôt public GitHub personnel, mis à jour au fur et à mesure de l'avancement avec des messages de commit explicites.
