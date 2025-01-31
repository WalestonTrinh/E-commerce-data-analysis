# E-commerce-data-analysis

Introduction du Projet : Analyse de Données E-Commerce
Contexte du Projet

Le dataset utilisé dans ce projet est synthétique et ne contient pas de variations significatives. Malgré cela, j'ai appliqué des techniques d'analyse de données pour explorer les tendances potentielles, segmenter les clients, et évaluer l'impact des réductions. Bien que les résultats ne montrent pas d'insights notables, ce projet démontre ma capacité à manipuler des données, à créer des visualisations, et à communiquer mes résultats de manière claire.

Ce projet consiste en une analyse approfondie d'un jeu de données e-commerce, disponible sur Kaggle. L'objectif principal est de démontrer mes compétences en analyse de données, en nettoyage de données, en visualisation, et en communication efficace des insights.

Lien Kaggle : https://www.kaggle.com/datasets/steve1215rogg/e-commerce-dataset

Le dataset contient des informations sur les achats des clients, telles que :

    User_ID : Identifiant unique de l'utilisateur.

    Product_ID : Identifiant unique du produit.

    Category : Catégorie du produit.

    Price (Rs.) : Prix initial du produit.

    Discount (%) : Pourcentage de réduction appliqué.

    Final_Price (Rs.) : Prix final après réduction.

    Payment_Method : Méthode de paiement utilisée.

    Purchase_Date : Date d'achat.

Objectifs du Projet

    Nettoyer et préparer les données : Identifier et gérer les valeurs manquantes, les doublons, et les incohérences.

    Analyser les tendances : Explorer les tendances des ventes, les performances des produits, et le comportement des clients.

    Visualiser les insights : Créer des tableaux de bord interactifs pour communiquer les résultats de manière claire et visuelle.

    Fournir des recommandations : Proposer des actions concrètes pour améliorer les performances de l'entreprise.

Compétences Déployées

    SQL : Pour interroger la base de données, nettoyer les données, et extraire des insights.

    Power BI : Pour créer des visualisations interactives et des tableaux de bord.

    Excel : Pour des analyses complémentaires et des calculs simples.

    Communication : Pour présenter les résultats de manière claire et convaincante.

Étapes du Projet

    Nettoyage des Données :

        Suppression des doublons et des valeurs manquantes.

        Vérification de la cohérence des données (ex : prix négatifs, dates invalides).

    Analyse Exploratoire :

        Tendances des ventes (mensuelles, trimestrielles).

        Segmentation des clients (clients à haute valeur vs. clients occasionnels).

        Performance des produits (meilleurs vendeurs, catégories les plus rentables).

        Impact des réductions sur les ventes.

    Visualisation :

        Création d'un tableau de bord interactif avec Power BI.

        Graphiques clés : tendances des ventes, répartition des catégories, performance des méthodes de paiement.

    Recommandations :

        Optimisation des réductions pour maximiser les revenus.

        Stratégies pour fidéliser les clients à haute valeur.

        Suggestions pour améliorer l'inventaire en fonction des performances des produits.




## Nettoyage des Données et mise en place 

Le nettoyage des données est une étape cruciale pour garantir la qualité des analyses. Cette section décrit les problèmes identifiés et les étapes pour les résoudre.

En premier lieu j'ai remarqué que les dates n'étaient pas au bon format pour pouvoir les utiliser correctement dans SQL.
Il faut modifier du format '12/11/2024' au format '2024-12-11'

![image](https://github.com/user-attachments/assets/5e124cfb-82a8-44d6-9b0c-553c3aa820ef)


En premier lieu, vérifier qu'il n y a pas de valeur nulle dans les colonnes importantes : 

![image](https://github.com/user-attachments/assets/7b34b816-c17c-400d-876f-751aaaaf4316)

Il n'y a aucune valeur nulle.

Ensuite, il faudrait également vérifier qu'il n y a pas de lignes en dupliqué. Si il y en a, il faut les supprimer.

![image](https://github.com/user-attachments/assets/ac7853d6-0a07-4e88-99e1-e6340a37c3ab)

Il n'y a aucune valeur en doublon.

Nous en avons fini avec la préparations de données et la gestion de potentielles anomalies de données.
Nous avons de la chance, la base de donnée était déjà très propre, il n y a pas besoin de faire de calculs complexes ou de jointures.
Nous pouvons maintenant passer à l'analyse des données.


## Analyser les tendances

 Cette section présente les analyses effectuées sur les données nettoyées. Elle met en avant les requêtes SQL utilisées et les insights obtenus.

 Commençons par quelques analyses simples afin d'identifier :
 
- Les ventes mensuelles et trimestrielles.
- Identification des périodes de forte et faible activité.

Voici le code SQL pour analyser la sommes des ventes trié par mois :
![image](https://github.com/user-attachments/assets/9bba0e78-3363-4d0b-82db-5e6e1ae6dfea)

Le résulat obtenu :

![image](https://github.com/user-attachments/assets/b21476f5-2fd5-4e9c-9834-0d248e731bcc)




Résultats et Insights

    Tendances des Ventes : Identification des périodes de forte et faible activité.

    Segmentation des Clients : Détection des clients les plus rentables et des opportunités de fidélisation.

    Performance des Produits : Identification des produits et catégories les plus performants.

    Impact des Réductions : Analyse de l'effet des réductions sur le volume des ventes et les revenus.

    



