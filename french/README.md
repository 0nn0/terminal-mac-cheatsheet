# Les commandes de base du Terminal sur Mac

_Les lettres sont en majuscules uniquement pour la lisibilité._  _La touche Verr Maj ne doit pas être activée_
## RACCOURCIS

| Touche/Commande | Description |
| ----------- | ----------- |
| Ctrl + A   | Va au début de la ligne. Marche aussi dans toutes les fenêtres de l'interface graphique |
| Ctrl + E   | Va à la fin de la ligne. Marche aussi dans toutes les fenêtres de l'interface graphique |
| Ctrl + Q   | Efface toute la ligne en cours |
| Ctrl + L   | Efface tout l'écran |
| Cmd + K    | Efface tout l'écran |
| Ctrl + U   | Coupe les caractères du curseur jusqu'au début de la ligne |
| Ctrl + K   | Coupe les caractères du curseur jusqu'à la fin de la ligne |
| Ctrl + W   | Coupe le mot précédent le curseur, l'espace étant le délimiteur |
| Ctrl + Y   | Copie ce qui a été coupé par la dernière commande couper |
| Ctrl + H   | Equivalent de la touche effacer |
| Ctrl + C   | Quitte le processus en cours |
| Ctrl + D   | Quitte le shell en cours lorsqu'aucun processus ne tourne, ou envoie EOF au processus en cours |
| Ctrl + Z   | Mets le processus en cours en arrière plan et rends la main sur le terminal. La commande fg restaure le processus |
| Ctrl + _   | Annule la dernière action typographique (effacer, insérer etc... des caractères) réalisée sur la ligne de commande en cours |
| Ctrl + T   | Inverse les 2 caractères qui précèdent le curseur |
| Ctrl + F   | Avance le curseur d'un caractère. Equivalent de la touche → |
| Ctrl + B   | Recule le curseur d'un caractère. Equivalent de la touche ← |
| Option + →  | Avance le curseur d'un mot |
| Option + ←  | Recule le curseur d'un mot |
| Esc + T  | Inverse les 2 mots qui précèdent le curseur |
| Tab  | Auto-complète les noms de dossiers et fichiers |

## COMMANDES PRINCIPALES

| Touche/Commande | Description |
| ----------- | ----------- |
| cd [répertoire] | Change de répertoire ex: `cd Documents` |
| cd |  Répertoire maison |
| cd ~ |  Répertoire maison |
| cd /  | Racine du disque dur |
| cd -  | Répertoire précédent |
| ls | Liste non détaillée des fichiers et dossiers du répertoire en cours |
| ls -l | Liste détaillée des fichiers et dossiers du répertoire en cours |
| ls -a | Liste incluant les fichiers cachés |
| ls -lh| Liste détaillée avec l'unité pour la taille des fichiers |
| ls -R | Liste le contenu de la totalité du répertoire en cours incluant les sous-dossiers et de manière récursive |
| sudo [commande] | Lance la commande avec les privilèges de sécurité du superuser (Super User DO) |
| open [fichier] | Ouvre le fichier (équivalent d'avoir double cliqué dessus dans l'interface graphique) |
| top | Affiche les processus actifs. Touche q pour quitter |
| nano [fichier] | Ouvre le fichier avec l'éditeur de texte nano |
| vim [fichier] | Ouvre le fichier avec l'éditeur de texte vim |
| clear |  Efface tout l'écran |
| reset |  Réinitialise le terminal |

## COMMANDES CHAINEES

| Touche/Commande | Description |
| ----------- | ----------- |
| [commande-a]; [commande-b] | Lance la commande A puis la commande B peu importe le succès ou non de la commande A |
| [commande-a] && [commande-b] | Lance la commande B si la commande A a réussi |
| [commande-a] \|\| [commande-b] | Lance la commande B si la commande A a échoué |
| [commande-a] & | Lance la commande A en arrière plan |


## COMMANDES EN FLUX DE REDIRECTION (PIPE)

| Touche/Commande | Description |
| ----------- | ----------- |
| [commande-a] \| [commande-b] | Lance la commande A qui envoie son résultat à la commande B. Par exemple : ls \| grep C affiche la liste des fichiers et dossiers qui contiennent la lettre C |


## HISTORIQUE DE COMMANDE

