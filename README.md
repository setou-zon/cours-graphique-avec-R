# Cours R en Épidémiologie - Méningite Burkina Faso 2025

## Description

Formation complète sur l'utilisation de R pour l'analyse épidémiologique avec les données réelles de méningite du Burkina Faso 2025.

## Contenu du Cours

### 1. Courbes Épidémiologiques
- Courbe épidémique classique avec identification des pics
- Stratification par groupe d'âge (aires empilées)
- Courbes avec seuils d'alerte épidémiologique
- Analyse par région (top 6 régions)
- Analyse temporelle détaillée (cas, décès, létalité)
- Tableau de bord complet pour décideurs

### 2. Tableaux Flextable
- Tableau de surveillance par région et semaine
- Formatage conditionnel professionnel
- Coloration selon les valeurs (vert pour cas > 0)
- Export en Word, HTML et CSV

### 3. Cartes Choroplèthes
- Carte des décès par district sanitaire
- Carte du taux de létalité
- Analyse spatiale de la mortalité
- Recommandations épidémiologiques

## Données Utilisées

- **1 157 cas** de méningite analysés
- **27 semaines épidémiologiques** (janvier-juillet 2025)
- **13 régions** du Burkina Faso
- Variables : semaine_epi, region, age_en_annees, sexe, resultat_final_national

## Packages R Requis

```r
library(ggplot2)      # Graphiques
library(dplyr)        # Manipulation des données
library(tidyr)        # Reshape des données
library(scales)       # Formatage des axes
library(patchwork)    # Combinaison de graphiques
library(readxl)       # Lecture Excel
library(lubridate)    # Gestion des dates
library(RColorBrewer) # Palettes de couleurs
library(flextable)    # Tableaux professionnels
library(sf)           # Données géospatiales
```

## Utilisation

1. Clonez ce repository
2. Ouvrez `index.html` dans votre navigateur
3. Suivez les sections du cours dans l'ordre
4. Utilisez le code R fourni avec vos propres données

## Fichiers Générés

Le script R complet génère :
- **6 graphiques PNG** haute résolution (300 DPI)
- **Tableaux flextable** en Word et HTML
- **Cartes choroplèthes** individuelles et combinées
- **Fichiers CSV** avec données agrégées

## Auteur

Direction Générale de la Santé Publique - Burkina Faso

## Licence

Ce cours est destiné à des fins éducatives et de formation en santé publique.

## Déploiement

Ce site est optimisé pour GitHub Pages. Pour le déployer :

1. Forkez ce repository
2. Activez GitHub Pages dans les paramètres
3. Sélectionnez la branche `main` comme source
4. Votre site sera disponible à l'adresse : `https://votre-username.github.io/nom-du-repo`

## Support

Pour toute question ou support technique, contactez l'équipe de formation en épidémiologie.

