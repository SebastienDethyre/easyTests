# easyTests
> Un outil pour Robot Framework

Ce script permet sur une interface graphique, de choisir un test Robot Framework parmi ceux disponibles et de l'attribuer automatiquement un alias prédéfini (dans .bash_aliases ou bien .bashrc).
* Il faudra donc rajouter cet alias dans un de ces deux fichiers (et ne pas hésiter à créer .bash_aliases s'il n'existe pas pour y insérer l'alias, son     existence étant incluse/testée à chaque lecture de .bashrc).
```alias t='. venv omdt && ~/bin/easyTests/./currentTest'```
* Un alias pour lancer le script pourrait également s'avérer utile.
```alias test='~/bin/easyTests/testsDialog'```

Enfin, ce script devra être installé dans un répertoire ~/bin (à la racine dossier personnel de l'utilisateur), ou être modifié afin que les chemins d'accès soient respectés, en particulier dans le fichier testsDialog.

<br>

# easyTests
> A Robot Framework tool

This script allows, on a graphical interface, to choose a Robot Framework test among those available and to automatically assign it a predefined alias (in .bash_aliases or .bashrc).
* You will have to add this alias in one of these two files (and don't hesitate to create .bash_aliases if it doesn't exist to insert the alias, its     existence being included/tested at each reading of .bashrc).
```alias t='. venv omdt && ~/bin/easyTests/./currentTest'```
* An alias to launch the script could also be useful.
```alias test='~/bin/easyTests/testsDialog'```

Finally, this script will have to be installed in a ~/bin directory (at the root of the user's personal folder), or be modified so that the access paths are respected, especially in the testsDialog file.
