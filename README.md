 # Quel est l’impact des promotions sur les ventes et le chiffre d’affaires d'un site e-commerce ?

Introduction du Projet : Quel est l’impact des promotions sur les ventes et le chiffre d’affaires d'un site e-commerce  ?
Contexte du Projet

📌 Présentation du Projet
Dans ce projet, j’analyse comment les promotions et réductions influencent le nombre de commandes, le chiffre d’affaires et le panier moyen d’un site e-commerce.

es entreprises e-commerce utilisent souvent des promotions pour booster les ventes, mais cela améliore-t-il vraiment le chiffre d’affaires ?
Ce projet répond aux questions suivantes :

✅ Faut-il continuer à appliquer des promotions élevées ?

✅ Toutes les catégories de produits réagissent-elles de la même manière aux réductions ?

✅ Quel est le taux de promotion optimal pour maximiser les revenus ?

Le dataset utilisé dans ce projet est synthétique et ne contient pas de variations significatives. Malgré cela, j'ai appliqué des techniques d'analyse de données pour explorer les tendances potentielles  et évaluer l'impact des réductions. Ce projet démontre ma capacité à manipuler des données, et à communiquer mes résultats de manière claire.

Ce projet consiste en une analyse légère d'un jeu de données e-commerce, disponible sur Kaggle. L'objectif principal est de démontrer mes compétences en SQL notamment en analyse de données et en nettoyage de données sur SQL ainsi qu'en visualisation sur des outils comme PowerBI

Lien Kaggle du dataset utilisé : https://www.kaggle.com/datasets/steve1215rogg/e-commerce-dataset

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

Nous en avons fini avec la préparations de données et la gestion de potentielles anomalies de données. J'en ai également profité pour renommer certaines colonnes afin de faciliter mon travail par la suite (eg. colonne price et colonne discount)












## Analyser les tendances

 Cette section présente les analyses effectuées sur les données nettoyées. Elle met en avant les requêtes SQL utilisées et les insights obtenus.
 
📊 Analyse Exploratoire des Données (EDA)

Avant de me concentrer sur l’impact des promotions, j’ai exploré plusieurs facteurs :

# 1️⃣ Évolution des ventes par mois

❌ Aucune saisonnalité marquée—les ventes sont restées stables sur toute l’année.


Les périodes de forte et faible activité :

Pour comprendre les tendances des ventes au fil du temps, j'ai analysé les revenus mensuels à l'aide de la requête SQL suivante :

