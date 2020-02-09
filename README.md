# WorkShop_Python

WorkShop Python pour débutant

# Introduction Python

Python est un langage de programmation interprété, ce qui veut dire que les intructions que vous lui envoyez sont "transcrites" en langage machine au fur et a mesure de leur lecture.
Autrement dit c'est le contraire de langages comme le C et le C++ qui sont des langages compilés, car à la différence de python, ces langages ont besoin d'un logiciel spécialisé pour transformer le code en langage machine. A chaque modification du code il faut donc repasser par une compilation.  
En somme les avantages d'un langages interprété comme python sont la simplicité et la portabilité, un langage tel que Python est censé fonctionner aussi bien sous Windows que sous Linux ou Mac OS, et on ne devrait avoir à effectuer aucun changement dans le code pour le passer d'un système à l'autre.  
Cela ne veut pas dire que les langages compilés ne sont pas portables, mais ils doivent passer par une étape supplémentaire souvent source d'erreur. En revanche, un langage compilé est plus rapide à l'execution qu'un langage interprété.

Le python est aussi ce que l'on appel un langage de haut niveau, puisque le langage se rapproche plus du langage de l'homme que du langage de la machine. Au contraire le C est un langage de bas niveau puisque que le langage est plus proche de la machine que de l'homme.

## Partie 1 Hello World

Pour commencer il faut savoir que l'extension d'un fichier python est __.py__ nous allons donc créer un fichier HelloWorld.py. Le but de l'exercice est d'afficher "Hello World" à l'éxecution du script, rien de plus simple pour cela il nous suffit d'écrire :

`print("Hello World")`

Mais avant de pouvoir lancer notre script il reste une dernière chose à faire, en effet pour exécuter notre HelloWorld.py il nous faut les permissions, pour cela un `CHMOD 777 HelloWorld.py` suffira.

Il ne reste qu'à éxecuter notre script avec : `python3 ./HelloWorld.py`

On remarque ici que les fonctions ne sont pas nécessaires pour dévelloper en python, mais __Attention__ croire pouvoir coder sans fonctions serait une grave erreur. En effet, il est possible de tout programmer dans un seul fichier et sans fonctions, mais cela deviendrait une purge pour vous comme pour vos collègues. C'est pourquoi nous allons voir comment prototyper et utiliser des fonctions en python.

## Partie 2 Déclaration et type

Le typage d'une variable consiste à associer à sa variable symbolique un « type » de donnée, permettant à l'ordinateur de savoir si celle-ci est de type numérique, textuel, etc., d'allouer en conséquence des zones de mémoire de dimension suffisantes pour stocker cette donnée, et éventuellement de vérifier que les manipulations programmées sur cette variable (opérations mathématiques, traitement de texte, etc.) sont cohérentes avec son type.

En python le typage est dynamique et consiste à laisser l'ordinateur réaliser cette opération de typage « à la volée », lors de l'exécution du code, contrairement à certains langages statiquement typés qui demandent au programmeur de déclarer expressément, pour chaque variable qu'il introduit dans son code, son typage(Comme dans les langages impératifs tel que le C, C++, ...).

Le typage dynamique est une solution très commode pour le développement rapide de programmes, où le type des objets manipulés n'est pas forcément connu à l'avance, ou bien où le programmeur veut permettre par commodité le changement de type d'une variable.

Voici un exemple de déclaration de variable en python :

```
HelloWorld = "Hello World"
```

En plus de ne pas avoir besoin de prototyper nos variables à la main, le typage dynamique de python alloue de lui même la mémoire.

Autre exemple concret d'allocation de mémoire automatique :

```
tab = []
```
Dans cet exemple on crée on tableau, celui-ci est automatiquement alloué dynamiquement (pas besoin d'allouer la mémoire à la main et encore moins de la free, tout passe par un un sytème de garbage collection), et gère de lui même les types qui lui sont attribués.

__Attention :__

Même si le python type automatiquement cela ne veut pas dire que l'on peut créer un tableau contenant différents types. Si l'on décide de remplir notre tableau de 'int' alors on ne pourra pas ensuite remplir ce même tableau de 'string', à moins de le vider.

__Exercice__

Déclarer une varible lui attribuer lui une valeur ou une string et printer là.

## Partie 3 Fonction et module

Avant de passer à un peu de pratique nous allons voir comment :
* Prototyper une fonction
* Importer des modules

Tout d'abord voici la syntaxe d'une fonction en python :
```
def fonction(args):
        <code>
```
__Attention :__ Le python n'utilise pas d'accolade l'indentation est donc primordiale c'est elle qui permet à l'interpréteur de faire son travail.

Avant de passer à un petit exercice nous allons voir comment faire un main en python, ce n'est pas nécessaire mais ça permet d'aider à mieux comprendre comment notre code fonctionne.


```
def main():
        <code>

if __name__ == '__main__':
        main()
```
__Note :__ Pour appeler un main en python on cherche si il existe, si c'est le cas alors la condition est vérifié et le main est appelé.

__Exercice :__

Ecrivez une fonction autre que le main qui prend en argument une string et qui la print.

__Note :__ Si vous avez le moindre problème n'hésiter pas et appeler nous.

Passons aux modules. Si on devait faire un comparatif avec le C un module serait une lib et pour l'utiliser il nous faut l'import.

Voila à quoi ressemble un import en python :
```
import VotreModule
```

__Exercice :__

Comme pour l'exercice précedent vous devez print une string que votre fonction prend en argument, mais cette fois ci vous devrez récupérer la string comme argument du script. Pour cela vous aurez besoin d'import `sys`.

## Partie 4 Shebang

Le shebang, représenté par #!, est un en-tête d'un fichier texte qui indique au système d'exploitation (de type Unix) que ce fichier n'est pas un fichier binaire mais un script; sur la même ligne est précisé l'interpréteur permettant d'exécuter ce script.

L'intérêt ici est de ne plus avoir à éxecuter notre script à l'aide de la commande `python3 ./script.py`, un simple `./script.py` suffira à éxecuter notre script.

__Note :__ Le shebang à aussi un autre intérêt surtout si vous prévoyer de faire du python pour vos projets, sans shebang la moulinette ne pourra pas éxecuter votre script.

__Exercice :__

Ecrivez un script qui à l'exécution print une string __sans__ l'éxecuter avec python3.

__Note :__ Si votre shebang ne fonctionne pas vérifier sa synthaxe. Sinon appeler nous.

## Partie 5 Les boucles et condition



