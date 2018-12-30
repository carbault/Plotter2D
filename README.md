#PLOTTER 2D:


**Prérequis à installer:**
* Arduino, Processing (voir prérequis.txt)
* Librairie Polagraph (voir prérequis.txt)
* Librairie Servo pour Arduino (installer depsuis l'arduino IDE)
* Fusion360 & Cura pour la modélisation et l'impression 3D


**Notes sur les fichiers dans ce repo:**
* Le dossier Polargraph est à placer dans le dossier Sketchbook d'Arduino. Les fichiers sont déjà modifiés en fonction des pins de notre board, etc.
* Le dossier Settings Polargraph Controller contient le fichier paramètres à charger dans Polargraph Controller.


**Lancer le plotter (sous WINDOWS):**

* Lancer Arduino en tant qu'administrateur
* Ouvrir Polargraph Server depuis le Sketchbook
* Sélectionner la board, compiler et uploader si besoin
* Lancer Processing en tant qu'administrateur
* Ouvrir Polargraph Controller depuis le Sketchbook
* Lancer Polargraph Controller

*Setup de Polargraph Controller*
* Cliquer sur l'onglet Setup
* Cliquer sur load config et charger le fichier .txt contenu dans le dossier "Settings Polargraph Controller du repo". Ce fichier contient des réglages en fonction des pièces du plotter (largeur de la ceinture, etc.)
* Cliquer sur *Serial Port* tout en bas de la fenêtre et choisir le port de la board
* Cliquer sur *upload machine specs*
* Cliquer sur *Command queue* en haut à droite de la fenêtre (aussi utilisable pour mettre en pause le dessin ou autre commande)
* Ajuster les dimensions en fonction de la taille de la surface sur laquelle dessiner et des positions des moteurs. (page height, page width, machine height, machine width). Par défaut il s'agit d'une feuille A4.
* Charger le dessin avec load vector. (format .svg)
* Régler sa taille et le positionnner. A noter que les marqueurs des bords de la feuille sont visible dans l'onglet input mais pas l'onglet Settings.
* Dans l'onglet Input, cliquer sur Set Home et déplacer (manuellement) le socle du stylo au point correspondant.
* Lancer le dessin (*draw vectors*)
