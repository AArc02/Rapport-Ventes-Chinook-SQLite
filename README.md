# Projet 5 — Automatiser les rapports de ventes avec SQL (Chinook / SQLite)
**captures  :**

**SQLite :** 3.46.1

## Objectif
Produire un rapport détaillant les **ventes totales par produit** sur le **dernier trimestre**.

## Base de données
Chinook Database : https://github.com/lerocha/chinook-database  
Fichier SQLite : `ChinookDatabase/DataSources/Chinook_Sqlite.sqlite`

## Livrables
- `chinook-queries.sql` : requêtes SQL (contrôles, rapport, KPI, vues)
- `exports/rapport_ventes_dernier_trimestre.csv` : export CSV du rapport

## Définition du “dernier trimestre”
Période calculée dynamiquement à partir de `MAX(Invoice.InvoiceDate)` :
- `start_date = début du mois (MAX - 2 mois)`
- `end_date   = début du mois suivant MAX` (borne exclusive)

## Exécution
1. Ouvrir `Chinook_Sqlite.sqlite` dans DB Browser for SQLite
2. Exécuter `chinook-queries.sql` (sections dans l’ordre)
3. Exporter le résultat final en CSV

**Auteur :** Arsene   
**Année :** : 2026
