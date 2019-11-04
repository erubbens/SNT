I. Du HMTL un peu stylé !
------------
On l'a vu, le rôle du fichier HTML est d’organiser le fond, le contenu de la page, avec des __balises__ .
Les balises possèdent généralement des options, appelées attributs.
Un attribut est toujours écrit dans la balise ouvrante, suivie d'un espace.
On lui associe sa ou ses propriétés avec un signe '=' et entre guillemets.
Par exemple, une balise orpheline qui permet d'insérer des images et dont on reparlera plus tard...
```html
<img src= "maphoto.jpg">
```
La balise est ```<img>``` et son attribut est ```src``` , la propriété associée à l'attibut est ```"maphoto.jpg"``` qui indique le chemin vers le fichier source de cette image.
L'attribut ```style``` : Pendant plusieurs années, on a codé le fond et la forme dans le même fichier en utilisant l'attribut style.
1. Ouvrir Bloc Note, puis ouvrir votre fichier HTML.
2. Dans une balise html ```<p> ```, taper le code suivant :
```<p style="color :blue"> Mon texte contenu dans ma balise paragraphe </p>```
3. Exécuter en double cliquant sur votre fichier dans l'explorateur pour voir le résultat. Le texte contenu dans la balise s'affichera en ...... ?
4. Imaginons maintenant que l'on veuille en plus que le texte soit souligné en rouge, une couleur de fond grise, une bordure jaune,... on va utiliser différentes propriétés de style.
```<p style="color :blue ; font-size :10px ; text-decoration: underline red ; background-color : grey ; border : solid yellow"> Mon texte contenu dans ma balise paragraphe </p>```
Le principal défaut de cette méthode est de surcharger la balise et de perdre de vue son contenu.
C'est surtout pour éviter ce problème de lisibilité qu'à été inventé le CSS, que nous allons tout de suite aborder...  

II. CSS: Cascading Style Sheets
-------------------------------
Le rôle du fichier CSS (Cascading Style Sheets) dont la dernière version est CSS3, est de gérer la mise en forme c’est-à-dire l’apparence de la page web: la couleur, la taille, le positionnement ... Il est apparu en 1996. Cascading Style Sheets se traduit littéralement par feuilles de styles en cascade.

CSS 1 : dès 1996, on dispose de la première version du CSS. Elle pose les bases de ce langage qui permet de présenter sa page web, comme les couleurs, les marges, les polices de caractères, etc.
CSS 2 : apparue en 1999 cette version rajoute de nombreuses options.
CSS 3 : la dernière version, qui apporte des fonctionnalités comme les bordures arrondies, les dégradés, les ombres, flex etc.
Il vous suffira d’ajouter l’extension appropriée .html ou .css lors de l’enregistrement de vos fichiers et nous allons voir comment. Un bon créateur de site web doit absolument connaître les règles de base des langages HTML et CSS.

III. Utilisation du CSS
------------------------
Nous allons utiliser un outil intéressant et disponible gratuitement ... jsfiddle.

