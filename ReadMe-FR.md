
# Guide pour Quadcopter-Redux

Voici un guide pratique pour utiliser le simulateur de drone FPV Quadcopter-Redux sur GTA V.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Quadcopter-Redux.jpg)


## Installation

- Il faut bien sûr avoir le jeu GTA V (peu importe la provenance steam, epic store ou autres...)
- ScriptHookV : Une librairie qui permet de s'interfacer avec GTA pour créer des mods.
- ScriptHookVDotNet : Une extension de la précédente librairie pour utiliser la technologie .NET
- Quadcopter-Redux : Le mod qui contient le simulateur.

Voici les liens vers les fichiers à installer (prenez les dernières versions pour chacun) :   
http://www.dev-c.com/gtav/scripthookv/   
https://github.com/crosire/scripthookvdotnet/releases   
https://www.gta5-mods.com/scripts/quadcopter-redux   

Il suffit de dézipper tout ces fichiers dans le répertoire d'installation du jeu GTA, et voilà.

**Note importante** : L'utilisation de mod pour GTA V n'est pas officiellement reconnue ni encouragée par l'editeur Rockstar, toutefois cette pratique est toléré tant que cela reste pour du contenu en mode offline (donc pour l'histoire en mode solo). Si vous comptez jouer en mode online à GTA il est donc recommandé de supprimer les mods pour éviter de vous faire bannir du mode online et éviter les tricheries.

## Lancement du simulateur

Lancer GTA en mode histoire, le simu sera automatiquement détecté.
Une fois en jeu vous pouvez utiliser sur les touches suivantes :

- G : Pour basculer en mode drone
- H : Pour arrêter de voler et retourner au personnage
- F9 : pour ouvrir le menu du simulateur (quand vous êtes en mode drone)
- PageUp / PageDown : pour le tilt camera
- R : Pour reset le drone si vous êtes coincé
- C : pour changer la caméra
- F : pour basculer entre le mode de vol acro ou angle
- X : Abandonner la mission
- B : Relancer la dernière mission


## Première installation

Si vous installez pour la toute première fois GTA V et que vous lancer le jeu, il vous faudra compléter l'intro qui dure une quinzaine de minutes et qui vous plonge dans l'univers du jeu mais sur une petite map pour vous apprendre à jouer. Une fois passée cette intro vous aurez un accès total à l'énorme map de GTA et vous pourrez utiliser le simu sans aucune contrainte.

Mais rassurez vous vous n'êtes pas du tout obligé de passer par cette intro ni même de faire les missions de GTA si vous voulez utiliser exclusivement ce jeu en mode simulateur de drone FPV avec Quadcopter-Redux.

Le plus simple pour cela est de télécharger une sauvegarde qui complète le jeu à 100%.

Vous pouvez télécharger une sauvegarde 100% depuis cette page :   
https://fr.gta5-mods.com/misc/100-game-save-for-1-7

Installer la sauvegarde sur votre pc à l'emplacement indiqué sur la page de description et relancer le jeu, vous pourrez ainsi directement utiliser Quadcopter-Redux sans passer par l'intro et vous serez propulsé à la fin du jeu avec toutes les missions déjà complétées.

## Utilisation du menu

Par defaut la touche pour afficher le menu est F9.    
Il est possible de changer cette touche en editant le fichier "Quadcopter.json" dans le dossier Quadcopter.   
Utiliser les fleches du clavier pour la navigation et backspace pour revenir en arriere. Appuyez sur F9 pour ouvrir/fermer le menu.   
Astuce : utilisez la touche shift pour changer plus rapidement les valeurs numériques.   


## Configuration de la radiocommande

Il est hautement recommandé d'utiliser une vrai radiocommande de drone FPV pour piloter avec précision le drone dans le simulateur et retrouver les mêmes sensations et la précision qu'en réel. 

Si vous n'avez pas de radiocommande, il est toutefois possible d'utiliser un gamepad type xbox360 pour s'initier ou tester ce simulateur mais ce n'est vraiment pas recommandé car vous risquez de prendre de mauvais reflexes avec ce genre de manette qui n'est pas assez précise ni adaptée pour piloter un drone, notamment pour le stick des gaz dont le ressort est désactivé sur une vrai radio.

La plupart des radiocommandes sont automatiquement détectée par le simulateur. (Du moment que Windows les detectent comme controller de jeu)

