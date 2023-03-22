# **Produire un CSV en utilisant la virgule comme séparateur**

Les fichiers CSV (comma-separated values) permettent de voir vos données dans une variété d'applications : LibreOffice, Microsoft Excel, Numbers, Google sheets, etc.

Il s’agit d’un **format texte ouvert représentant des données tabulaires,** sous forme de valeurs séparées par des virgules (ou points virgules). 

<table>
  <tr>
   <td> 
<p>
<strong>Fichier au format .csv </strong>
<p>
(ce que la machine interprète) 
   </td>
   <td><strong>Représentation tabulaire </strong>
<p>
(ce que vous voyez) 
   </td>
  </tr>
  <tr>
   <td>Sexe,Prénom,Année de naissance
<p>
M,Mickey,1928
<p>
F,Minnie,1928
<p>
M,Donald,1934
   </td>
   <td>

<table>
  <tr>
   <td> Sexe
   </td>
   <td>Prénom
   </td>
   <td>Année de naissance
   </td>
  </tr>
  <tr>
   <td>M
   </td>
   <td>Mickey
   </td>
   <td>1928
   </td>
  </tr>
  <tr>
   <td>F
   </td>
   <td>Minnie
   </td>
   <td>1928
   </td>
  </tr>
  <tr>
   <td>M
   </td>
   <td>Donald
   </td>
   <td>1934
   </td>
  </tr>
</table>

   </td>
  </tr>
</table>


Les colonnes peuvent être séparées par des points-virgules ou des virgules. Si les deux possibilités existent **il est fortement recommandé d’utiliser la virgule comme séparateur** : il est le plus utilisé à l’international (malgré une persistance du point-virgule sur les portails francophones). De nombreuses applications, notamment de contrôle de la qualité des données, ne permettent donc pas de traiter des fichiers utilisant le point-virgule. Car il ne propose pas toujours l’utilisation de la virgule, ce qui entrave donc l’utilisation d’application, Excel est l’outil le moins recommandé. Nous vous suggérons plutôt d’utiliser LibreOffice, ou éventuellement GoogleSheet.

En tant que producteur de données, il faut donc vous assurer de travailler sur (puis de publier) un jeu de données utilisant la bonne norme. 

## **<span style="text-decoration:underline;">Sur LibreOffice</span>**

(LibreOffice est le logiciel minimisant les erreurs dans un CSV) 

### **1. Enregistrer un fichier au format CSV  (depuis LibreOffice)**

Depuis votre logiciel, il suffit d’ « enregistrer sous » au format « text CSV (.csv) » 

![image](https://i.ibb.co/JdrjgkR/Capture-d-e-cran-2023-03-22-a-11-51-00.png)

Puis de valider caractéristiques suivantes : 

* Encodage (_character set_) : Unicode UTF-8 (ce codage est le plus usuel car compatible avec la norme ASCII) 
* Séparateur de champ (_field delimiter_) : virgule (,)
* Identificateur de texte (_string delimiter_) : guillemets (“)

![alt_text](https://i.ibb.co/JdrjgkR/Capture-d-e-cran-2023-03-22-a-11-51-00.png)

Votre fichier est désormais un csv utilisant la virgule comme séparateur : l’idéal pour le partage de données ! 

### **2. Ouvrir un fichier CSV**

Lorsque vous ouvrez un fichier CSV dans LibreOffice, le logiciel vous propose de valider un ensemble de paramètres. 

Comme pour enregistrer un nouveau fichier CSV, assurer vous de valider : 

* Encodage (_character set_) : Unicode UTF-8
* Séparateur de champ (_separated by_) : virgule (,)
* Identificateur de texte (_string delimiter_) : guillemets (“)

![alt_text](https://i.ibb.co/zZyGL7K/Capture-d-e-cran-2023-03-22-a-11-59-02.png)

## **<span style="text-decoration:underline;">Depuis Excel</span>**

### **Convertir un fichier (passer du séparateur point-virgule au séparateur virgule)**

Si vous utilisez Excel plutôt que LibreOffice, il arrive que les données apparaissent sur une seule colonne. Pas de panique, en quelques clics vous pouvez remettre votre jeu de données en ordre et vous assurer qu’il est enregistré au bon format.   

**La situation de départ : toutes les valeurs d’une ligne sont dans la même colonne (la virgule n’est donc pas considérée comme le séparateur)**

![alt_text](https://i.ibb.co/PWsB1Mx/Capture-d-e-cran-2023-03-22-a-11-59-52.png)

**La solution :**

> **1. Je sélectionne la colonne A**

![alt_text](https://i.ibb.co/Qn88YLB/Capture-d-e-cran-2023-03-22-a-12-00-32.png)

> **2. Dans l’onglet « Données », je clique sur l’icône « Convertir »** 

![alt_text](https://i.ibb.co/6wtt8Ym/Capture-d-e-cran-2023-03-22-a-12-01-20.png)

> **3. Je m’assure que mes données sont de type « Délimité » et je clique sur « Suivant »**

![alt_text](https://i.ibb.co/gWYp37L/Capture-d-e-cran-2023-03-22-a-12-01-58.png)

> **4. Je choisis comme séparateur/délimiteur « Virgule », et je m’assure que l’identificateur de texte est le guillemet. Je clique sur « Fin ».**

![alt_text](https://i.ibb.co/B2WRn83/Capture-d-e-cran-2023-03-22-a-12-02-39.png)

> **5. Mes données sont réorganisées !**

![alt_text](https://i.ibb.co/1nb4kB9/Capture-d-e-cran-2023-03-22-a-12-03-18.png)

> **6. Je n’ai plus qu’à enregistrer le fichier au format « CSV UTF-8 ».** 

![alt_text](https://i.ibb.co/vPPjZnN/Capture-d-e-cran-2023-03-22-a-12-04-09.png)

_→ Dans le (rare) cas où votre version d’Excel ne permettra pas l’enregistrement du fichier sous la bonne norme, il faudra basculer vers un autre outil (si vous ne pouvez pas télécharger LibreOffice, GoogleSheet vous permet de travailler en ligne)._
