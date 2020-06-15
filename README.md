# Instructions_pour_découper_au_laser 

## Créer le fichier avec Inkscape
La découpe laser utilise un fichier svg pour déterminer les traits de coupe. Inkscape, un logiciel libre, permet de créer des fichiers appropriés.
La Speedy300 est configurée pour assigner des paramètres de découpe aux vecteurs contenus dans une image en fonction de leur couleure. Par défaut, les traits rouge pur (valeur rgb: 255,0,0) seront découpés alors que les formes noires sont gravées.

Pour modifier la couleur des traits, ouvrez l'outil de modification des traits et formes tel qu'indiqué sur l'image ci-dessous. 

#### Traits de découpe
Pour les traits qui doivent êtres découpés, enlever le remplissage ("fill") en cliquant sur le X, encore une fois comme sur l'image ci-dessous. Cette étape est importante, sans elle la découpe laser interprète mal le fichier et ajoute des traits non-désirés.

![Inkscape_remplissage](https://user-images.githubusercontent.com/65183668/84679866-227c0480-af32-11ea-8a83-6b82ab9388be.png)

Dans l'onglet des traits, mettre un trait uni ("flat color") en cliquant sur le carré à droite du X, et changer la valeur RGB pour 255, 0, 0 (en gardant l'opacité, A, à 255) comme sur l'image ci-dessous.

![Inkscape_trait](https://user-images.githubusercontent.com/65183668/84679901-2f005d00-af32-11ea-988a-df4180514c96.png)

#### Traits de gravure
Le format des traits de gravure est l'inverse: il faut ajouter un remplissage et enlever les traits. Les étapes sont essentiellement les mêmes, la seule différence est que le remplissage doit être noir (valeur RGB: 0,0,0) au lieu de rouge.

## Envoyer à Job Control
Pour envoyer le fichier à la découpe laser, il suffit de cliquer sur "imprimer" dans le menu "fichier" et selectionner la machine appelée Trotec. Job Control, le programme qui contrôle la découpe laser s'ouvrira alors (s'il ne l'est pas déjà) et votre fichier apparaitra dans le liste à droite de l'écran. 

## Préparer la machine
#### Faire le focus
Pour faire le focus, utiliser le petit appareil calibré placé dans la découpe laser. Il faut poser le rectangle doré sur le rebord de la tête de découpe comme indiqué sur l'image ci-dessous. 

Ensuite, faire monter la plaque par petits coups jusqu'à ce que l'outil de calibration tombe; la machine est alors bien calibrée. Si le matériel n'est pas de hauteure uniforme, trouver un point où l'épaisseure est moyenne pour faire le focus. Il faut aussi s'assurer qu'à la hauteur calibrée, aucun point du matériel ne peut toucher la tête.

#### Déterminer la position initiale
Il est important de bien choisir la position de la découpe sur la plaque. Cette opération est effectuée du logiciel Job Control, mais il est utile de s'aider en positionant manuellement la tête de la découpe à un endroit sur le matériel qui correspond au coin supérieur gauche de la découpe à faire. On peut ensuite venir fixer le fichier à découper dans Job Control sur la position de la tête.

## Paramètres de découpe

**acrylique extrudé noir 1/8''** :
* Coupe: P = 100; V = 0.9; F = 5000;

**plywood (merisier russe) 1/4''** :
* Coupe: P = 100; V = 0.3; F = 2000;
* Gravure: TBD

**Acrylique Cast Transparent 0.125 (1/8):**
* P = 100; V = 0.9; F = ????

**Acrylique (Épaisseur = 9mm)**

* Coupe V = 0.15; F = 2000
* Gravure = V = 40.00

**Acrylique (Épaisseur = 5mm)**

* Coupe V = 0.30; F = 5000; P=100;

**Papier Stacké (5 épaisseures de carton)**

* Coupe V = 1; P = 60; F = 49 999;

## Lancer la découpe
Une fois le fichier placer sur laq surface de travail, on doit s'assurer que les paramètres de découpe sont appropriés au matériel et au rendu désiré. Pour ce faire on peut utiliser les configurations par défaut associés au matériel en le choisissant de la liste en haut de l'écran. On peut aussi ajuster la vitesse et la puissance de découpe et de gravure au besoin avec les champs en haut de l'écran. Des tests peuvent êtres nécessaires pour déterminer l'effet d'une certaine configuration sur le matériel utilisé.

Une étape cruciale pour éviter le gaspillage de temps machine et de matériel et de vérifier que les dimensions de la découpe dans Job Control correspondent aux dimensions et à la position du matériel sur la plaque. Les unités indiqués en bordure de plaque permettent de faire cette vérification.

On peut s'assurer que notre fichier est bien compris pas la découpe laser en cliquant sur l'icône de prévisualisation (l'oeil) en haut de l'écrant, les traits de découpe apparaîtron alors à l'écran.

Une fois le focus, la position, les dimensions et les traits de coupe confirmés, on peut cliquer sur le bouton "play" pour partir la découpe. Il est obligatoire de surveiller CONSTAMMENT la machine durant son opération pour s'assurer que le matériel ne prend pas feu. Un extincteur à CO2 demeure à portée de main en cas d'incident. Le bouton "pause" sur la machine permet d'arrêter la machine au besoin, tout en conservant la capacitée de repartir le travail du point d'arrêt. En cas d'urgence, ouvrir la porte de la découpe peut être utilisé comme moyen d'arrêt immédiat de la machine.

Une fois le travail fini, laisser la porte de la machine fermée pour au moins une minute pour s'assurer que tous les gazs sont biens partis par le système de filtrage, faute de quoi des gazs potentiellement néfastes s'échapperont.

Avant de bouger quoi que ce soit, s'assurer que le matériel à bien été traversé par le laser. Faute de quoi, on peut relancer le travail pour finir la découpe.