Voici la liste des radiocommandes avec lesquelles j'ai pu testé le jeu sans souci :
- TBS tango 2
- DJI FPV controller 2 (celle de l'avata et du DJI FPV)
- BetaFPV LiteRadio 2 SE
- Radiomaster TX12

Pour la configuration de la radiocommande, ouvrez le menu du drone.
Aller dans le sous-menu '*Gamepad*'.

Activer l'option 'direct input' si vous avez une radiocommande ou sinon désactiver la pour utiliser un gamepad style xbox360.

Changer la valeur des sticks afin d'assigner correctement le throttle, pitch, yaw et roll. Vous pouvez vous aider des jauges afin de détecter l'index des stick que vous etes en train de toucher.

Et faites la même chose si vous voulez binder des boutons, comme par exemple l'armement des moteurs, la touche unstuck, ou le bouton fire...

Vous pourrez aussi ajuster la précision des sticks depuis ce menu ou ajouter de la deadband.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Gamepad.jpg)


## Configuration des rates

Le menu 'controller' vous permet de définir vos rates pour obtenir les vitesses de rotation désirées.
Les modes supportés sont Actual, Betaflight, Kiss et Raceflight.

Il est possible d'utiliser jusqu'à 3 slots pour enregistrer différentes configurations de rates.


![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Rates.jpg)

## Configuration du drone

Aller dans le menu '*Physx*' pour ajuster le comportement de vol.

Vous pouvez définir plusieurs slots pour sauvegarder différentes configurations pour représenter différents type de drone.

Pour configurer votre drone, vous pouvez procéder ainsi :

- Commencer par définir la taille des hélices (en pouces)
- Ensuite la masse du drone (en Kg)
- Définisser la vitesse maximum du drone (en metres / seconde)
- Régler ensuite la force de la poussée des moteurs en testant l'accélération et la vitesse de pointe pour essayer de retrouver les même sensation qu'avec votre drone en réel.
- Ajuster ensuite les autres facteurs tels que la gravité, le coef de trainée ou de résistance de l'air, ainsi que les damping linéaire au feeling pour ajuster vos sensations.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Physx.jpg)

Notes sur la physique :   

La taille des hélices influe sur la force de poussée des moteurs ainsi que la portance du drone.  

Air density et drag coef permettent de simuler la densité de l'air et de créer une force de resistance qui s'oppose aux mouvements du drone. Plus cette force est élevé plus le drone sera freiné, il aura moins d'inertie, il "glisserra" moins. Evitez des valeurs trop élévés sinon vous aurez l'impression de voler dans un fluide très épais ou dense.   

Les 3 valeurs damping linear permettent d'une certaine facon de créér également une force de résistance opposée, comme un amortissement aux autre forces du drone comme la poussé ou la gravité. "Damping Linear C" influe faiblement, "Damping Linear V" modérément et "Damping Linear V2" agit tres fortement et est donc très sensible restez aux alentour des 0.005. Ces 3 facteurs agissant chacun de façon complémentaire sur la physique du drone. Mettez a 0 ces valeurs et le drone "glissera" dans l'air sans aucune resistance.   

Il est possible de mettre à 0 ces 3 valeurs du damping lineaaire et ne jouer qu'avec l'air density et le drag coef pour obtenir une force de resistance suffisante tout comme il est possible de mettre à 0 l'air density et le drag factor pour ne jouer qu'avec les damping lineaire pour obtenir cette force de resistance, ces 2 aspects étant assez similaires mais avec quelques différence subtiles. Et il est possible de jouer avec tous ces parametres ensemble pour ajuster encore plus finement la réaction du drone.  

La différence reside aussi dans le fait que le damping lineaire est géré en interne par le moteur physique de GTA alors que l'Air density et le drag coef sont des forces ajoutés et gérés par le mod Quadcopter par dessus la couche du moteur physique de GTA.   


## Contenu additionnel

La communauté de modding autour de GTA est énorme et de nombreux mods ont été réalisés.   
Vous pouvez ainsi enrichir encore plus votre expérience avec ce simulateur en ajoutant des mods additionnels.   

Voici une petite liste de mods que je recommande :

Native Trainer (founi avec ScriptHookV) : vous permet tout un tas de chose (téléportaion, changer la méteo, l'heure, etc...)   
[Map Editor](https://www.gta5-mods.com/scripts/map-editor) : Un editeur de carte créer vos propres parcours ou circuits de courses.   
[Forests of San Andreas](https://www.gta5-mods.com/maps/forests-of-san-andreas-revised) : Améliore grandement la densité et la varieté des arbres pour de belles ballades en forêts.   
[GTA V Remastered: Enhanced](https://www.gta5-mods.com/maps/gta-v-remastered-enhanced) : Améliore certaines parties de la carte en ajoutant plus de détails.   
[QuantV](https://www.gtainside.com/en/gta5/mods/119996-quantv-2-1-4) : Refonte et amélioration globale du rendu graphique de GTA, des effets de lumieres et des effets météorologiques.    
