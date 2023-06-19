# **Nettoyer ses données**

Que ce soit pour des raisons techniques ou organisationnelles, il arrive que les données fournies en format tabulaire ou scrapées soient jugées "sales". Une donnée est jugée sale quand son format gêne son utilisation, que ce soit par un humain ou par une machine.

Plusieurs dimensions d'une base de données peuvent contribuer à sa saleté :
* une source manquante, défectueuse, imprécise ;
* des têtières incompréhensibles, redondantes, incomplètes ;
* des données imbriquées, mal formatées, lacunaires, excédentaires ;
* des colonnes mal agencées, des lignes incohérentes, une mauvaise architecture...

Par opposition, une donnée est propre lorsque : 
* elle est reconnue par la machine pour ce qu'elle est ;
* elle est lisible par l'utilisateur·rice ;
* elle permet de faire les calculs nécessaires.

**Une étape importante de la production de données (standardisées ou non) est donc leur nettoyage.**

**Il n'existe pas de méthode miracle ou universelle**, toutes les bases de données ayant leurs propres lacunes, mais quelques questions clefs permettent tout de même de s’assurer de la propreté « minimale » de ses données : 
1. La source (base de données originale) est-elle accessible ? 
2. Les têtières (noms de champs) sont-elles compréhensibles ? Me permettent-elles de comprendre (directement ou par la documentation) la nature des données que contient ma base ?
3. Les données sont-elles lues correctement par ma machine ?
4. Est-ce que je peux les réutiliser (effectuer des calculs…) ?

## **Quelques conseils**

Voici trois bonnes pratiques concernant le nettoyage des données. 

### 1. **Conserver la source :**

Le nettoyage n'est pas une opération anodine : **vous allez modifier en profondeur votre base de données suivant vos critères dans le cadre d'une analyse spécifique**. De telle manière que les producteur·rices de la base, d'autres utilisateurs ou vous-même dans un futur proche ne seriez pas capable de reconnaître le fichier !

Conserver la source a plusieurs avantages :
* retrouver les données de base en cas d'erreur ;
* citer l'origine de votre analyse sans vous tromper ;
* situer votre source dans le temps et par rapport à d'autres données comparables.

Que vous utilisiez LibreOffice, Excel ou Google sheet, nous vous conseillons **de vous servir de la fonctionnalité "onglets",** qui permet de réunir plusieurs feuilles dans un même document. Nous allons procéder en trois étapes :

> 1. renommer l'onglet principal **source** ;
> 2. dupliquer cet onglet pour créer une feuille de travail ;
> 3. réunir les informations sur la base dans un onglet dédié, **metadata**, avec trois infos :
   > * _nom_ de la source ;
   > * _lien_ de téléchargement ;
   > * _date_ de téléchargement.

![alt_text](https://i.ibb.co/r0dNVPR/Capture-d-e-cran-2023-03-22-a-12-10-54.png)

Au moment de la publication des données, vous ne partagerez bien sûr pas cet onglet, mais l’avoir créé vous permettra de ne pas perdre localement votre source de données !  

### 2. **Comprendre les données**

Dans votre tableur, renommer le fichier et les têtières est essentiel pour **correspondre à un standard de données,** et plus largement pour qu’il soit compris et réutilisé par le plus grand nombre. 

Pour des jeux de données qui ne possèdent pas de standard, il existe peut-être un **dictionnaire commun** pour utiliser les mêmes termes que d'autres collectivités (en France, le CEREMA a par exemple produit [un document regroupant les terminologies recommandées pour décrire l’offre de transport public](https://www.cerema.fr/fr/actualites/referentiel-donnees-offre-transport-public-guide-mise-oeuvre)).

Dans tous les cas, il sera utile, **dans la documentation, de préciser à quoi correspond chaque têtière**.

### 3. **Un outil pour aider au nettoyage des données : Open Refine**

LibreOffice, Excel et Google sheet ont des fonctionnalités pour aider au nettoyage de données : filtres, trouver/remplacer, scinder une colonne (fonction _split_), compiler des données… ([de nombreuses expressions régulières](https://fr.wikipedia.org/wiki/Expression_r%C3%A9guli%C3%A8re) sont à votre disposition). 

**L’outil gratuit et open source Open Refine** offre cependant d’autres fonctionnalités. En plus de trier et gérer les doublons (de la même façon que LibreOffice, Excel et Google sheet), il permet notamment de : 
* Réordonner / supprimer des colonnes
* Les transformations courantes
* Utiliser les facettes
* Diviser une colonne
* Regrouper des valeurs proches (clusterisation)
* Suivre l’historique des modifications (ce qui permet de reproduire facilement les manipulations effectuées)  

> De nombreux tutoriels sont accessibles en ligne, parmi lesquels : 
> * _Une vidéo : **[OpenRefine, "Excel aux hormones" pour nettoyage de données](https://www.patrimoine-et-numerique.fr/tutoriels/52-36-openrefine-excel-aux-hormones-pour-nettoyage-de-donnees)**_
> * _Le tuto de Thomas Padilla (anglais) : **[Getting Started with OpenRefine](https://www.thomaspadilla.org/dataprep/)**_
> * _Celui de Mathieu Saby (français) : **[Tutoriel OpenRefine](https://msaby.gitlab.io/tutoriel-openrefine/index.html)**_
