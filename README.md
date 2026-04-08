# Hôpitaux de soins aigus en Grand Est — Distribution et accessibilité

> Projet de datavisualisation universitaire · Santé · Grand Est

---

## Aperçu

Ce site web analyse la **répartition et l'accessibilité des hôpitaux de soins aigus** dans la région Grand Est (France), à l'échelle de chaque commune. L'étude couvre **5 115 communes**, **182 hôpitaux** et **10 départements**.

---

## Structure du projet

```
/
├── index.html                                       # Page d'accueil
├── carte_graphique.html                             # Carte interactive + Nuage de points D3.js
├── infographie.html                                 # Infographie
├── carte_accessibilite_departement_grandest.png     # Carte choroplèthe de l'accessibilité aux établissements par département
├── DEPARTEMENT_GRANDEST_4326.geojson                # Contour de département
├── hopitaux_grand_est_4326.geojson                  # Localisation des hôpitaux
└── distance_commune_hopitaux_Grandest_4326.geojson  # Distance à un établissement la plus proche par commune
```


## Fonctionnalités

### Page 1 — Accueil
- Présentation du sujet : définition des soins aigus, périmètre de l'étude, motivation

### Page 2 — Carte & Graphique
- **Carte choroplèthe** : distance de chaque commune à l'hôpital le plus proche (5 classes Jenks), points hôpitaux colorés par type, tooltips interactifs, filtre par type d'établissement, légende cliquable
- **Nuage de points** : relation population × distance en échelle logarithmique, légende interactive filtrable

### Page 3 — Infographie
- Indicateurs clés
- Graphiques comparatifs par département et type d'espace
- Panorama de 6 politiques publiques liées à l'accès aux soins (PRS Grand Est, SAS, MCS, Loi Rist, MSP/CPTS, Ségur de la Santé)

---

## Données utilisées

| Source | Description | Millésime |
|--------|-------------|-----------|
| **FINESS** | Répertoire national des établissements sanitaires | 2025 |
| **INSEE** | Population communale, zonage en aires urbaines | 2022 |
| **IGN** | Contours communaux et départementaux | — |

---

## Technologies

- **Leaflet.js** (v1.9.4) — carte interactive
- **D3.js** (v7.8.5) — nuage de points

---

Projet réalisé dans le cadre d'un cours de datavisualisation universitaire.  

