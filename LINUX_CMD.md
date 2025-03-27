# Commandes Linux
## Syntaxe generale
```bash
commande [options] <arguments>
```
lorsque vous entrerez la commande, les `[]` et `<>` ne sont pas à entrer, ils indiquent qu'il s'agit respectivement d'options et d'arguments.
lorsque que vous verrez `<? ?>` l'argument est optionnel

`#` sont des commentaire et non fon pas partie de la commande


## Commandes essentiels

### Manuel

la commande `man` suivie d'une commande, affiche le manuel de cette dernière 

### `sudo`

sudo = Super User DO

Cette commande permet d'exécuter une commande en tant que super utilisateur (admin) 

```bash
sudo <commande> 
```
### Navigation :

#### `cd`

cd = Change Directory

Cette commande permet de déplacer l'invite de commande dans le répertoire spécifié.

```bash
cd <chemin/avec/ce/format> 
```

#### `ls`

ls = List (Oui ya pas de moyen mnémotechnique pour celui là)

cette commande permet de lister les fichiers et dossiers dans le répertoire courant OU le répertoir specifié.

```bash
ls [-a] [-l] <?chemin/avec/ce/format?>
```
* `-a` : affiche les fichiers cachés
* `-l` : affiche les informations détaillées (appartenance, permissions, etc.)

#### Les chemins relatifs/absolus et symboles spéciaux

* `.` : le répertoire courant
* `..` : le répertoire parent
* `~` : le répertoire home
* `/` : la racine du disque dur

En utilisant les commandes déjà évoqués plus haut comme exemple :

```bash
cd . # ne fait rien
cd .. # remonte d'un répertoire
cd ~ # va dans le répertoire home
cd / # va à la racine du disque dur
```
et
```bash
ls / # liste les fichiers et dossiers à la racine du disque dur
ls ~ # liste les fichiers et dossiers dans le répertoire home
ls . # liste les fichiers et dossiers dans le répertoire courant
ls .. # liste les fichiers et dossiers dans le répertoire parent
```

Pour former un chemin relatif, on peut utiliser les symboles cité juste au dessus :

```bash 
../dossier_cible # chemin vers un dossier cible présent dans le répertoire parent
~/dossier_cible # chemin vers un dossier cible présent dans le répertoire home
/dossier_cible # chemin vers un dossier cible présent à la racine du disque dur
./dossier_cible # chemin vers un dossier cible présent dans le répertoire courant 
```
le dernier chemin est équivalent à `dossier_cible`

### Manipulation de fichiers et dossiers

#### `touch`

touch : vous "touchez" le fichier sans le modifier

Cette commande permet de créer un fichier vide du nom spécifié (et s'il existe, vous mettez à jour l'horodatage du fichier, mais on s'en fout) 

```bash
touch </chemin/vers/fichier/nom_du_fichier>
```

#### `mkdir`

mkdir = MaKe DIRectory

Cette commande permet de créer un dossier du nom spécifié

```bash
mkdir </chemin/vers/dossier/nom_du_dossier>
```

#### `rm`

rm = ReMove

Cette commande permet de supprimer un fichier ou un dossier

```bash
rm </chemin/vers/fichier/nom_du_fichier> # supprime un fichier
rm -r </chemin/vers/dossier/nom_du_dossier> # supprime un dossier
```
* `-r` : supprime récursivement : il applique RM à tous les fichiers à l'interieur du dossier et des dossiers à l'interieur du dossier puis supprimer le dossier cible (récusivement)

#### `mv`

mv = MoVe

Cette commande permet de déplacer ou renommer un fichier ou un dossier

```bash
mv </chemin/vers/fichier/nom_du_fichier_ou_dossier> </chemin/vers/nouveau_chemin/nouveau_nom_du_fichier_ou_dossier> # déplace/renomme un fichier
```

### `cat`

cat = conCATenate (lobjectif de départ de la fonction était de concatener des fichiers dans un flux de sortie...)

Cette commande permet d'afficher le contenu d'un fichier

```bash
cat </chemin/vers/fichier/nom_du_fichier>
```