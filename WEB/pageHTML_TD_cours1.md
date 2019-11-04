

I -- Navigateur et langages 
---------------------------

Pour parcourir ('to browse' in english) le **web**, la principale application d'internet, il faut disposer d'un navigateur ('browser' en anglais).  
Les navigateurs sont nombreux et possèdent tous des qualités et des défauts par rapport aux autres. Les plus connus actuellement sont certainement **Firefox** de Mozilla, **Chrome** de Google et **Edge** de Microsoft (le successeur d'**Internet Explorer**). **Safari** reste la référence sur les machines Apple.
La plupart des navigateurs mobiles sont des versions adaptées à ce support des logiciels précédents.

Le navigateur reçoit des instructions (un code HTML) et __l'interprète__ en affichant (correctement ou non) du texte, des images, des vidéos ...

*__Un rapide aperçu 'historique' de l'HTML :__*


HTML (**HyperText Markup Language**) fait son apparition dès 1991 lors du lancement du Web. Son rôle est de gérer et d'organiser le contenu. HTML sert à définir clairement le type de données que vous allez afficher à l'écran. En anglais, _'Markup'_ signifie _'balise'_, on verra l'importance de ce mot ...

-   HTML 1 : c'est la toute première version créée par Tim Berners-Lee
    en 1991.
-   HTML 2 : cette version du HTML apparaît en 1994 et cette fois les
    règles sont établies par une organisation,le W3C .
-   HTML 3 : cette version date de 1996 et on y trouve plusieurs ajouts
    (tableaux, applets, scripts,...)
-   HTML 4 : apparaît en 1998 et propose plusieurs améliorations (dont l'utilisation de frames) et surtout, cette version permet
    d'utiliser le CSS (on en reparlera plus tard) : la forme de la page n'a plus à être mélangée avec son contenu.
-   HTML 5 : La dernière version pour l'instant.


II -- Le logiciel à utiliser
----------------------------
Un code HTML n'est qu'une suite de données : une suite très codifiée d'ordres alphanumériques. L'ordinateur ne peut en aucun cas « comprendre» le code : il le déchiffre caractère par caractère contrairement à un humain. Par conséquent, la moindre erreur rend l'instruction incompréhensible pour lui..

Le code HTML n'est au final qu'un simple texte. Le **bloc-note** peut suffir pour créer ce code. 

Une fois le code tapé, il faut en vérifier l'exécution et la compréhension à l'aide d'un navigateur.

 1. Ouvrir **Bloc Note**. 
 2. Notez sur plusieurs lignes le texte que vous voulez afficher:
```
Phrase sur la première ligne.
Phrase sur la deuxième ligne.
Contenu un peu spécial.
Ceci est une partie importante.
Là, je veux vraiment que personne ne le manque.
```  
 3. Choisir un encodage UTF-8. Enregistrez le fichier sous format **.html** (c'est à dire que vous ajoutez une extension à votre nom de fichier de manière à indiquer que vous choisissez HTML comme langage).
 4. Laisser le **Bloc Note** ouvert, et lancer l'explorateur pour ouvrir le dossier dans lequel se trouve votre fichier.
 5. Exécuter en double cliquant sur votre fichier dans l'explorateur pour voir le résultat.

On constate que le HTML sait afficher du texte (quelle surprise !) Par contre, le navigateur n'a pas compris que vous vouliez partir à la ligne. Il affiche les phrases à la suite des autres : votre code n'est pour l'instant constitué que de texte, il manque les instructions d'affichage : le fait d'avoir fait des passages à la ligne dans le fichier HTML ne change rien à l'affaire : le navigateur ne les « voit » pas. Pour lui, c'est comme si vous aviez tout tapé sur la même ligne.

III -- Les premières balises pour structurer le texte de base
--------------------------------------------------------

Les **balises** et leurs chevrons ```< >```, voilà ce qui va structurer le code et donner des informations à votre navigateur.

En HTML, les indications sont toujours définies par des **balises**.

Les balises d'instructions ou d'informations vont souvent par paire : la
première (ouvrante) indique l'instruction à suivre et à partir de où démarre son contenu, et la seconde (fermante) signale la fin du contenu. La seconde contient un slash ( / ) supplémentaire pour bien la distinguer de la première.

 6. Modifiez la première ligne de votre code dans le **Bloc Note** comme indiqué ci-dessous.  
```<h1>Phrase sur la première ligne.</h1>```
 7. Sauvegardez et relancez pour voir ce que cela change.
 8. Voilà quelques exemples de balises  :

-   ```<h1>``` fermée par ```</h1>``` : les balises de titre principal.
-   ```<p>``` fermée par ```</p>``` : les balises de .............
-   ```<em>``` fermée par ```</em>``` : les balises de ................
-   ```<strong>``` fermée par ```</strong>``` : les balises de ..................
-   ```<mark>``` fermée par ```</mark>``` : les balises de ..................  

Utiliser les balises précedentes sur une ligne à la fois pour voir la différence de traitement.

Il existe beaucoup de balises différentes que nous allons utiliser.
Chacune d'elle apporte au navigateur soit une information sur le contenu (texte, image, vidéos, fichiers, liens ...), soit la nature du contenu (titre, liste d'éléments, paragraphe normal, élément important  ...  ).

 9. Remplir le tableau suivant :


  |Balise                      |```<h1>``` | ```<p>``` | ```<em>``` | ```<strong>``` | ```<mark>```|
  |----------------------------|-----------|-----------|------------|----------------|-------------|
  |Passage à la ligne ?        |                                                
  |Augmentation de la taille ? |                                         
  |Italique ?                  |                                                         
  |Gras ?                      |                                                             
  |Surligné ?                  |                                                         


Il existe également de plus vielles balises pour mettre en gras ou en italique. C'est encore de l'anglais : les balises ```<b>```
pour [bold]```<i>``` pour [italic]
Nous expliquerons la différence avec ```<strong>``` et ```<em>``` plus loin dans le chapitre.

Parfois, on désire afficher une **liste**. Nous disposons alors de deux types possibles de liste : la liste ordonnée (avec des numéros) et la liste normale (pas ordonnée, sans numéro).

Si la liste est **ordonnée** (comme les explications à suivre pour écrire en HTML...), on la crée avec des balises ```<ol>``` et ```</ol>```, ol pour **Ordered List**.

Si la liste n'est **pas ordonnée** (comme une liste d'achats), on la crée avec des balises ```<ul>``` et ```</ul>```, ul pour **Unordered List**.

Les éléments d'une liste sont à donner entre des balises ```<li>``` et ```</li>```.

un exemple de liste **ordonnée**   :
```html
<ol> Comment structurer mon texte en HTML

    <li>ouvrir la balise choisie</li>

    <li>taper mon texte</li>

    <li>fermer la balise</li>

</ol>
```

On voit bien que la première ligne signale l'ouverture d'une nouvelle liste ordonnée.

Les trois lignes suivantes strucurent les éléments de la liste.

La dernière ligne précise la fermeture de la liste ordonnée.


**Exemple de liste non ordonnée** :

```html
<ul> Ma liste de course

    <li>lait</li>

    <li>oeufs</li>

    <li>farine</li>

</ul>
```


10. Rajouter une liste ordonnée et une liste non ordonnée sur votre page.
11. Nous allons maintenant voir notre première balise **orpheline**. La balise  `<br>`  
Qu'est-ce qu'une balise **orpheline** ? C'est une balise solitaire : on n'a pas besoin de refermer l'instruction avec une seconde balise.  
Placer quelques balises `<br>` dans votre code.  
Que peut-on remarquer? (--> br signifie 'bracket return', c'est à dire 'retour chariot'...)


**Résumons** :

Le **saut de ligne** n'est pas implanté de base dans la reconnaissance
du texte. Pour faire sauter le texte, il faut fermer par une balise titre, paragraphe ou ligne. Dans certains cas, on peut utiliser unebalise `<br>`.

Les balises **\<em\>**, **\<strong\>** et **\<mark\>** permettent de signaler l'importance d'une partie du texte.

Les balises **\<p\>** permettent de signaler qu'on désire un paragraphe.
Le début du texte est donc sur une nouvelle ligne et la fermeture de la balise entraîne un passage à la ligne.

Les balises **\<h1\>** à **\<h6\>** indiquent la présence d'un titre, h1 représentant un titre plus important sémantiquement que h6.

Les balises **\<ol\>** et **\<li\>** permettent de créer des listes ordonnées.

Les balises **\<ul\>** et **\<li\>** permettent de créer des listes non ordonnées.


**Une dernière remarque qui a son utilité!!!**

Les balises `<!--` et `-->` sont très spéciales... on remarque d'ailleurs qu'elles ne s'ouvrent pas et ne se ferment pas de la même manière que les autres. Elles permettent d'insérer des commentaires qui ne seront ni affichés ni interprétés. Très utiles lorsqu'on veut donner des indications à un lecteur de notre code, ou pour se souvenir de la signification d'une partie du code.
```html
<ul> <!-- on commence ici une liste non ordonée --> 

    <li>Rentrer en classe</li> <!-- chaque balise <li> donne un élément de liste -->

    <li>Travailler</li>

    <li>Sortir de la classe</li>

</ul> <!-- on termine ici une liste non ordonée -->
```


Nous avons maintenant les connaissances de base nous permettant de voir comment structurer notre première page html.

IV -- Squelette de base d'une page HTML
--------------------------------------------------------
Il reste un point important à aborder... 
Pour qu'une page soit correctement interprétée par un navigateur et être lue selon le protocole HTTP, il est nécessaire de respecter une structure de base.
```html
<!DOCTYPE html>                      <!--  on indique qu’il s’agit d’une page html   -->
<html>                               <!--  la balise principale qui englobe tout le contenu de la page   -->
<head>                               <!--  la section head donne des informations générales sur la page   -->
<meta charset="UTF-8">               <!--  l’encodage utilisé par le fichier html, UTF8 permet d’afficher pratiquement tous les symboles de toutes les langues  -->
<title> SNT Lycée Jean Bart </title> <!--  le titre qui s’affiche dans l’onglet du navigateur, il apparaît également dans les résultats de recherche des moteurs tels que Google   -->

</head>

<body>  

   <!--  c’est le corps de la page qui va contenir tout le texte, le code HTML que vous avez tapé   -->

</body>

</html>  <!--  n'oubliez pas de fermer cette balise   -->
```
 
12. Enregistrer ce fichier sous le nom "squeletteDOM.html" ( _'DOM' signifie Document Object Model_). On réutilisera ce document HTML pour chaque nouveau fichier HTML que nous serons amenés à créer.  
La section  ```<head>.....</head>``` ( _'la tête' en anglais_) de la page est particulièrement importante dès lors que votre fichier .html est destiné à être mis en ligne. Elle donne des informations générales au navigateur.  
On verra dans la suite du cours qu'elle devra encore être complétée.
