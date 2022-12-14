# easyTests
> Un outil pour Robot Framework

**Zenity est nécessaire à l'exécution de ce script.**
```sudo apt-get install zenity```

Ce script permet sur une interface graphique, de choisir un test Robot Framework parmi ceux disponibles et de l'attribuer automatiquement un alias prédéfini (dans .bash_aliases ou bien .bashrc).
* Il faudra donc rajouter cet alias dans un de ces deux fichiers (et ne pas hésiter à créer ~/.bash_aliases s'il n'existe pas pour y insérer l'alias, son     existence étant testée/incluse à chaque lecture de .bashrc).
```alias t='. venv omdt && ~/bin/easyTests/./currentTest'```
* Un alias pour lancer le script pourrait également s'avérer utile.
```alias te='~/bin/easyTests/testsDialog'```    

> _Penser à sourcer .bashrc ou .bash_aliases après chaque modification, pour qu'ils soient pris en compte avant le redémarrage du terminal._
```source ~/.bashrc && source ~/.bash_aliases```

Enfin, ce script devra être installé dans un répertoire ~/bin (à la racine dossier personnel de l'utilisateur), ou être modifié afin que les chemins d'accès soient respectés, en particulier dans le fichier testsDialog.

## Installation complète via le script *install*
> N.B. : L'installation va générer 2 alias (paramétrables dans le fichier .bash_aliases, lui-même créé s'il n'existait pas) :
> * te : pour ouvrir la boite de dialogue et choisir le test à effectuer
> * t : pour lancer le test choisi

A la fermeture du terminal, une confirmation sera demandée, car un processus est toujours actif. Fermez la fenêtre sans vous en soucier : il ne réapparaîtra pas (Ce processus provient de la commande *exec bash* lancée lors du script d'installation, pour remplacer le *source ~/.bash_aliases* non reconnue par un script).

Pensez à donner le droit d'éxecution au script pour le lancer :
```chmod 755 install && ./install```

De même pour le script de désinstallation :
```chmod 755 uninstall && ./uninstall```

<br>

<br>

# easyTests
> A Robot Framework tool

**Zenity is required to run this script**
```sudo apt-get install zenity```

This script allows, on a graphical interface, to choose a Robot Framework test among those available and to automatically assign it a predefined alias (in .bash_aliases or .bashrc).
* You will have to add this alias in one of these two files (and don't hesitate to create ~/.bash_aliases if it doesn't exist to insert the alias, its     existence being tested/included at each reading of .bashrc).
```alias t='. venv omdt && ~/bin/easyTests/./currentTest'```
* An alias to launch the script could also be useful.
```alias te='~/bin/easyTests/testsDialog'```    

> _Remember to source .bashrc or .bash_aliases after each modification, so that they are taken into account before restarting the terminal._
```source ~/.bashrc && source ~/.bash_aliases```    

Finally, this script will have to be installed in a ~/bin directory (at the root of the user's personal folder), or be modified so that the access paths are respected, especially in the testsDialog file.

## Complete install with script
> N.B. : The installation will generate 2 aliases (which can be set in the .bash_aliases file, which was created if it did not exist):
> * te : to open the dialog box and choose the test to run
> * t : to launch the chosen test

When the terminal is closed, a confirmation will be requested, as a process is still active. Close the window without worrying about it : it will not reappear (this process comes from the *exec bash* command launched during the installation script, to replace the *source ~/.bash_aliases* not recognized by a script).

Don't forget to allow the install script execution :
```chmod 755 install && ./install```

Same for the uninstall :
```chmod 755 uninstall && ./unistall```
