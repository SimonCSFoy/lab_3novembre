# Laboratoire - 2 novembre 2023

## Exercice #1 - Palindrôme

Faites un programme en utilisant les fonctions qui demande à l'utilisateur d'entrer une chaîne de caractères. Votre programme doit vérifier si la chaîne de caractères entrée est un palindrôme et afficher le résultat. Il __doit toujours le redemander à l'utilisateur__ tant qu'il n'appuie pas sur le bouton pour fermer la fenêtre du terminal. Assumez que l'utilisateur entrera que des lettres minuscules.
> [!NOTE]
> Définition de palindrôme selon Wikipédia : Mot ou groupe de mots qui peut se lire indifféremment de gauche à droite ou de droite à gauche en gardant le même sens.
> Par exemple, si la chaîne de caractère initale est le mot `laval`, si on le lit à l'envers on obtient toujours `laval`. C'est donc un palindrôme.

Voici une liste de fonctions qui pourraient être utiles. Vous pouvez en ajouter des supplémentaires si nécessaire.
```c#
string InverserTexte(string texteEntree);
```
```c#
string ObtenirStringUtilisateur(string message);
```
```c#
bool EstPalindrome(string texte);
```

__Voici un visuel de ce que le programme doit produire :__ 
```console
Entrez une chaîne de caractères en minuscules à vérifier :
laval
laval est un palindrôme.

Entrez une chaîne de caractères en minuscules à vérifier :
allo
allo n'est pas un palindrôme.

Entrez une chaîne de caractères en minuscules à vérifier :
kayak
kayak est un palindrôme.

Entrez une chaîne de caractères en minuscules à vérifier :
aa bb cc cc bb aa
aa bb cc cc bb aa est un palindrôme.
```
---
## Exercice #2 - Nombre pair
Faites un programme en utilisant les fonctions qui demande à l'utilisateur d'entrer un __nombre entier__. Votre programme doit vérifier si le nombre entré est un nombre pair et afficher le résultat. Il __doit toujours le redemander à l'utilisateur__ tant qu'il n'appuie pas sur le bouton pour fermer la fenêtre du terminal.

> [!NOTE]
> __Indices__ : La boucle principale du programme devrait se trouver dans le `Main`.
> La seule place que vous devriez retrouver un `Console.Readline()` dans votre code est dans la fonction `ObtenirStringUtilisateur`.

Voici une liste de fonctions qui pourraient être utiles. Vous pouvez en ajouter des supplémentaires si nécessaire.
```c#
int ObtenirEntierUtilisateur(string message);
```
```c#
string ObtenirStringUtilisateur(string message);
```
```c#
bool EstPair(int nombre);
```

__Voici un visuel de ce que le programme doit produire :__ 
```console
Entrez un nombre entier :
10
Le nombre 10 est pair

Entrez un nombre entier :
11
Le nombre 11 n'est pas pair

Entrez un nombre entier :
43287592
Le nombre 43287592 est pair
```
---
## Exercice #3 - Palindrôme pair
Le but de cet exercice est de combiner les deux premiers exercices en un seul programme. Le logiciel affiche un menu principal avec quatre options à l'utilisateur (voir plus bas pour le visuel). Le choix #1 exécute l'exercice #1 avec comme seule différence qu'il l'exécute une seule fois et revient ensuite au menu principal. Même principe pour le choix #2, mais avec l'exercice #2. L'option #3 elle est nouvelle et exécute un programme qui valide si le nombre entré est un nombre pair ET un palindrôme et affiche le résultat. L'option #4 est pour quitter le programme.

> [!NOTE]
> __Indices__ : La boucle principale du programme devrait toujours se trouver dans le `Main`.
> Le contenu de la fonction `ProgrammeVerifierPair()` est sensiblement un __copier coller du `Main` de l'exercice #2.__ Même chose pour `ProgrammeVerifierPalindrome()`, mais avec l'exercice #2. La majorité des autres fonctions sont __identiques à celles programmées dans les exercices précédents__.

Voici une liste de fonctions qui pourraient être utiles. Vous pouvez en ajouter des supplémentaires si nécessaire.
```c#
void ProgrammeVerifierPair()
```
```c#
void ProgrammeVerifierPalindrome()
```
```c#
void ProgrammeVerifierPalindromeEtPair()
```
```c#
void AfficherMenu()
```
```c#
string InverserTexte(string texteEntree)
```
```c#
string ObtenirStringUtilisateur(string message)
```
```c#
bool EstPalindrome(string texte)
```
```c#
int ObtenirEntierUtilisateur(string message)
```
```c#
bool EstPair(int nombre)
```
__Voici un visuel de ce que le programme doit produire :__ 
```console
(1) - Vérifier si un nombre est pair
(2) - Vérifier si une chaîne de caractères est un palindrôme
(3) - Vérifier si un nombre est pair ET est un palindrôme
(4) - Quitter

Entrez votre choix :
1

Entrez un nombre entier :
5884
Le nombre 5884 est pair
(1) - Vérifier si un nombre est pair
(2) - Vérifier si une chaîne de caractères est un palindrôme
(3) - Vérifier si un nombre est pair ET est un palindrôme
(4) - Quitter

Entrez votre choix :
2

Entrez une chaîne de caractères en minuscules à vérifier :
kayak
kayak est un palindrôme.

(1) - Vérifier si un nombre est pair
(2) - Vérifier si une chaîne de caractères est un palindrôme
(3) - Vérifier si un nombre est pair ET est un palindrôme
(4) - Quitter

Entrez votre choix :
3

Entrez un entier à vérifier :
2442
2442 est un entier palindrôme pair.

(1) - Vérifier si un nombre est pair
(2) - Vérifier si une chaîne de caractères est un palindrôme
(3) - Vérifier si un nombre est pair ET est un palindrôme
(4) - Quitter

Entrez votre choix :
4

Sortie de C:. Code : 0.
Pour fermer automatiquement la console quand le débogage s'arrête, activez Outils->Options->Débogage->Fermer automatiquement la console à l'arrêt du débogage.
Appuyez sur une touche pour fermer cette fenêtre. . .
```
