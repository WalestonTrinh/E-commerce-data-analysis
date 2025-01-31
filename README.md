# E-commerce-data-analysis

Introduction du Projet : Analyse de Données E-Commerce
Contexte du Projet

Le dataset utilisé dans ce projet est synthétique et ne contient pas de variations significatives. Malgré cela, j'ai appliqué des techniques d'analyse de données pour explorer les tendances potentielles, segmenter les clients, et évaluer l'impact des réductions. Bien que les résultats ne montrent pas d'insights notables, ce projet démontre ma capacité à manipuler des données, et à communiquer mes résultats de manière claire.

Ce projet consiste en une analyse légère d'un jeu de données e-commerce, disponible sur Kaggle. L'objectif principal est de démontrer mes compétences en SQL notamment en analyse de données et en nettoyage de données sur SQL.

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

        Tendances des ventes (mensuelles).

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

- Format des Dates
     
Le nettoyage des données est une étape essentielle pour assurer la qualité et la fiabilité des analyses. Cette section détaille les problèmes rencontrés et les solutions mises en œuvre pour les résoudre.

Lors de l'examen initial des données, j'ai constaté que les dates n'étaient pas dans le format approprié pour une utilisation optimale dans SQL. Les dates étaient initialement au format '12/11/2024', ce qui n'est pas idéal pour les requêtes SQL. Pour remédier à cela, j'ai converti les dates au format '2024-12-11', qui est plus adapté aux opérations SQL.

Avant : '12/11/2024'
Après : '2024-12-11'

 ![image](https://github.com/user-attachments/assets/5e124cfb-82a8-44d6-9b0c-553c3aa820ef)

- Vérification des Valeurs Manquantes

La seconde étape du nettoyage a consisté à vérifier la présence de valeurs manquantes dans les colonnes critiques. Cette vérification est cruciale pour éviter des analyses biaisées ou incomplètes.

![image](https://github.com/user-attachments/assets/7b34b816-c17c-400d-876f-751aaaaf4316)


- Détection et Suppression des Doublons

Ensuite, j'ai procédé à la détection des éventuelles lignes en double. La présence de doublons peut fausser les résultats des analyses, il est donc essentiel de les identifier et de les supprimer.

![image](https://github.com/user-attachments/assets/ac7853d6-0a07-4e88-99e1-e6340a37c3ab)

Nous en avons fini avec la préparations de données et la gestion de potentielles anomalies de données.

## Analyser les tendances

 Cette section présente les analyses effectuées sur les données nettoyées. Elle met en avant les requêtes SQL utilisées et les insights obtenus.

 Commençons par quelques analyses simples afin d'identifier :
 
 ## Les périodes de forte et faible activité :

Voici le code SQL pour analyser la sommes des ventes trié par mois :

![image](https://github.com/user-attachments/assets/9bba0e78-3363-4d0b-82db-5e6e1ae6dfea)

Le résulat obtenu :

![image](https://github.com/user-attachments/assets/b21476f5-2fd5-4e9c-9834-0d248e731bcc)




## Essayons de voir si il y a une corrélation avec le moyen de paiement utilisé :

![image](https://github.com/user-attachments/assets/3e7a62b4-4b21-4f71-b705-4e731c267433)

Résultat :

![image](https://github.com/user-attachments/assets/6d124b1d-22b1-42bb-9182-ea4872449504)

Il ne semble pas y avoir de corrélation non plus












    



