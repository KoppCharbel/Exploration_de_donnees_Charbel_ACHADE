# Exploration des données Fordgobike-Tripdata

## par Charbel G. ACHADE

## Base de données 

> Le jeu de données que je choisis s'appelle Fordgobike-Tripdata. Cet ensemble de données comprend des informations sur les trajets individuels effectués dans un système de partage de vélos couvrant la grande région de la baie de San Francisco. Fordgobike-Tripdata est un système de partage de vélos où les gens peuvent emprunter un vélo pour aller où ils veulent. Ils peuvent être client ou abonné.

L'ensemble de données peut être trouvé ici : https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv.

Avant de faire mon exploration, j'ai fait quelques nettoyage de données :

- j'ai converti la colonne member_gender en type 'catégory'
- J'ai supprimé les colonnes start_station_latitude, start_station_longitude, end_station_latitude, end_station_longitude, bike_share_for_all_trip
- J'ai converti en datetime les colonnes start_time et end_time.
- J'ai converti user_type en type category
- J'ai supprimer les valeurs manquantes dans le dataset



## Résumé des résultats

> Pour mon exploration, j'ai choisis deux caractéristiques intéressantes : la durée et le type d'utilisateur. Pour avoir une visualisation plus claire, j'ai converti la durée de secondes en minutes. J'ai fait de l'exploration univariée, bivariée et multivariée. Ces explorations m'ont permis d'avoir ces découvertes :


    - La durée de la plupart des trajets à vélo ne dépasse pas 30 mn

    - Il y a plus d'utilisateurs masculins pour ce service que de femmes

    - Le jeudi est le jour de la semaine où le service est le plus utilisé

    - La durée du voyage pour le client est supérieure à la durée des abonnés

    - Les abonnés prennent moins de temps tous les jours de la semaine, par rapport aux clients.




## Informations clés pour la présentation

>  Le service de voyage à vélo compte plus d'abonnés que de clients.

J'ai trouvé ces données très importantes pour ce service car il est essentiel de savoir quelles personnes utilisent le service. Pour le savoir, j'ai utilisé un "countplot" avec le type d'utilisateur comme variable. Il m'a montré qu'environ 160 000 personnes sont abonnées et moins de 20 000 personnes sont clientes.


>  Les abonnés de tous les sexes ont moins de temps d'utilisation du service en minutes que les clients.

Pour découvrir ces données, j'ai utilisé une exploration multivariée entre member_gender, duration_min et user_type. Il a donné une visualisation des données en deux parties. Une partie indiquait la durée en minutes pour les clients de tous les sexes et l'autre partie indiquait la durée en minutes pour les abonnés. Nous pouvons voir sur la visualisation que pour les clients, la durée pour les hommes est d'environ 20 minutes, 23 minutes pour les femmes et plus de 25 minutes pour les autres sexes. Pour les abonnés, la durée moyenne pour les hommes est inférieure à 10 minutes, pour les femmes, elle est légèrement supérieure à 10 minutes et pour les autres, elle est d'environ 15 minutes.
