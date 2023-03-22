# **Documenter son jeu de données**

Avant de publier son jeu de données sur un portail open data, il est essentiel de le documenter. 

La « bonne » documentation ne s’arrête pas aux métadonnées essentielles (nom du producteur de données, date de mise à jour, etc.). 

**Les compléter par des informations sur la composition du jeu de données (explicitation de chaque champ), sur les raisons et les conditions de collecte des données, ou encore sur les éventuels traitements dont elles ont fait l’objet permet au réutilisateur de comprendre ce que contient le jeu de données et ses éventuels biais.**

Une documentation complète favorise par ailleurs la découvrabilité des données, c’est-à-dire rend plus aisé pour le réutilisateur de trouver le jeu de données recherché.  



_**Nous recommandons deux choses, en plus de la complétion des métadonnées de base :**_

* **La description des champs du jeu de données**
* **L’utilisation de la méthode [Datasheets for Datasets](https://arxiv.org/pdf/1803.09010.pdf)** (dans la mesure des informations à disposition du producteur de données) 

Constatant le manque d’exhaustivité et d’harmonisation dans la documentation des jeux de données servant à l'entraînement des modèles d’intelligence artificielles, les autrices de l’article _Datasheets for Datasets_[1] proposent aux producteurs de données de renseigner une « fiche technique » comportant 7 parties : 
* Motivations pour la création du jeu de données
* Composition du jeu de données
* Processus de collecte des données
* Pré-traitement des données
* Diffusion du jeu de données
* Maintenance du jeu de données
* Considérations légales et éthiques

[1]Gebru, T., Morgenstern, J., Vecchione, B., Vaughan, J. W., Wallach, H., Iii, H. D., & Crawford, K. (2021). Datasheets for datasets. Communications of the ACM, 64(12), 86-92.

![alt_text](https://i.ibb.co/gZkmbtT/Capture-d-e-cran-2023-03-22-a-14-08-29.png)


**[Une traduction en français a été réalisée par Samuel Goëta](https://teamopendata.org/t/traduction-et-adaptation-du-modele-de-description-des-donnees-datasheet-for-datasets/1400) :**

**Motivations pour la création du jeu de données**

* Pourquoi le jeu de données a-t-il été initialement créé ?
* Quelles ont été les utilisations non prévues du jeu de données ?
* Pour quelles autres tâches le jeu de données pourrait-il être utilisé ?
* Quelles sont les utilisations trompeuses du jeu de données ?
* Qui a financé ou soutenu la création du jeu de données ?

**Composition du jeu de données**

* Que contient le jeu de données principalement ? Les enregistrements représentent-ils principalement des documents, des personnes, des territoires, des entreprises… ?
* Dispose-t-on d’un schéma décrivant les variables du jeu de données ?
* Que contient chaque champ du jeu de données ?
* Est-ce que le contenu du jeu de données dépend de ressources externes (ex. identifiant SIRET ou lien vers le document…) ? De quelles garanties dispose-t-on concernant la pérennité de ces ressources ?

**Processus de collecte des données**

* Comment les données ont été collectées (avec des capteurs, manuellement, par des outils informatiques…) ?
* Qui a assuré le processus de collecte de données (des agents, des bénévoles, des étudiants…) ?
* Quelle a été la période de collecte des données ?
* Les données ont-elles été collectées directement ou inférées à partir d’autres données ?
* Les données ont-elles été collectées sur un échantillon ? Quelle est la population complète ? Selon quelles méthodes ?
* Quelles sont les erreurs connues, les limites, les sources de bruit ou de redondances associées à ces données ?

**Pré-traitement des données**

* Comment les données ont-elles nettoyées ou préparées ?
* Les données « brutes » ont-elles été conservées ? Sont-elles diffusées ?
* L’outil de pré-traitement des données est-il disponible ?

**Diffusion du jeu de données**

* Les données sont-elles diffusées en ligne ? Selon quelles modalités (sur un portail open data, un site web, une API…) ?
* Si non, les données sont-elles diffusées au cas par cas ? à la demande ?
* Selon quelle licence les données sont-elles diffusées ?
* Des redevances ou des restrictions sont-elles appliquées dans l’accès aux données ?

**Maintenance du jeu de données**

* Qui assure la maintenance du jeu de données ? Comment peut-on contacter cette personne ? Quel est le service responsable du jeu de données ?
* Est-ce que les rôles sont distincts entre la production des données, leur éditorialisation et leur diffusion ?
* Le jeu de données sera-t-il mis à jour ? Si oui, à quelle fréquence ?
* Si les données deviennent obsolètes, comment cette information sera-t-elle communiquée ?
* Est-il possible de contribuer à l’amélioration des données ? Selon quelles modalités ?

**Considérations légales et éthiques**

* Si le jeu de données concerne des individus, ont-ils exprimé leur consentement de manière claire ?
* Les individus ont-ils été informés sur la finalité du traitement de données ?
* Le jeu de données peut-il exposer de manière directe ou indirecte des individus ?
* Ces données sont-elles conformes au RGPD ?
* Les données peuvent-elles avantager ou désavantager des groupes sociaux ?
* Le jeu de données contient-il des informations pouvant être considérées comme inappropriées ou offensantes ?
