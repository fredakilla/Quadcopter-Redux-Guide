
# Guide pour Quadcopter-Redux

Voici un guide pratique pour utiliser le simulateur de drone FPV Quadcopter-Redux sur GTA V.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Quadcopter-Redux.jpg)


## Installation

- Il faut bien sûr avoir le jeu GTA V (peu importe la provenance steam, epic store ou autres...)
- ScriptHookV : Une librairie qui permet de s'interfacer avec GTA pour créer des mods.
- ScriptHookVDotNet : Une extension de la précédente librairie pour utiliser la technologie .NET
- Quadcopter-Redux : Le mod qui contient le simulateur.

La facon la plus facile d'installer tout cela est d'utiliser le package complet disponible sur cette page github dans la section releases, copier le contenu du zip dans le repertoire du jeu GTA et c'est fini:    
https://github.com/fredakilla/Quadcopter-Redux-Guide/releases

Si vous preferez installer manuellement chaque composant un par un:     
Voici les liens vers les fichiers à installer (prenez les dernières versions pour chacun) :   
http://www.dev-c.com/gtav/scripthookv/ ou sur ce mirroir https://www.gta5-mods.com/tools/script-hook-v   
https://github.com/crosire/scripthookvdotnet/releases   
https://www.gta5-mods.com/scripts/quadcopter-redux   

Il suffit de dézipper tout ces fichiers dans le répertoire d'installation du jeu GTA, et voilà.   

Assurez-vous que les fichiers sont au bon endroit.   
Pour l'archive zip ScriptHookV, c'est le contenu du dossier bin que vous devez placer à la racine du jeu.   
Voici par exemple ce que vous devriez normalement trouver à la racine du jeu GTA :   

```
E:\SteamLibrary\steamapps\common\Grand Theft Auto V\  

// ScriptHookV files :
dinput8.dll
NativeTrainer.asi
ScriptHookV.dll

// ScriptHookVDotNet files :
ScriptHookVDotNet.asi
ScriptHookVDotNet.ini
ScriptHookVDotNet2.dll
ScriptHookVDotNet2.xml
ScriptHookVDotNet3.dll
ScriptHookVDotNet3.xml

// Quadcopter-Redux files :
soft_oal.dll
scripts\Quadcopter\img\
scripts\Quadcopter\sounds\
scripts\Quadcopter\GTA5-Quadcopter.dll
scripts\Quadcopter\Changelog.txt
```

Astuce : Si vous appuyez sur F4 dans le jeu, vous devriez accéder au menu ScriptHookV, ce qui signifie que cette librairie est correctement installée.   

```diff
! Problème potentiel
Rien ne se passe lorsque l'on appuie sur 'G' ?
Si vous voyez le message "quadcopter-redux loaded" dans le coin supérieur gauche en entrant dans le jeu, tout va bien.
Mais sur certains systèmes, il y a un problème de droits d'accès car le dossier GTA peut être en lecture seule et ScriptHookV et
Quadcopter-Redux au démarrage essaient d'écrire leurs paramètres ou leurs fichiers journaux s'ils n'existent pas encore dans ce dossier.   
Essayez d'aller dans la sécurité du dossier GTA et donnez-lui un accès en écriture.

(La version Steam ne devrait pas etre concernée par ce problème mais j'ai eu un retour de ce probleme rencontré sur une versions du jeu provenant du Launcher de Rockstar Games. 
```

**Note importante** : L'utilisation de mod pour GTA V n'est pas officiellement reconnue ni encouragée par l'editeur Rockstar, toutefois cette pratique est toléré tant que cela reste pour du contenu en mode offline (donc pour l'histoire en mode solo). Si vous comptez jouer en mode online à GTA il est donc recommandé de supprimer les mods pour éviter de vous faire bannir du mode online et éviter les tricheries.

## Lancement du simulateur

Lancer GTA en mode histoire, le simu sera automatiquement détecté.
Une fois en jeu vous pouvez utiliser sur les touches suivantes :

- G : Pour basculer en mode drone/joueur
- H : Pour arrêter de voler et téléporter le joueur sur la position du drone
- F10 : pour ouvrir le menu du simulateur (quand vous êtes en mode drone)
- PageUp / PageDown : pour le tilt camera
- R : Pour reset le drone si vous êtes coincé
- C : pour changer la vue de la caméra
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
- Radiomaster TX12/TX16

Pour la configuration de la radiocommande, ouvrez le menu du drone.
Aller dans le sous-menu '*Controller*'.

Activer l'option 'direct input' si vous avez une radiocommande ou sinon désactiver la pour utiliser un gamepad style xbox360.

Changer la valeur des sticks afin d'assigner correctement le throttle, pitch, yaw et roll. Vous pouvez vous aider des jauges et des indications afin de détecter l'index des stick que vous etes en train de toucher.

Et faites la même chose si vous voulez binder des boutons, comme par exemple l'armement des moteurs, la touche unstuck, ou le bouton fire...

Vous pourrez aussi ajuster la précision des sticks depuis ce menu ou ajouter de la deadband.

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Controller.jpg)


## Configuration des rates

Le menu 'controller' vous permet de définir vos rates pour obtenir les vitesses de rotation désirées.
Les modes supportés sont Actual, Betaflight, Kiss et Raceflight.

Il est possible d'utiliser jusqu'à 3 slots pour enregistrer différentes configurations de rates.


![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/Rates2.jpg)

## Configuration du drone

Aller dans le menu '*Drone Presets*' pour configurer vos drones.

Vous pouvez créer autant de presets que vous desirez pour représenter différents types de drones.   
Les presets des drones sont enregistrés sous forme de fichiers .txt dans le répertoire scripts\Quadcopter\drone_presets.

Pour configurer votre drone, vous pouvez procéder ainsi :

![ScreenShot](https://github.com/fredakilla/Quadcopter-Redux-Guide/blob/main/img/DronePreset.jpg)


## Contenu additionnel

La communauté de modding autour de GTA est énorme et de nombreux mods ont été réalisés.   
Vous pouvez ainsi enrichir encore plus votre expérience avec ce simulateur en ajoutant des mods additionnels.   

Voici une petite liste de mods que je recommande :

Native Trainer (founi avec ScriptHookV) : vous permet tout un tas de chose (téléportaion, changer la méteo, l'heure, etc...)   
[Menyoo](https://www.gta5-mods.com/scripts/menyoo-pc-sp) : Un trainer multifonctions et un editeur de niveau créer vos propres parcours ou circuits de courses.   
[Forests of San Andreas](https://www.gta5-mods.com/maps/forests-of-san-andreas-revised) : Améliore grandement la densité et la varieté des arbres pour de belles ballades en forêts.   
[GTA V Remastered: Enhanced](https://www.gta5-mods.com/maps/gta-v-remastered-enhanced) : Améliore certaines parties de la carte en ajoutant plus de détails.   
[QuantV](https://www.gtainside.com/en/gta5/mods/119996-quantv-2-1-4) : Refonte et amélioration globale du rendu graphique de GTA, des effets de lumieres et des effets météorologiques.    
