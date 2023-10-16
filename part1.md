## Création du projet
Avant d’utiliser GitLab nous allons dans un premier temps créer un site Internet sur votre ordinateur. <br>
Pour cela, vous pouvez vous inspirer du répertoire suivant : https://github.com/nicolas-sanch/creer-site-statique-3iSystem

### Les logs
Vérifier que votre projet est bien commité, avec la commande `git status`. Vous pouvez également vérifier l’historique de vos commits via `git log` <br>

* Votre historique contient-il bien les deux _commits_ que vous avez réalisés ?
* Quelle est la différence entre `git status` et `git log` ?

## Gitlab

### Création du compte
Créer votre compte sur [GitLab.com onglet Register](https://gitlab.com/users/sign_in). Ce compte sera utile pour plusieurs projets, remplissez les champs avec attention.

### Échange de clé
Pour vous reconnaître, GitLab/Github utilise un système de clé. Cette clé garantit votre identité sans utiliser un mot de passe.

### Génération de votre clé
Cette procédure n'est à faire qu'une seule fois « par ordinateur ». <br>
<br>
🚨 La procédure de génération de clé est la même pour Github et Gitlab, vous pouvez donc utiliser la même clé pour les deux services. 🚨 <br>
<br>
La commande sera la même, quel que soit votre système d'exploitation. Cependant, le terminal lui sera différent :<br>
<br>
* Windows : `Git Bash` (ou Git cmd`). (nécessite Git)
* macOS : `terminal`.
* Linux : `console`.

```sh
ssh-keygen
```
La commande va générer deux fichiers :<br>

* id_rsa, est privé. Vous ne devez jamais le partager.
* id_rsa.pub, est publique, vous pouvez le partager autant que vous voulez, ce fichier permettra de vous reconnaître au moment de la connexion.

_Vous pouvez faire « entrée (3×) » pour générer une clef sans mot de passe. Vous pouvez également faire le choix de mettre un mot de passe sur votre clef pour plus de sécurité._ <br>

#### Gitlab
Maintenant que nous avons généré les clefs, il vous suffit d'envoyer votre clef publique sur Gitlab pour que celui-ci vous reconnaisse automatiquement. <br>

Copier le contenu du fichier id_rsa.pub(ouvrir le fichier avec par exemple Notepad++)<br>
[L'ajouter à votre profil Gitlab](https://gitlab.com/-/profile/keys)<br>
Tester votre connexion avec la commande `ssh -T git@gitlab.com`<br>

### Création de votre premier projet
Maintenant que votre compte est créé (et que l’échange de clé est effectif), vous allez pouvoir créer un nouveau projet. Ce projet gitlab aura pour vocation de contenir les sources de votre site Internet <br>

* Je vous laisse explorer les menus de GitLab pour créer votre projet.
* Attention, vous devez choisir le type de projet Blank project ».
* Vous devez choisir la visibilité du projet. (Public ou Private).

#### Question
* Comment choisir la visibilité du projet ? (Visiblity Level)

Maintenant que votre projet est créé, GitLab doit vous donner les instructions pour « pusher » votre projet sur le serveur. Suivez les instructions. <br>

Je vous invite pour cette première fois à suivre les instructions que Gitlab vous donne.<br>

⬅️ [Intro](https://github.com/nicolas-sanch/tp-gitlab/blob/main/README.md) | [Part2](https://github.com/nicolas-sanch/tp-gitlab/blob/main/part2.md)  ➡️