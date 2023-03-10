
# Guide pour Quadcopter-Redux

Voici un guide pratique pour utiliser le simulateur de drone FPV Quadcopter-Redux sur GTA V.

## installation

- Il faut bien sûr avoir le jeu GTA V (peu importe la provenance steam, epic store ou autres...)
- ScriptHookV : Une librairie qui permet de s'interfacer avec GTA pour créer des mods.
- ScriptHookVDotNet : Une extension de la précédente librairie pour utiliser la technologie .NET
- Quadcopter-Redux : Le mod qui contient le simulateur.

Voici les liens vers les fichiers à installer (prenez les dernières versions pour chacun) :   
http://www.dev-c.com/gtav/scripthookv/   
https://github.com/crosire/scripthookvdotnet/releases   
https://www.gta5-mods.com/scripts/quadcopter-redux   

Il suffit de dézipper tout ces fichiers dans le répertoire d'installation du jeu GTA., et voilà.

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


## Première installation

Si vous installez pour la toute première fois GTA V et que vous lancer le jeu, il vous faudra compléter l'intro qui dure une quinzaine de minutes et qui vous plonge dans l'univers du jeu mais sur une petite map pour vous apprendre à jouer. Une fois passez cette intro vous aurez un accès total à énorme map de GTA et vous pourrez utiliser le simu sans aucune contrainte.

Mais rassurez vous vous n'êtes pas du tout obligé de passer par cette intro ni même de faire les missions de GTA si vous voulez utiliser exclusivement ce jeu en mode simulateur de drone FPV avec Quadcopter-Redux.

Le plus simple pour cela est de télécharger une sauvegarde qui complète le jeu à 100%.

Vous pouvez télécharger une sauvegarde depuis cette page :   
https://fr.gta5-mods.com/misc/100-game-save-for-1-7

Installer la sauvegarde sur votre pc à l'emplacement indiqué sur la page de description et relancer le jeu, vous pourrez ainsi directement utiliser Quadcopter-Redux sans passer par l'intro et vous serez propulsé à la fin du jeu avec toutes les missions déjà complétées.


## Configuration du controller

Il est hautement recommandé d'utiliser un vrai radio-controller de drone FPV pour piloter avec précision le drone dans le simulateur et retrouver les memes sensations et la précision qu'en réel. 

Si vous n'avez pas de radio, il est toutefois possible d'utiliser un gamepad type xbox360 pour s'initier ou tester ce mod mais ce n'est vraiment pas recommandé car vous risquez de prendre de mauvais reflexes avec ce genre de manette qui n'est pas assez précise ni adapter pour piloter un drone, notamment pour le stick des gaz dont le ressort est désactivé sur une vrai radio.

La plupart des radiocontroller devrait être automatiquement détectée.

Voici la liste des radio avec lesquelles j'ai pu testé le jeu :
- TBS tango 2
- DJI FPV controller 2 (celle de l'avata et du DJI FPV)
- BetaFPV LiteRadio 2 SE
- Radiomaster TX12

Pour la configuration, ouvrez le menu du drone.
Aller dans le sous-menu '*Gamepad*'.

Activer 'direct imput' si vous avez un radio controller sinon désactiver le pour utiliser un gamepad style xbox360.

Changer la valeurs des sticks afin d'affecter correctement le throttle, pitch, yaw et roll. VOus pouvez vous aider des jauges afin de détecter l'index du stick que vous etes en train de toucher.

Et faites la même chose si vous voulez binder des boutons, comme par exemple l'armement des moteurs, la touche unstuck, ou le bouton fire...

Vous pourrez aussi ajuster la précision des sticks depuis ce menu ou ajouter de la deadband.


## Configuration des rates

Le menu 'controller' vous permet de définir vos rates pour obtenir les vitesse de rotation désirées.
Les modes supportés sont Actual, Betaflight, Kiss et Raceflight.

Il est possible d'utiliser jusqu'à 3 slots pour enregistrer différentes configurations de rates.


## Configuration du drone

Aller dans le menu '*Physx*' pour ajuster le comportement de vol.

Vous pouvez définir plusieurs slots pour enregistrer différentes configuration pour représenter différents type de drone.

Pour configurer votre drone, vous pouvez procéder ainsi :

- Commencer par définir la taille des hélices (en pouces)
- Ensuite la masse du drone (en Kg)
- Régler ensuite la force de la poussée des moteurs en testant l'accélération et la vitesse de pointe pour essayer de retrouver les même sensation qu'avec votre drone en réel.
- Ajuster ensuite les autres facteurs tels que la gravité, le coef de trainée ou de résistance de l'air, ainsi que les damping linéaire au feeling pour ajuster vos sensations.


## Contenu additionnel

La communauté de modding autour de GTA est énorme et de nombreux mods ont été réalisés. Vous pouvez ainsi enrichir encore plus votre expérience avec ce simulateur en ajoutant des mods additionnels. 

Voici une petite liste de mods que je recommande :

(liste à venir...)
