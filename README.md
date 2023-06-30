# CosmicSail
###### _CosmicSail est l'un des 7 programmes de science participative de l'association Astrolabe Expeditions, qui consiste en la mesure des particules cosmiques (les muons) à bord de voiliers volontaires._
###### _Le kit de mesure "CosmicSail" est composé d'un détecteur de muons, conçu en collaboration avec les bénévoles de l'association My Human Kit (https://myhumankit.org/). La réalisation s'est basée sur le détecteur de muon open-source "CosmicWatch" (http://www.cosmicwatch.lns.mit.edu/)  sur lequel des développements ont été réalisés._
###

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />Ce(tte) œuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Licence Creative Commons Attribution -  Partage dans les Mêmes Conditions 4.0 International</a> 

##### Le kit de mesure CosmicSail permet de mesurer:

- Le nombre de détection de muons par unité de temps
- La pression atmosphérique
- Positions GPS des points de mesure, ainsi que la date et l'heure

##### Les liens du programme
- Site web du programme : https://www.astrolabe-expeditions.org/programme-de-sciences/CosmicSail/
- Wikifactory pour fabriquer le détecteur: (lien à venir)
- Github du code de l'instrument de mesure:  https://github.com/astrolabe-expeditions/CosmicSail


##### Ce github contient: 
- Les codes pour faire fonctionner le détecteur
- Les librairies
- Les étapes de configuration et d'installation du détecteur
- Le schéma électronique
- Le manuel d'utilisation du détecteur
- Le manuel technique du détecteur

### Configuration et installation du détecteur
Une fois le détecteur assemblé selon le mode opératoire décrit ici: (lien vers le wikifactory)
il faut configurer le détecteur.

#### 1-  Installer les librairies, les drivers
Toutes les librairies utiles se trouvent dans le dossier CS_librairies/ de ce github.


#### 2- Mettre à l'heure l'horloge UTC
L'horloge du détecteur doit être mise à l'heure universelle. Procédure:

- si le GPS est fonctionnel, la mise à jour de la date et de l'heure se fera automatiquement
- si le GPS n'est pas fonctionnel, l'initialisation de l'horloge se fait grâce au programme set_UTC_time.

#### 3- Installation du programme principal
Le programme principal se trouve dans le dossier Code ESP32/ de ce github.

#### 4- Installation de la carte SD
- la carte micro-SD doit être formatée en fat32 et doit contenir le fichier PARAM.txt (paramètres d'environnement à définir)
- Le logement de la carte se situe en face avant du détecteur.

Pour plus de détails, voir la notice d'utilisation du détecteur (Dossier /Docs/ de ce github).
