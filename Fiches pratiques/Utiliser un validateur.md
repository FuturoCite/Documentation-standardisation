# **Utiliser un validateur**

Un validateur vous permet de vous assurer de la correspondance de votre jeu de données à un standard (les champs et les valeurs contraintes sont respectées) et pointera les éventuelles erreurs. 

Nous recommandons l’usage de Validata https://validata.fr, plateforme développée par l’association française OpenDataFrance. 

## **La marche à suivre :**

**1. Dans « Schéma à la carte », en bas de la page, je mets le lien vers le standard FuturoCité et clique sur « Valider un fichier ».**

![alt_text](https://i.ibb.co/y5JpyQ3/Capture-d-e-cran-2023-03-22-a-12-20-14.png)

Voici les liens pour rappel, vous n’avez qu’à les copier-coller : 
* Equipements collectifs : [https://raw.githubusercontent.com/FuturoCite/standard-equipements-collectifs/main/schema.json](https://raw.githubusercontent.com/FuturoCite/standard-equipements-collectifs/main/schema.json) 
* Emplacements PMR : [https://raw.githubusercontent.com/FuturoCite/standard-emplacements-PMR/main/schema.json](https://raw.githubusercontent.com/FuturoCite/standard-emplacements-PMR/main/schema.json) 
* Circuits touristiques : [https://raw.githubusercontent.com/FuturoCite/standard-circuits-touristiques/main/schema.json](https://raw.githubusercontent.com/FuturoCite/standard-circuits-touristiques/main/schema.json) 
* Travaux de voirie : [https://raw.githubusercontent.com/FuturoCite/standard-travaux-voiries/main/schema.json](https://raw.githubusercontent.com/FuturoCite/standard-travaux-voiries/main/schema.json) 
* Stationnements vélo : [https://raw.githubusercontent.com/FuturoCite/standard-stationnements-velos/main/schema.json](https://raw.githubusercontent.com/FuturoCite/standard-stationnements-velos/main/schema.json) 

(Pour information, ces liens sont des uri. Elles se trouvent dans les fichiers tableschema, auxquels vous pouvez accéder depuis le site de FuturoCité [http://www.futurocite.be/standardiser-les-donnees-ouvertes/](http://www.futurocite.be/standardiser-les-donnees-ouvertes/) 

![alt_text](https://i.ibb.co/CWkHJ4p/Capture-d-e-cran-2023-03-22-a-12-21-03.png)

![alt_text](https://i.ibb.co/TYBVsYQ/Capture-d-e-cran-2023-03-22-a-12-21-50.png)

**2. J’importe mon fichier CSV (depuis mon ordinateur ou depuis une URL) et je clique sur « Valider le fichier »**

![alt_text](https://i.ibb.co/kcDSPDC/Capture-d-e-cran-2023-03-22-a-12-22-49.png)

### **→ Si mon fichier est validé** 
Félicitations ! Je m’assure que mon fichier est correctement nommé et je peux le publier sur ODWB (sans oublier de le documenter !) 

![alt_text](https://i.ibb.co/PNh4Bm4/Capture-d-e-cran-2023-03-22-a-12-24-01.png)

### **→ Si mon fichier est invalide** 
Pas de panique.   

Une liste de recommandations est générée en bas de la page. 

![alt_text](https://i.ibb.co/5Mcm2Hv/Capture-d-e-cran-2023-03-22-a-12-24-44.png)

En dessous, les valeurs posant problème apparaissent en rouge.  

![alt_text](https://i.ibb.co/6yDyHTd/Capture-d-e-cran-2023-03-22-a-12-25-19.png)


**Quatre principaux types d’erreurs :**

**1. Il manque des champs/colonnes :**

→ Il faut les ajouter, même si leur remplissage n’est pas obligatoire, et les laisser vides si on n’est pas en mesure de les renseigner. 

Par exemple : dans les standards conçus par FuturoCité vous pouvez laisser vide le “Code rue national”, mais une colonne doit tout de même figurer dans votre jeu de données. 

**2. Des valeurs obligatoires sont manquantes**

→ Dans la mesure du possible, je complète le jeu de données à partir de sources externes (voir la fiche “Compléter les champs techniques” pour quelques exemples). 

Si la donnée est introuvable/inexistante et que mon jeu de données est par ailleurs conforme au schéma, je le publie.  

**3. Les valeurs sont erronées :**

→ S’assurer d’avoir bien suivi les spécifications du standard, concernant notamment : 

* Le format des dates (année-mois-jour) et des coordonnées   
* Les valeurs contraintes : elles doivent être bien orthographiées (y compris accents et majuscules), sans espace supplémentaire ("vélo" ≠ "velo ") 

**4. Il y a des champs en trop :**

→ En fonction de mon patrimoine de données, j’ai intégré des champs supplémentaires. Le non-respect du standard est donc volontaire. Mais afin de faciliter l’agrégation de plusieurs jeux de données par un réutilisateur il est recommandé de publier deux jeux de données : 
* Un jeu de données standardisé, s’en tenant aux champs du standard (il est possible de supprimer des colonnes d’un jeu de données enrichi grâce à un processeur OpenDataSoft)
* Un jeu de données enrichi, intégrant des champs supplémentaires 

Cette double publication assure de ne pas faire reposer de travail supplémentaire sur le réutilisateur : il n’a pas à retravailler le jeu de données afin de supprimer les champs en trop en vue de les agréger avec d’autres.  
