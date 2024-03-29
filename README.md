Ce dépôt documente l'intérêt de standardiser les données ouvertes. Il s'appuie sur les exemples des standards de données prioritaires identifiés et produits par FuturoCité dans le cadre de [groupes de travail](https://www.futurocite.be/activites/groupe-de-travail-open-data). Ces derniers réunissent régulièrement des collectivités wallonnes engagées dans des démarches d'open data. 
Cinq premiers standards concernent : les circuits touristiques, les emplacements PMR, les équipements collectifs, les stationnements vélos, les travaux de voiries. 

# Pourquoi standardiser des données ouvertes ? 


## Favoriser la découvrabilité des données 

Il existe un besoin d'harmonisation de la publication en open data de données essentielles produites par les administrations publiques wallonnes. En octobre 2022, plus de 660 jeux de données sont publiés sur le portail [Open Data Wallonie Bruxelles (ODWB)](https://www.odwb.be/explore/?sort=modified), qui sont très hétérogènes.

En fonction de leur patrimoine, de leurs pratiques et de leurs compétences, les territoires publient en effet des données très diverses. Ils ne publient pas les mêmes jeux de données, et lorsque c'est le cas ils ne les nomment pas toujours de la même manière. 

Par exemple, sur le sujet des aménagements cyclables de nombreuses terminologies sont possibles. Il faudra alternativement chercher « aménagements cyclables » ou « pistes cyclables » et on retrouvera rarement le mot clef  « vélo » dans les descriptions des jeux de données alors que le terme vient spontanément sur le sujet.

La première étape de la standardisation des données consiste dont à s'accorder sur un vocabulaire commun, afin de favoriser la découvrabilité des données, c'est-à-dire permettre aux utilisateurs de les trouver facilement.   


## Faciliter leur interopérabilité 
À cet enjeu de découvrabilité s’ajoute un défi lié à la normalisation des données ouvertes. D’un producteur à l'autre, les fichiers ne contiennent pas nécessairement les mêmes champs ou ne donnent pas le même niveau de détail. Les valeurs dans les champs eux-mêmes ne sont pas normalisées. 

La diversité des modèles concernant les jeux de données prioritaires identifiés dans le cadre du groupe de travail a confirmé ce besoin d'harmonisation. Les emplacements PMR ne sont par exemple pas décrits de la même manière à Liège, Namur, Mons et La Louvière. [À Namur](https://data.namur.be/explore/dataset/namur-parking-emplacements-surfaciques/information/?disjunctive.type_parking&disjunctive.zone&disjunctive.localite&disjunctive.rue_nom&disjunctive.code_rue&sort=-type_parking), l'accessibilité PMR est précisée dans un jeu de donnée "généraliste" portant sur le stationnement, alors qu'elle fait l'objet d'un jeu de données distinct [à Liège](https://opendata.liege.be/explore/dataset/stationnement-pmr/information/). Par ailleurs, les champs relatifs à l'adresse ne sont pas nommés de la même manière et ne contiennent pas tout à fait les mêmes données. 

Concrètement, cela rend très compliqué l'agrégation des données au niveau du territoire wallon, et donc entrave un état des lieux de l'accessibilité et la développement d'applications qui fonctionneraient au-delà du niveau urbain. En d'autres termes, les données sont disponibles dans les quatre villes citées, mais pas intéroprables. 

## En bref : standardiser pour accroître l'impact de l'open data 

<b>Ces enjeux de découvrabilité et de normalisation des données limitent l’impact de l’open data. Sans harmonisation des pratiques, il est difficile de développer des services ou des usages qui dépassent un seul territoire.</b>

Si la standardisation est un levier important  de l’open data, les données non standardisées ne sont pour autant pas sans valeur, loin de là ! La publication de jeux de données dans un format ouvert (CSV plutôt que PDF par exemple) constitue déjà une étape importante dans l’application du principe de transparence, et une donnée peut être réutilisable sans être standardisée. Si de nombreux standards sont déjà disponibles ou en cours de conception, il n'en existe d'ailleurs pas encore pour tous les jeux de données. 
La standardisation de données déjà publiées peut tout de même constituer une étape supplémentaire dans la stratégie open data d’une collectivité. Rendre conforme un jeu de données à un schéma est en effet possible post-publication.    

# Standardiser des "données prioritaires"   

Constatant la production de jeux de données disparates à l'échelle de la fédération Wallonie-Bruxelles, FuturoCité a réuni, dans le cadre d'un groupe de travail sollicité depuis mai 2021, une vingtaine de collectivités. La concertation de celles-ci a permis 
* d'identifier collectivitement des jeux de données jugés prioritaires  
* de s'accorder sur des spécifications des modèles de données. 
La standardisation de ces données prioritaires est en effet essentielles pour s'assurer de leur publication homogène et de faciliter leur exploitation (notamment leur agrégation) par les réutilisateurs. Elle facilitent l'exploitation des données publiées par les réutilisateurs (agrégation, consolidation et traitements automatiques).

## Six schémas de données à disposition 

La standardisation des données ouvertes s’articule autour de schémas. Ces derniers sont des standards lisibles par des machines, des conventions qui décrivent les champs et les valeurs admises dans un jeu de données conforme à ses préconisations. C’est donc en s’y conformant que nous produisons des jeux de données standardisés. Compréhensibles par les machines, les schémas sont réexploités dans des formulaires et des interfaces à destination des humains. 

Les membres du groupe de travail ont défini des schémas de données qui décrivent le format des fichiers, les différents champs, les valeurs possibles… Ils se sont appuyés sur un état des lieux du patrimoine de données des collectivités wallones et sur une étude des modèles utilisés par des collectivités déjà productrices de ces données, en prenant en compte les retours faits par les réutilisateurs.

Cinq schémas sont actuellement disponibles : 
* [les circuits touristiques](http://www.futurocite.be/schemas-des-circuits-touristiques/)
* [les emplacements PMR](http://www.futurocite.be/schema-des-emplacements-pmr/)
* [les équipements collectifs](http://www.futurocite.be/schema-des-equipements-collectifs/) 
* [les stationnements vélos](https://www.futurocite.be/schema-des-stationnements-velos/)
* [les travaux de voiries](http://www.futurocite.be/schema-des-travaux-de-voirie/) 
* [les marchés](http://www.futurocite.be/schema-des-marches/) 


# La standardisation concrètement 

La standardisation demande un travail important de la part des producteurs de données publiques ouvertes. Reprendre des données selon les spécifications d’un standard, ou produire de nouveaux de jeux de données demande en effet du travail, souvent peu visible.  

Deux situations sont possibles : 
* Le producteur veut standardiser des données déjà existantes
* Le producteur souhaite produire de nouvelles données en se conformant à un standard

Dans les deux cas (précisés [ici](https://github.com/FuturoCite/Documentation-standardisation/tree/main/Fiches%20pratiques)), les producteurs peuvent utiliser des outils de validation afin de s'assurer de la conformité de leur jeu de données à un standard, en s'appuyant sur l'outil [validata](https://validata.fr/) par exemple

Quel que soit le cas de figure, le producteur doit également respecter des règles de formatage. Si le format de publication est le CSV (Comma Separated Values, valeurs séparées par des virgules), les règles sont les suivantes :
* l’encodage des caractères est UTF-8,
* le séparateur des colonnes est la virgule,
* le séparateur des nombres décimaux est le point,
* le séparateur de valeurs multiples dans un champ est le point-virgule,
* si un champ contient une virgule, il doit être entouré de guillemets doubles,
* chaque ligne doit avoir le même nombre de champs,
* le type MIME ou Content-Type est text/csv.
