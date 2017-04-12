Rex
===

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

* Un poids léger (18.9ko minifié)

* Utilisant la technologie moderne qu'est le Flexbox

Fichiers
--------

Les fichiers dans le dossier src (source) sont destinés au contributeurs.

* `rex.css`: Le framework tout juste compilé, sans prefixes vendeurs.

* `rex.sass`: Base de développement, peut être utilisé pour personnaliser
le nombre de grid ou les préfixes pour le responsive (s/m/l/xl) simplement.

Les fichiers dans le dossier css sont destinés à ceux voulant utiliser Rex.

* `rex.css`: Le framework, avec les prefixes vendeurs pour assurer plus de compatibilité.
Il y a également quelques ajustement pour optimiser sa taille.

* `rex.min.css`: Le framework, minifié, destiné à la production.

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
Regarder le [fichier de LICENCE][] pour plus d'informations.


[fichier de LICENCE]: https://github.com/Mimyka/Rex/blob/master/LICENSE