| Touche/Commande | Description |
| ----------- | ----------- |
| history N |  Affiche l'historique des N commandes tapées précédemment |
| Ctrl + R  | Recherche interactivement dans l'historique des commandes |
| ![valeur] |  Exécute la dernière commande tapée qui commence par ‘valeur’ |
| ![valeur]:p |  Affiche à l'écran la dernière commande tapée qui commence par ‘valeur’ |
| !! |  Exécute la dernière commande tapée |
| !!:p |  Affiche à l'écran la dernière commande tapée |

## GESTION DE FICHIERS

| Touche/Commande | Description |
| ----------- | ----------- |
| touch [fichier] | Crée un nouveau fichier |
| pwd | Affiche le chemin complet du répertoire en cours |
| . |  Répertoire en cours, par exemple `ls .` |
| .. | Répertoire parent c'est à dire qui contient le répertoire en cours, par exemple `ls ..` |
| ls -l .. | Liste détaillée du répertoire parent |
| cd ../../ | Monte de 2 niveaux |
| cat | Concatène à l'écran |
| rm [fichier] | Supprime un fichier, par exemple `rm data.tmp` |
| rm -i [fichier] | Supprime un fichier avec demande de confirmation |
| rm -r [rép] | Supprime le répertoire et son contenu |
| rm -f [fichier] | Force la suppression du fichier sans demande de confirmation |
| cp [fichier] [nouveauFichier] | Copie fichier vers nouveauFichier |
| cp [fichier] [répertoire] | Copie fichier dans répertoire |
| mv [fichier] [nouveauFichier] | Déplace/Renomme fichier vers nouveauFichier par exemple `mv fichier1.ad /tmp` |
| pbcopy < [fichier] | Copie le contenu du fichier dans le presse-papier. Equivalent d'avoir ouvert le fichier avec un éditeur puis d'avoir tout sélectionné puis Ctrl-C |
| pbpaste | Colle le contenu du presse-papier |
| pbpaste > [fichier] | Colle le contenu du presse-papier dans fichier, `pbpaste > paste-test.txt` |

## GESTION DES REPERTOIRES

| Touche/Commande | Description |
| ----------- | ----------- |
| mkdir [rép] | Crée un nouveau répertoire |
| mkdir -p [rép]/[rép] | Crée un répertoire et un sous-répertoire dans la foulée |
| rmdir [rép] | Supprime le répertoire (uniquement si le répertoire est vide) |
| rm -R [rép] | Supprime le répertoire et son contenu |
| less [fichier]| Affiche le contenu du fichier par morceau |
| [commande] > [fichier] | Envoie le résultat de la commande vers le fichier. Attention le contenu du fichier est écrasé |
| [commande] >> [fichier] | Ajoute le résultat de la commande au contenu existant du fichier |
| [commande] < [fichier] | Indique à la commande de lire le contenu du fichier |

## RECHERCHE

| Touche/Commande | Description |
| ----------- | ----------- |
| find [rép] -name [expression] | Recherche les fichiers dont le nom est conforme à l'expression dans le répertoire spécifié, par exemple `find /Utilisateurs -name "fichier.txt"` |
| grep [expression] [fichier] | Recherche toutes les lignes contenant l'expression, par exemple `grep "Tom" fichier.txt` |
| grep -r [expression] [rép] | Recherche récursivement dans tous les fichiers du répertoire spécifié toutes les lignes qui contiennent l'expression |
| grep -v [expression] [fichier] | Recherche toutes les lignes qui ne contiennent PAS l'expression |
| grep -i [expression] [fichier] | Recherche toutes les lignes qui contiennent l'expression sans tenir compte de la casse (majuscules/minuscules) |
| mdfind [expression] | Recherche Spotlight des fichiers dont l'expression est présent dans le nom, le contenu ou autre metadata |
| mdfind -onlyin [rép] -name [fichier] [expression] | Recherche Spotlight des fichiers dont le nom est spécifié et présent uniquement dans le répertoire spécifié |

## AIDE

| Touche/Commande | Description |
| ----------- | ----------- |
| [commande] -h | Affiche l'aide pour la commande |
| [commande] --help | Affiche l'aide pour la commande |
| info [commande] | Affiche l'aide pour la commande |
| man [commande] | Affiche le manuel d'utilisation de la commande |
| whatis [commande] | Décris ce que fait la commande en 1 seule ligne |
| apropos [expression] | Recherche les commandes dont la description contient l'expression |
