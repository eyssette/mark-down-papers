Mark(down)Papers est un outil en ligne d'aide à l'annotation et l'évaluation de travaux d'élèves, au format texte.

Il est accessible ici : [https://eyssette.github.io/mark-down-papers/](https://eyssette.github.io/mark-down-papers/)

## Fonctionnement
1. Copier-coller le texte de la copie dans la fenêtre de gauche.
2. Cliquer sur l'étoile dans la barre d'icônes (tout à droite) pour mettre en forme automatiquement le texte.
3. Annoter la copie (cf. ci-dessous). Les raccourcis ordinaires pour annuler (Cmd + Z) ou rétablir (Cmd + Shift + Z) la dernière action fonctionnent.
4. Transmettre la correction, soit par copier-coller de la fenêtre de droite, soit par impression dans un fichier PDF (Cmd-P ou Ctrl-Cmd-P). Attention : si vous souhaitez pouvoir reprendre votre correction pour la modifier, il faut conserver la fenêtre de gauche (p.ex. par copier-coller dans un [pastebin](https://pastebin.zici.fr/))

Le document est automatiquement sauvegardé (à chaque seconde).

## Les possibilités d'édition du texte

### Souligner, barrer, italiques, gras, puces

* Souligner : Cmd + U
* Barrer : Cmd + Shift + X
* Italiques : Cmd + Shift + I (ou bouton : “I”)
* Gras : Cmd + Shift + B (ou bouton : “B”)
* Puces : commencer par “1.” pour une liste numérotée, par “*” pour une liste non numérotée (ou utiliser les icônes correspondantes)

<i>Exemple</i> : Lorem `ipsum dolor` ~~sit amet~~,  <i>consectetur</i> <b>adipiscing</b> elit.

### Commenter un passage

* En bleu : Cmd + I
* En rouge : Cmd + B
* Souligner puis commenter en bleu :  Ctrl + Cmd + U

<i>Exemple</i> : Lorem ipsum dolor *Commentaire en bleu* sit amet, consectetur adipiscing elit.**Commentaire en rouge** Maecenas ut egestas orci, `accumsan pharetra`*Passage souligné puis commentaire en bleu* felis.

### Rédiger une appréciation générale

Il suffit de commencer chaque ligne avec le caractère “>”. On peut, à l'intérieur d'une appréciation utiliser les raccourcis ci-dessus.
 
>Lorem ipsum dolor sit amet, consectetur <i>adipiscing elit</i>.
>
> Maecenas ut <b>egestas orci</b>, accumsan pharetra felis.
> 
> 1. Nullam venenatis imperdiet sapien, eget fringilla lorem venenatis non.
> 2. Donec vitae est varius, maximus erat non, porttitor ante.

### Notes de bas de page

<i>Exemple</i> : Lorem ipsum^[Note dans le texte lui-même] dolor sit amet[^mot-clé-pour-cette-note], consectetur adipiscing elit.

[^mot-clé-pour-cette-note]: Note définie par un mot clé

<br/>

<i>Code</i> : Lorem ipsum`^[Note]` dolor sit amet`[^mot-clé]`, consectetur adipiscing elit.

`[^mot-clé]:` Note

## Autres fonctions
### Compteur de mots
Le compteur de mot dans la barre d'icônes est automatiquement réinitialisé lorsqu'on formate le texte avec l'icône “étoile”. Sinon, il suffit de cliquer sur l'icône “calculatrice” pour recalculer le nombre de mots.
### Chronomètre
* Lancer ou arrêter le chronomètre : Ctrl + S (ou : cliquer sur l'icône “sablier”)
* Réinitialiser le chronomètre : Ctrl + R (ou : cliquer sur l'icône “retour en arrière”)

## Modules expérimentaux
### Aide à l'évaluation
Pour chaque paragraphe, vous pouvez mettre une évaluation de cette manière : `<n>+</n>`

La balise <n>+</n> ne se voit pas dans la fenêtre de droite (et donc n'apparaîtra pas dans le fichier destiné à l'élève). Pour l'évaluation, on a le choix entre 7 options :


| Code | Note / 20 | Classement |
|:--------:|:--------:|:--------:|
| +++     | 20     | A+     |
| ++     | 17.5     | A     |
| +     | 15     | B     |
| +-     | 12.5     | C+     |
| -+     | 10     | C     |
| -     | 7.5     | D     |
| --     | 5     | E     |


* Insérer la balise : Ctrl-n
* Calculer la note : Shift-Ctrl-n (le module fait simplement la moyenne des évaluations).

### Insertion automatique d'une annotation type
Pour définir des annotations automatiques, il faut cliquer sur le “code barre” dans la barre d'icônes, et insérer ses codes, en respectant la syntaxe indiquée. Il suffira ensuite d'insérer le code de cette manière : `<a class="code"></a>`

* Insérer une annotation type : Cmd-Ctrl-A

### Annotations dans la marge
Il est possible d'insérer des remarques très courtes dans la marge, à gauche ou à droite. Cela peut fonctionner si on a un système de codage de ses annotations : par exemple E<sup>+</sup> <span class="margeL">E^+^</span> (pour un bon exemple) ou OL<sup>-</sup> <span class="margeR">OL<sup>-</sup></span> (pour une organisation logique défaillante).

Si on veut utiliser des remarques plus longues, il faut encadrer la copie de l'élève avec les balises suivantes : `<div class="grandesmarges"></div>`

* Mettre un commentaire dans la marge à gauche : Ctrl-M
* Mettre un commentaire dans la marge à droite : Shift-Ctrl-M
* Insérer un caractère ou un mot en <sup>exposant</sup> : `^mot^`
    * Raccourci pour le signe ⁺ : Ctrl-P
    * Raccourci pour le signe ⁻ ; Shift-Ctrl-P

## Crédits
Cet outil vous est proposé, sans garantie de fonctionnement. Il a été construit à partir de :
* [SimpleMDE](https://github.com/sparksuite/simplemde-markdown-editor/)
* [Turndown](https://github.com/domchristie/turndown)
* [Online Stopwatch](https://github.com/kaleidawave/online-stopwatch)
* [Remarkable](https://github.com/jonschlinkert/remarkable)
