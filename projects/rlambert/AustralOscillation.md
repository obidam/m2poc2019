# Oscillation Australe

## But

Le but est de visualiser l'oscillations australe (différence de pression entre l'antarctique et les basses latitudes de l'hémisphère sud) grâce aux données satellitaires. Pour une bonne visualisation, on peut regrouper les données en Clusters.

## Dataset

J'ai à disposition les données de pression atmosphérique de surface de l'hémisphère sud, du 01-01-1948 au 31-12-2017.

## Traitement des données

On peut déjà réduire le nombre de données en les moyennant par mois (réduction du pas de temps de 102272 à 840).
Le cycle saisonnier de la variation de pression doit être supprimer pour pouvoir travailler avec l'ensemble des données quelque soit le mois. Pour cela, on cré une climatologie correspondant aux moyennes des données pour chaque mois de l'année. Pour chaque donnée on lui soustrait sa climatologie.

On se retrouve avec un jeu de données de pression de surface à trois dimensions: longitude (144), latitude (37) et temps (840).
Pour clusteriser les données, on doit dimensionner le problème: la position géographique sera l'espace des features et le temps sera le sample. On regroupe la latitude et la longitude ensemble (fonction "stack") pour créer l'espace des features de dimensions 144x37=5328.

On peut normaliser les données afin de supprimer les variations de pression discrètes (exemple: variations dues à la topographie).
De même on peut réduire les données en correlant plusieurs données entre elles (exemple: la variation de pression est la même pour deux points peu éloignés.) La réduction fait passer la dimention des features de 5328 à 398.

## Clustering

On réalise un clustering par la méthodes KMeans avec un nombre de clusters défini à 2. On crée une variable "Labels" à la dimension "time" ayant pour valeurs 0 ou 1 en fonction du cluster auquel elle appartient.

On crée ensuite 2 datasets "lab0" et "lab1" pour stocker les données du cluster 1 ou du cluster 2 dans 2 datasets differents. En même temps, on peut unstacker la dimension "features" pour retrouver les dimensions latitude, longitude et temps.

On peut ensuite moyenner en temps les données de chaque dataset avant de ploter les données en latitude/longitude.
On retrouve bien deux cartes (inversées) correspondant aux 2 clusters. Le trait de côte est très reconnaissable.
