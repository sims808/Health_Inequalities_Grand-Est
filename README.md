# Hôpitaux de soins aigus en Grand Est — Distribution et accessibilité

> Projet de datavisualisation universitaire · Santé · Grand Est

---

## Aperçu

Ce site web analyse la **répartition et l'accessibilité des hôpitaux de soins aigus** dans la région Grand Est (France), à l'échelle de chaque commune. L'étude couvre **5 115 communes**, **182 hôpitaux** et **10 départements**.

---

## Structure du projet

```
/
├── grandest_10v_accueil.html        # Page d'accueil
├── grandest_10v_analyse.html        # Carte Leaflet + Nuage de points D3.js
├── grandest_10v_infographie.html    # Infographie & Politiques publiques
├── dep_carte_sans-Photoroom.png     # Carte choroplèthe des départements
├── DEPARTEMENT_GRANDEST_4326.geojson
├── hopitaux_grand_est_4326.geojson
└── Dist_Com_hopitaux_Grandest_4326.geojson
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

