# **Compléter les champs techniques**

Tous les standards de données de FuturoCité comportent un ensemble de champs « techniques » obligatoires. **La précision du code INS de la commune, du code d’identification des rues, ou encore des coordonnées géographiques d’un objet, permettent notamment d’éviter les imprécisions**. Par exemple, une rue peut porter le même nom dans deux communes, menant à des erreurs au moment de la situer sur une carte : coupler le nom de rue au code de cette dernière rend cela impossible. 

Remplir ces champs nécessite cependant d’aller chercher des données dans plusieurs sources. 


## **Le code INS**

Le code INS est l’identifiant unique de chaque commune belge. 

Il est facilement trouvable à partir du jeu de données « Codes des communes » de StatBel, téléchargeable depuis [cette page](https://statbel.fgov.be/fr/propos-de-statbel/methodologie/classifications/geographie)  

![alt_text](https://i.ibb.co/B3dFcnx/Capture-d-e-cran-2023-03-22-a-13-55-31.png)

Sur la même page du site de StatBel, il est également possible de télécharger le jeu « Codes des parties de communes (NIS6) », dans lequel se trouve le code INS d’une partie de commune. 

## **Retrouver le code le code rue BeSTAddress ("street_number")**

Ce code identifie chaque rue en Belgique. Il se trouve dans la base adresse nationale. 

Pour éviter de manipuler un fichier contenant près de deux millions de lignes, vous pouvez télécharger le jeu de données propre à votre commune sur [ici](https://nextcloud.datactivist.coop/s/rn5CMRWNGGaGWaS)<span style="text-decoration:underline;">. </span>

La fonction « rechercher » permet de retrouver facilement le nom de chaque rue. Il suffit alors de copier/coller le "street_id" de celle-ci dans le champ "street_number" du nouveau jeu de données.   

![alt_text](https://i.ibb.co/mJCNWTc/Capture-d-e-cran-2023-03-22-a-13-57-09.png)

## **Obtenir des coordonnées géographiques à partir d’une adresse (et vice-versa)**

Plusieurs outils en ligne permettent de retrouver facilement des coordonnées géographiques à partir d’une adresse. Par exemple : 

* Le site [https://www.coordonnees-gps.fr/carte/pays/BE](https://www.coordonnees-gps.fr/carte/pays/BE). On peut également obtenir des informations topographiques sur une adresse.
* Geoapity permet également de retrouver les coordonnées géographiques ([https://www.geoapify.com/tools/geocoding-online](https://www.geoapify.com/tools/geocoding-online)), ou au contraire de trouver une adresse à partir de coordonnées ([https://www.geoapify.com/tools/reverse-geocoding-online](https://www.geoapify.com/tools/reverse-geocoding-online))

## **Remplir le champ “geometry” (si applicable, par ex. standard des circuits touristiques) :**

Le champ "geometry" est une suite de coordonnées, générées à partir d’un fichier GPX (un format qui permet l’échange de coordonnées GPS). Concrètement, elle permet l’affichage de l’objet d’écrit (ici, un itinéraire de balade) sur une carte.   

La valeur bien formatée se présente ainsi : 

    {"coordinates": [[4.964690032, 50.4809399829], [4.9642300332, 50.4809099744],[...],[4.9602079968, 50.4856900041]],"type": "LineString"}

Pour obtenir cette valeur à partir d’un fichier GPX, il faut suivre **une procédure en 3 étapes** :  

 >  **1. Convertir le fichier GPX en GeoJSON, en utilisant** :  [https://samgoeta.shinyapps.io/gpxGeoJSONLinestring/](https://samgoeta.shinyapps.io/gpxGeoJSONLinestring/)  (il est possible de convertir plusieurs fichiers d’un coup). **Ne pas tenir compte du message d’erreur**. 


![alt_text](https://i.ibb.co/Ht2rNzG/Capture-d-e-cran-2023-03-22-a-13-58-33.png)

 >  **2. Importer ce fichier GeoJSON dans un portail OpenDataSoft (ODWB)**

(Nouveau jeu de donnée → Récupérer un fichier depuis mon ordinateur) 

![alt_text](https://i.ibb.co/p3WNrxh/Capture-d-e-cran-2023-03-22-a-13-59-40.png)

>   **3. Copier/coller la valeur du champ Geo Shape dans le champ "geometry" de son jeu de données**

![alt_text](https://i.ibb.co/2FjF85x/Capture-d-e-cran-2023-03-22-a-14-00-25.png)
 
![alt_text](https://i.ibb.co/z84XSd3/Capture-d-e-cran-2023-03-22-a-14-01-03.png)
