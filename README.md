# APPRENDRE A UTILISER GIT
Bienvenue sur ce tutoriel qui vous permettra de comprendre comment utiliser Git (et GitHub. (un peu)) !
Ce repo contient les différentes niveau de compréhension de Git, de la base à l'expertise.

## 0. Introduction : Qu'est-ce que Git ?

Git est un logiciel de gestion de versions. C'est un outil qui permet de suivre l'évolution d'un projet. Il est particulièrement utilisé en informatique, mais vous pouvez en réalité l'utiliser pour toute sorte de projet. 

Quel est l'intérêt de Git exactement? Voyons ensemble rapidement comment un projet classique se déroule sans Git.

Lors d'un projet, il y a 2 écoles : 
1. Ceux qui ne veulent qu'un seul exemplaire du projet et qui écrasent le fichier à chaque modification.
2. Ceux qui veulent garder une trace de chaque modification et qui multiplient les copie du projet entre chaque modification.

Maintenant, mise en situation pour les 2 ecoles : 
1. Vous aviez eu une super idée il y a une semaine mais vous l'avez effacé au profit d'une autre idée qui se trouve être infructueuse (ou pire : une catastrophe)... Comment faites vous pour revenir en arrière? A moins d'avoir en tête l'EXACT contenu de votre fichier il y a une semaine, vous êtes coincé.
2. Vous avez 95 copies de votre projet. Dans cette situation, comment savez vous quelle version ajoute quoi au projet ? Si vous decidez de nommer vos version par fonctionnalités ajoutées... Comment savez vous l'ordre chronologique de ces dernière ? Et surtout : comment gerez vous votre espace disque encombré par ces copies ? Vous êtes egalement coincés et vous embourbé à mesure que le projet évolue

Et je ne parles ici que du travail en solo. Imaginez maintenant le travail en équipe... C'est le chaos assuré.

C'est là que git intervient. Git permet de n'avoir qu'une seule copie du projet ET garde en mémoire les évolutions successives nommés, daté et lié à son auteur, avec un titre permettant de savoir ce qui a été fait. Il permet également de travailler en équipe, gérant les conflits que peuvent entrainés des modifications faites par plusieurs personnes à des moments différents, et permettant de fusionner ces modifications dans un historique clair (si vous faites ça bien).

Voilà ce qu'est GIT. 

Fun fact 1 : git à été inventé par la même personne qui a créé Linux : Linus Torvald.
Fun fact 2 : personne ne sait, pas même Linus, ce que veut réellement dire "git", et on le sait car ...
Fun fact 3 : ... git est sur git (oui oui). Ce qui signifie que nous pouvons lire la toute première version de git... Grace à git.

## 1. Préparation

### 1.1 Avant propos

#### Les GUI (Graphical User Interface)

Pour cette formation, nous n'utiliserons pas de GUI (Graphical User Interface). Nous utiliserons uniquement des commandes. Git est certes très puissant, il est aussi très délicat et il est facile de "casser" un projet si on ne sait pas ce qu'il se passe en arrière plan et très compliqué de réparer les dégâts. Un dernier point en faveur des commandes : elles sont les mêmes sur toutes les plateformes (Windows, Mac, Linux) et vous permettront de vous adapter à n'importe quel environnement.

D'autre part, je déconseille l'utilisation spécifique de github desktop : étant directement relié à github, les comportements et fonctionnement rencontré dans ce logiciel ne sont pas forcément les mêmes que dans les commandes et peuvent être source de confusion très peu productive. Quoiqu'il en soit, n'utilisez AUCUN GUI avant d'avoir à minima terminer la formation [Basics](./Basics/formation.md). Une fois ceci fait, vous pouvez utiliser des GUI comme gitKraken (toute plateforme), git fork (mac) ou lazygit (c'est un TUI, mais c'est pareil) qui sont très bien fait et vous permettront de gagner du temps une fois que vous aurez les bases. Si, comme moi, vous codez sous VS Code, vous pouvez également utiliser l'extension git intégrée à l'éditeur.

Cependant, j'essaierais, à chaque fois que possible et fonction de la demande, de vous donner l'équivalent GUI de la commande que nous utilisons (dans un second temps).

#### Pre-requis : les commandes linux

Pour utiliser les commandes git, il faut connaitre les commandes Linux de base. En effet, que ce soit sous linux, windows ou mac, l'invite de commande (git bash) reconnait et utilise les commandes linux. Si vous ne les connaissez pas, j'ai laissé une petite fiche de rappel dans ce hub [ici](./LINUX_CMD.md).

### 1.2 Installation

Pour l'installation de git, on va se rendre directement sur le site officiel de [git](https://git-scm.com/downloads). Selectionner votre systeme d'exploitatation et suivez les instructions.

Une fois fait, verifions que git est bien installé. Cela va dépendre de votre système d'exploitation :

#### Windows

Ouvrez l'explorateur de fichier et faite un clique droit n'importe où (pas sur un fichier) et une option "ouvrir git bash ici" sera dans la liste des options   : vous avez bien installé git.

#### Mac

////////////////////////////////////////////////////////////////

#### Linux

Ouvrez un terminal et tapez `git --version`. Si vous avez une réponse, git est bien installé.

### 1.3 Creation d'un compte github

La formation est certes sur git, beaucoup de fonctionnalités importantes et utiles (nottament pour le travail en équipe) ne sont disponibles qu'avec un "service" tel que github, il est donc necessaire de créer un compte pour pleinement profiter de cette formation.

Je vous conseille également d'utiliser votre mail ensea, vous profiterez alors de certaines avantages, comme la possibilité d'avoir CoPilot, un assistant IA pour coder, gratuitement.

## 2. Contenue de chaque formations

### 2.1 Basics

* Notions concernant le fonctionnement de git
* Les oprations local de bases (init, add, commit, status, log)
* Les opérations distantes de bases (clone, push, pull, fetch)
* Corrections des erreurs locales avant commit

### 2.2 Intermediate

* Manipulation des commits
* Stash
* Les branches
* Corrections des erreurs après commits

### 2.3 Team work

* Merge, rebase, cherry-pick
* Gestion des conflits
* Les pull requests
* Corrections des erreurs après push

### 2.4 Expert : bonne pratique et astuces

### 2.5 Le self hosting

