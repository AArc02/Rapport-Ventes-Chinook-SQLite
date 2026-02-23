# Projet 5 — Automatiser les rapports de ventes avec SQL (Chinook / SQLite)
**SQLite :** 3.46.1

**captures  :**
<img width="1469" height="847" alt="controle des tables principaux" src="https://github.com/user-attachments/assets/cb63db9c-6a0f-4c16-b239-ee7c54a37632" />
<img width="1469" height="847" alt="KPI prix moyen pondéré" src="https://github.com/user-attachments/assets/92b65ab3-dbef-4993-b191-5938d8ffa052" />

<img width="1469" height="847" alt="Rapport vente totale" src="https://github.com/user-attachments/assets/5b092660-7aea-42cf-9dcf-d15fca4b6dfd" />

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
