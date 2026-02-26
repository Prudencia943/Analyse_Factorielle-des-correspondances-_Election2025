# 🗳️ Analyse Factorielle des Correspondances — Élections Présidentielles 2025 (Cameroun)

## 📋 Description

Ce projet applique une **Analyse Factorielle des Correspondances (AFC)** sur les résultats des élections présidentielles camerounaises de 2025. L'objectif est d'explorer les relations entre les **candidats** et les **régions**, en révélant les profils de vote régionaux et les affinités géographiques de chaque candidat.

---

## 🗂️ Structure du projet

```
├── AFC_Election2025.ipynb       # Notebook principal d'analyse
├── Statitic_election2025.xlsx   # Données brutes des résultats par région
└── README.md
```

---

## 📊 Données

Le fichier `Statitic_election2025.xlsx` contient les résultats de vote de **7 candidats** répartis sur **7 régions** du Cameroun :

| Candidats | Régions couvertes |
|---|---|
| Biya Paul, Issa Chiroma, Cabrel, Belo Bouba, Hiram Samuel, Oshi, Dam Njoya | Centre, Est, Extrême-Nord, Littoral, Nord, Nord-Ouest, Ouest |

---

## 🔬 Méthodologie

L'analyse suit les étapes suivantes :

1. **Chargement et nettoyage des données** — Lecture du fichier Excel et standardisation des colonnes
2. **Calcul des profils** — Profils lignes (candidats) et profils colonnes (régions)
3. **Visualisation des votes** — Diagramme en barres du total des votes par candidat
4. **AFC avec `fanalysis`** — Extraction des axes factoriels, valeurs propres et coordonnées
5. **Analyse des inerties** — Graphiques des valeurs propres (absolues, pourcentage, cumulé)
6. **Qualité de représentation** — Cos² des lignes et colonnes sur les axes 1 et 2
7. **Cartographie factorielle** — Représentation simultanée candidats × régions sur le plan factoriel

---

## ⚙️ Prérequis

```bash
pip install pandas numpy matplotlib openpyxl fanalysis
```

---

## 🚀 Lancement

```bash
jupyter notebook AFC_Election2025.ipynb
```

---

## 📈 Résultats clés

- Identification des **régions d'ancrage** de chaque candidat
- Mise en évidence des **profils de vote similaires** entre régions
- Représentation graphique des **affinités candidat-région** sur le plan factoriel
- Export des coordonnées factorielles dans `Coordonnees regions.xlsx`

---

## 🛠️ Technologies

![Python](https://img.shields.io/badge/Python-3.x-blue) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange) ![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)

---

## 👤 Auteur

Projet réalisé dans le cadre d'une analyse statistique exploratoire des données électorales camerounaises 2025.
