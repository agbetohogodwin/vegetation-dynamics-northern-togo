# Dynamique spatio-temporelle du couvert végétal, des sols nus et des feux dans le Nord-Togo (2016-2025)

Analyse multi-indices par télédétection satellitaire (Sentinel-2, Google Earth Engine) dans 8 préfectures du Nord-Togo. Projet personnel de développement de compétences en télédétection et analyse spatiale.

## Zone d'étude

8 préfectures : Binah, Dankpen, Doufelgou, Kéran, Cinkassé, Kpendjal-Ouest, Oti-Sud, Tandjouaré

Période : 2016-2025 (saison sèche, janvier-mars)

Résolution spatiale : 20 mètres (Sentinel-2, niveau 2A)


## Indices calculés

NDVI : vitalité de la végétation

BSI : extension des sols nus

dNBR : dynamique des perturbations par le feu


## Résultats principaux

6 préfectures enregistrent une amélioration du couvert végétal (ΔNDVI positif jusqu'à +0,045), toutes avec une densité de population inférieure à 150 hab/km². Cinkassé (450 hab/km²) présente une dégradation triaxiale : perte de végétation (ΔNDVI = -0,023), extension des sols nus (ΔBSI = +0,027) et augmentation de la fréquence des feux (ΔNBR = +0,018).
La corrélation de Spearman entre densité de population et ΔNDVI est de -0,738 (p ≈ 0,05), confirmant la pression démographique comme facteur déterminant de dégradation des paysages agroforestiers.


## Outils

Plateforme : Google Earth Engine (JavaScript)

Analyse zonale et cartographie : QGIS 3.40.0

Statistiques : corrélation de Spearman (n = 8)

Données démographiques : INSEED (recensement 2022)


## Cartes produites

![Evolution de la végétation](https://raw.githubusercontent.com/agbetohogodwin/vegetation-dynamics-northern-togo/main/outputs/EVOLUTION%20DE%20LA%20VEGETATION.png)
![Evolution des feux](https://raw.githubusercontent.com/agbetohogodwin/vegetation-dynamics-northern-togo/main/outputs/EVOLUTION%20DES%20FEUX.png)
![Evolution des sols nus](https://raw.githubusercontent.com/agbetohogodwin/vegetation-dynamics-northern-togo/main/outputs/EVOLUTION%20DES%20SOLS%20NUS.png)


## Structure du dépôt

├── scripts/
│   └── indices_sentinel2_ndtogo.js
│   ├── dnbr_sentinel2_ndtogo.js
├── outputs/
│   ├── EVOLUTION DE LA VEGETATION.png
│   ├── EVOLUTION DES FEUX.png
│   └── EVOLUTION DES SOLS NUS.png
└── README.md


## Statut

Projet personnel d'apprentissage. Article scientifique rédigé, non encore soumis pour publication.
