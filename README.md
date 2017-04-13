Rex
===

[![Join the chat at https://gitter.im/RexCSS/Lobby](https://badges.gitter.im/RexCSS/Lobby.svg)](https://gitter.im/RexCSS/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Plus qu'un simple framework, un ami pour la vie.

Installation
------------

Vous pouvez directement télécharger le projet sur cette page web ou en utilisant cette commande.

```shell
$ git clone https://github.com/Mimyka/Rex.git
```

Caractéristiques
----------------

Rex est un framework CSS sur la base de flexbox.
Il a été conçu pour être léger et coder beaucoup plus rapidement.

* Une grille responsive adaptable en fonction de vos besoins (SASS).

* Pas de style interne, ce qui vous laisse designer librement vos projets.

* Une syntaxe rapide et minimaliste

* Mobile first

* Un poids léger (20.8ko minifié)

* Utilisant la technologie moderne qu'est le Flexbox

Fichiers
--------

Les fichiers dans le dossier src (source) sont destinés au développement.

* `rex.css`: Le framework tout juste compilé, sans prefixes vendeurs.

* `rex.sass`: Base de développement, peut être utilisé pour personnaliser
le nombre de grid ou les préfixes pour le responsive (s/m/l/xl) simplement.

Les fichiers dans le dossier css sont destinés à ceux voulant utiliser Rex.

* `rex.css`: Le framework, avec les prefixes vendeurs pour assurer plus de compatibilité.
Il y a également quelques ajustement pour optimiser sa taille.

* `rex.min.css`: Le framework, minifié, destiné à la production.

Documentation
-------------

Rex fonctionne avec un système de lignes et de colonnes flex.
* `.r` : ligne (row)
* `.c` : colonne (column)

``` css
/* Pour le nowrap, il y a aussi les classes .r-no et .c-no */
.r{
    display: flex;
    flex-wrap: wrap;
}
.c{
    display: flex;
    flex-wrap: wrap;
    flex-direction: column;
}
```

On utilise dans celles ci, des unités allant de 1 à 24.
* `.u-[nbr]` : unité (unit)

``` css
/* Il y a aussi la classe .u qui correspond à flex: 1 */
.u-24{
    width: 100%;
}
.u-23{
    width: 95.83333%;     
}
.u-22{
    ...
}
```

Pour placer ces unit, on peut utiliser toutes les propriétés d'align-items/content/self et justify-content:
* `.[x|y]-start` : alignement sur l'axe choisi au début (défaut)
* `.[x|y]-end` : alignement sur l'axe choisi à la fin
* `.[x|y]-center` : alignement sur l'axe choisi au centre
* `.[x|y]-around` : alignement sur l'axe choisi en mode space-around
* `.[x|y]-between` : alignement sur l'axe choisi en mode space-between
* `.start` : alignement de l'élément choisi en mode align-self: start
* `.end` : alignement de l'élément choisi en mode align-self: end
* `.center` : alignement de l'élément choisi en mode align-self: center

Ces propriétés doivent être appliqué sur une ligne ou une colonne flex pour ainsi aligner les éléments enfants :

``` html
<div class="r x-center y-center">
    <div>
	<!-- Je vais être centré horizontalement et verticalement par rapport à mon parent -->
    </div>
    <div class="end">
	<!-- Je vais être centré horizontalement et être verticalement à la fin de mon parent -->
    </div>
</div>
```

Également disponible, un système d'offset également basé de 1 à 24:
* `.o-[nbr]` : offset

``` css
.o-24{
    margin-left: 100%;
}
.o-23{
    margin-left: 95.83333%;     
}
.o-22{
    ...
}
```

Aussi présente la classe hidden.
* `.hidden` : hidden

``` css
.hidden{
    visibility: hidden;
}
```


A tout ceci, l'on peut ajouter librement des préfixes pour faire du responsive.
* `...` : all
* `.s-...` : >= 568px
* `.m-...` : >= 768px
* `.l-...` : >= 1080px
* `.xl-...` : >= 1280px


Compatibilité navigateurs
-------------------------

Les tests n'ont pas encore été tous accomplis.
Rex fonctionne normalement sous :

* IE 10+
* Latest Stable: Firefox, Chrome, Safari
* Android 2.1+

Si vous rencontrez des bugs sous ces versions, n'hésitez pas à nous en faire part.

Pour assurer une plus grande compatibilité, vous pouvez utiliser [Flexibility.js][].

[Flexibility.js]: https://github.com/jonathantneal/flexibility

Licence
-------

Rex est sous licence MIT.
Regardez le [fichier de LICENCE][] pour plus d'informations.


[fichier de LICENCE]: https://github.com/Mimyka/Rex/blob/master/LICENSE
