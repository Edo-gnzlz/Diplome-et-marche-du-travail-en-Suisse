# Diplômes & marché du travail en Suisse

Projet RMarkdown analysant la montée de la formation tertiaire en Suisse et ses liens avec le marché du travail, les bourses d’études, les pénuries de main-d’œuvre qualifiée et l’inadéquation formation-emploi.

## Objectif du projet

Le projet cherche à comprendre comment le niveau de formation de la population suisse a évolué dans le temps, puis à mettre cette évolution en relation avec les besoins du marché du travail.

Il s’appuie notamment sur des données de l’OFS et du SECO.

## Contenu du projet

- Évolution cantonale de la formation tertiaire
- Montée du tertiaire par région linguistique
- Différences générationnelles selon l’âge
- Comparaison entre bénéficiaires de bourses et effectifs étudiants
- Indice de pénurie de main-d’œuvre qualifiée par groupe de professions
- Inadéquation entre formation et emploi
- Projection du niveau de formation de la population jusqu’en 2055

## Structure recommandée

```text
education-suisse/
├── Diplome_et_marche_du_travail2.Rmd
├── data/
│   ├── formation_tertiaire.csv
│   ├── seco_indice_penurie_qualifiee_2023.csv
│   ├── inadequation_TA3.csv
│   └── autres fichiers de données OFS/SECO
├── README.md
└── .gitignore
```

## Données

Les fichiers de données doivent être placés dans le dossier `data/`.

Le fichier `.Rmd` est prévu pour chercher automatiquement les données soit dans `data/`, soit dans le même dossier que le fichier `.Rmd`.

## Packages R utilisés

Le projet utilise principalement les packages suivants :

```r
tidyverse
readxl
scales
fmsb
sf
svglite
xml2
jsonlite
htmltools
ggrepel
```

## Reproduire l’analyse

1. Cloner le dépôt :

```bash
git clone https://github.com/ton-utilisateur/education-suisse.git
cd education-suisse
```

2. Ouvrir le fichier `.Rmd` dans RStudio.

3. Installer les packages nécessaires si besoin :

```r
install.packages(c(
  "tidyverse", "readxl", "scales", "fmsb", "sf",
  "svglite", "xml2", "jsonlite", "htmltools", "ggrepel"
))
```

4. Vérifier que les fichiers de données sont bien dans le dossier `data/`.

5. Générer le rapport HTML avec le bouton **Knit** dans RStudio.

## Auteur

Eduardo Gonzalez
