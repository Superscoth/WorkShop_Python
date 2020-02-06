# WorkShop_Python

WorkShop Python pour débutant

# Introduction Python

Python est un langage de programmation interprété, ce qui veut dire que les intructions que vous lui envoyez sont "transcrites" en langage machine au fur et a mesure de leur lecture.
Autrement dit c'est le contraire de langages comme le C et le C++ qui sont des langages compilés, car à la différence de python, ces langages ont besoin d'un logiciel spécialisé pour transformer le code en langage machine. A chaque modification du code il faut donc repasser par une compilation.
En somme les avantages d'un langages interprété comme python sont la simplicité et la portabilité, un langage tel que Python est censé fonctionner aussi bien sous Windows que sous Linux ou Mac OS, et on ne devrait avoir à effectuer aucun changement dans le code pour le passer d'un système à l'autre. Cela ne veut pas dire que les langages compilés ne sont pas portables, mais ils doivent passer par une étape supplémentaire souvent source d'erreur. En revanche, un langage compilé est plus rapide à l'execution qu'un langage interprété.


## Partie 1 Hello World

Pour commencer il faut savoir que l'extension d'un fichier python est __.py__ nous allons donc créer un fichier HelloWorld.py. Le but de l'exercice est d'afficher "Hello World" à l'éxecution du script, rien de plus simple pour cela il nous suffit d'écrire :

`print("Hello World")`

Mais avant de pouvoir lancer notre script il reste une dernière chose à faire, en effet pour éxecuter notre HelloWorld.py il nous faut les permissions, pour cela un CHMOD 777 HelloWorld.py suffira.

Il ne reste qu'à éxecuter notre script avec : `python3 ./HelloWorld.py`

On remarque ici que les fonctions ne sont pas nécessaires pour dévelloper en python, mais __Attention__ croire pouvoir coder sans fonctions serait une grave erreur. En effet, il est possible de tout programmer dans un seul fichier et sans fonctions, mais cela deviendrait une purge pour vous comme pour vos collègues. C'est pourquoi nous allons voir comment prototyper et utiliser des fonctions en python.

## Partie 2 Les fonctions



Le python n'utilise pas d'accolade l'indentation est donc primordiale c'est elle qui permet à l'interpréteur de faire son travail.