![image](https://github.com/user-attachments/assets/9bba0e78-3363-4d0b-82db-5e6e1ae6dfea)

Le résultat obtenu :

![image](https://github.com/user-attachments/assets/b21476f5-2fd5-4e9c-9834-0d248e731bcc)


    Les revenus mensuels varient entre 51,915.08 (novembre) et 76,034.51 (octobre).

    Le mois d'octobre est le plus performant, tandis que novembre est le moins performant.

    Les revenus restent relativement stables entre 68,000 et 74,000 pour la plupart des mois, à l'exception de novembre.


    Pour mieux comprendre ces tendances, j'ai créé un graphique en ligne dans Power BI, montrant l'évolution des revenus mensuels.

Graphique :


Analyse de la Visualisation :

    Le graphique confirme les insights de l'analyse SQL :

        Un pic clair est visible en octobre, avec un revenu de 76,034.51.

        Une baisse significative est observée en novembre, avec un revenu de seulement 51,915.08.

    Les mois de mars à août montrent une performance stable, avec des revenus compris entre 64,000 et 74,000.









## 2️⃣ Méthodes de paiement utilisées

❌ Aucune différence notable—toutes les méthodes sont utilisées de manière équivalente.

📌 Conclusion : Ces facteurs n’ayant pas d’impact significatif, j’ai décidé d’analyser l’effet des promotions sur les ventes et le chiffre d’affaires, ce qui a révélé des insights clés.

 Essayons de voir si il y a une corrélation avec le moyen de paiement utilisé :

![image](https://github.com/user-attachments/assets/3e7a62b4-4b21-4f71-b705-4e731c267433)

Résultat :

![image](https://github.com/user-attachments/assets/6d124b1d-22b1-42bb-9182-ea4872449504)

Il ne semble pas y avoir de corrélation non plus

📌 Conclusion : Ces facteurs n’ayant pas d’impact significatif, j’ai décidé d’analyser l’effet des promotions sur les ventes et le chiffre d’affaires, ce qui a révélé des insights clés.



## 3️⃣ 🎯 Analyse Finale : L'Impact des Promotions sur les Ventes et le Chiffre d’Affaires

1️⃣ Plus la promotion est élevée, moins il y a de commandes

📉 Le nombre de commandes diminue progressivement lorsque les promotions dépassent 20 %.

![image](https://github.com/user-attachments/assets/3d2aca5a-09a5-48d9-8b17-af3103c13b63)


🔎 Explications possibles :

- Les clients perçoivent peut-être les produits trop remisés comme étant de moindre qualité.


  

2️⃣ Plus la promotion est élevée, plus le panier moyen baisse :

![image](https://github.com/user-attachments/assets/f85a7f4a-6570-4284-8852-dd9a126296bc)


🛒 Lorsque les remises augmentent, les clients dépensent moins par commande, ce qui peut signifier :

- Que les produits avec une haute promotion n'ont pas un prix initial plsu elevé que ceux avec une promotion basse. Cela impacte le panier moyen.
    

3️⃣ Plus la promotion est élevée, plus le chiffre d’affaires diminue

💰 Une réduction supérieure à 20 % entraîne une baisse significative du chiffre d’affaires total. Les produits à hautes promotions sont moins cher et sont moins achetés par les clients. Ce phénomène entraine une baisse considérable du chiffre d'affaires pour les produits à haute promotion.

![image](https://github.com/user-attachments/assets/338223ba-0038-45e6-a43b-b66a948cc1e4)

🚀 Conclusion principale : Supprimer les promotions trop élevées permettrait d’augmenter les revenus.


## 📂 Analyse par Catégorie & Recommandations

Mais avant de procéder à une conclusion trop hative, il faudrait vérifier si ce phénomène s'applique à chaque catégorie de produits. En effet, il est possible que les produits electronique puissent profiter pleinement des promotions elevées pour augmenter leur chiffre d'affaires. Retirer hativement ces promotions pourrait impacter cette catégorie de produit.

J'ai donc réalisé un graphique représentant le nombre de commandes (à gauche) et le revenu (à droite) par promotions et par catégories, ainsi chaque manager marketing dans la catégorie peut adapter son pricing & ses promotions dans la gamme de produits correspondants (voir dossier Powerbi pour voir en détail) :

![image](https://github.com/user-attachments/assets/6fe9d6bf-2312-4273-82f4-dca9ea146b38)


Voici également un tableau claire et efficace réalisé sur Excel pour accélérer la prise de décision : 


![image](https://github.com/user-attachments/assets/fd0f8828-563e-4fe1-b9bf-26d0eef207ea)


📌 Justification des Recommandations

Les recommandations présentées dans cette analyse sont basées sur une double approche combinant l’étude des données et une logique business éprouvée dans le secteur de l’e-commerce.


✔ Les recommandations chiffrées (ex: "limiter les promotions à 15-20 %") proviennent directement des tendances observées dans l’analyse des données. Elles sont justifiables car elles reflètent un lien clair entre le niveau des promotions et l’impact sur les ventes et le chiffre d’affaires.

✔ Les recommandations stratégiques (ex: "privilégier les bundles", "ventes privées") ne relèvent pas du marketing pur, mais d’alternatives aux promotions massives. Ces stratégies sont couramment utilisées en e-commerce pour améliorer la rentabilité sans sacrifier le volume des ventes.
📌 Preuves que ces stratégies sont courantes en e-commerce

👉 👕 Vêtements : Les promotions augmentent les ventes mais réduisent la rentabilité. Les ventes privées et programmes de fidélisation sont souvent utilisés par des enseignes comme Zalando Privé ou Veepee pour limiter l’impact des promotions sur les marges.

👉 💄 Beauté : Les grandes marques (ex: Sephora, L’Oréal) évitent les grosses réductions qui dévalorisent leur image et préfèrent offrir des échantillons ou des produits en bundle pour stimuler les ventes tout en maintenant une perception premium.

👉 💻 Électronique : Peu de réductions importantes chez Apple ou Samsung, mais des alternatives comme les financements sans frais et les offres groupées (ex: iPhone + AirPods). Ces stratégies augmentent le panier moyen sans réduire drastiquement les prix.


## 📢 Conclusion

Cette analyse montre que les réductions supérieures à 20 % nuisent au chiffre d’affaires sans augmenter significativement le volume de ventes. Une meilleure stratégie consiste à adapter les promotions par catégorie plutôt que d’appliquer des remises généralisées.







    



