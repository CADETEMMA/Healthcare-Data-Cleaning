# Healthcare-Data-Cleaning

Descrption : 
Nettoyage et harmonisation d’un jeu de données cliniques non structurées contenant des informations sur des patients : âge, poids, groupe sanguin et prescriptions de médicaments.
L’objectif était de corriger les erreurs, gérer les valeurs manquantes et standardiser les prescriptions pour rendre les données exploitables pour des analyses ultérieures ou du machine learning.

Détails du datset : 
Fichier : donnees_cliniques1.csv
Variables :
patient_id : Identifiant unique du patient
date_consultation : Date de consultation (jj/mm/aa)
age : Âge du patient
poids : Poids en kg
groupe_sanguin : Groupe sanguin
prescription_medicament : Médicament prescrit
Taille : 50 patients, 6 colonnes
Certaines valeurs étaient manquantes ou aberrantes (ex : âge = 300, poids = 0, médicaments mal orthographiés)

Nettoyage : 
1) Correction des colonnes : Suppression des espaces invisibles, Uniformisation du format des dates (datetime)
2) Nettoyage des valeurs numériques : Âge : valeurs <0 ou >100 remplacées par NaN, Poids : valeurs <2 ou >300 remplacées par NaN
3) Harmonisation des médicaments : Standardisation des différentes écritures du même médicament (paracetamol, Doliprane, EFFERALGAN, etc.) en une seule catégorie paracetamol
4) Vérification des valeurs manquantes : age : 4 valeurs manquantes, poids : 34 valeurs manquantes
5) Visualisations : Histogrammes avant/après nettoyage pour age, Barplot des valeurs manquantes par colonne, Tableau des médicaments uniques avant/après nettoyage

Résultats : 
Les colonnes numériques sont désormais cohérentes et exploitables
Les prescriptions de médicaments sont unifiées :
Avant nettoyage : 7 variantes pour le paracétamol (PARACETAMOL, Doliprane, DAFFALGAN, etc.)
Après nettoyage : 1 seule catégorie paracetamol
Visualisations permettent de détecter facilement les valeurs manquantes et aberrantes

Compétences :
Python : pandas, numpy, matplotlib, seaborn
Data cleaning / wrangling
Gestion des valeurs manquantes
Harmonisation et standardisation des données textuelles (regex, fonctions Python)
Visualisation pour Python : pandas, numpy, matplotlib, seaborn (Histogrammes pour age et poids avant/après nettoyage, Heatmap et Barplot des valeurs manquantes)
Visualisation pour data quality checks