5. Rendez-vous à l'adresse https://jsfiddle.net. Vous devez aboutir à une page ressemblant à cette image: ![image de jsfiddle](img_jsfiddle.jpg)  
On remarque bien un espace pour le code HTML et un espace pour le code CSS séparé. (On ne se servira pas de l'espace JavaScript)
6. Dans l'espace HTML, taper ```<p> Mon texte contenu dans ma balise paragraphe </p>```. Puis cliquer sur l'icone en haut à gauche 'Run'. Vous observez le résultat dans l'espace Result.
7. Dans l'espace CSS, taper ```p {color :blue}``` . Observez le résultat.  
Remarquez bien que l'attribut style n'est plus nécessaire, puisque nous sommes dans une feuille de style!

__Structure générale du code CSS__

On trouve dans le code CSS

des noms de balises appelés sélecteurs
des propriétés CSS en cascade
des valeurs  

il faut respecter la structure suivante :
```css
balise1
{ 
propriete1 : valeur1 ;
propriete2 : valeur2 ;
propriete3 : valeur3 ;
}
balise2
{ 
propriete1 : valeur4 ;
propriete2 : valeur5 ;
propriete3 : valeur6 ;
}
```

8. Dans notre exemple pris au début, tapez dans l'espace CSS, puis observez le résultat:

```css
p
{
color : blue ;
font-size :10px ;
text-decoration: underline red ; 
background-color : grey ; 
border : solid yellow;
}
```

9. On va enrichir un peu notre code HTML. Tapez:

```html
<p> Mon texte contenu dans ma balise paragraphe </p>
<h1> un titre </h1>
<h2> un sous-titre </h2>
<p> un autre paragraphe </p>
```
On l'a dit, le CSS permet plus de lisibilité du code, mais vous pouvez remarquer ici un autre avantage très important: tous les paragraphes repérés par la balise ```<p>....</p>``` ont hérité des propriétés énoncées dans le fichier css. Inutile de répéter la même chose pour chaque balise... __Gain de temps et lisibilité !__

10. En vous inspirant du CSS sur la balise ``` <p> ```, donner un style à vos balises ```<h1>``` et ```<h2>```

>remarque: vous pouvez utiliser la propriété 'text-align:' avec la valeur center, ou pour un peu plus de 'fun', les propriétés 'text-shadow:' et 'box-shadow:' avec les valeurs '3px 3px 1px black;' ...

>Il existe une multitude de propriétés CSS et il n'est pas question d'en faire la liste ici. Vous pourrez facilement en trouver d'autres en "fouillant" un peu sur le Web !

III. Comment place-t-on le code CSS ?
--------------------------------------

On vient de le voir, ll est donc conseillé, voire obligatoire, d’utiliser un fichier css pour distinguer nettement le fond de la forme ; par ailleurs, et c’est là le plus important, si le site comporte plusieurs pages, on peut affecter la même mise en forme pour toutes les pages du site. Ainsi une modification dans le seul fichier css affectera immédiatement la mise en forme de toutes les pages du site.

11. Dans le Bloc Note, ouvrir votre fichier "squeletteDOM.html" et l'enregistrer sous le nom "fichier_exo.html"
12. Coller le code HTML que vous avez tapé dans Fiddle. Enregistrez.
13. Toujours dans Bloc Note, ouvrir un nouveau fichier, puis coller le code CSS que vous avez tapé dans Fiddle.
14. Sauvegardez ce fichier dans votre répertoire sous le nom "style_exo.css".
On vient de créer un fichier externe de mise en forme appelé "style_exo.css" qui accompagnera mon "fichier_exo.html".

15. Exécuter en double cliquant sur votre fichier "fichier_exo.html" dans l'explorateur pour voir le résultat.
On observe.... RIEN!!! ??? Aucune mise en forme, notre texte apparait brut! Problème: Comment le navigateur peut-il identifier que ces deux pages doivent être liées?
Pour cela, dans le fichier html, il faudra ajouter une balise spéciale... la balise ```<link>``` ( 'lien' en anglais).
C'est une balise orpheline, qui ne doit pas être fermée. Elle recevra 2 attributs:
```html
<link rel="stylesheet" href="style_exo.css">
```
16. Dans le Bloc Note, ouvrir votre fichier "fichier_exo.html".
17. Rajoutez ```<link rel="stylesheet" href="style_exo.css">``` dans la section ```<head>.....</head>``` de manière à obtenir le code suivant:

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>SNT Lycée Jean Bart</title>
<link rel="stylesheet" href="style_exo.css" />
</head>

<body>
<p> Mon texte contenu dans ma balise paragraphe </p>
<h1> un titre </h1>
<h2> un sous-titre </h2>
<p> un autre paragraphe </p>
</body>

</html>
```

18. Exécuter en double cliquant sur votre fichier "fichier_exo.html" dans l'explorateur pour voir le résultat.