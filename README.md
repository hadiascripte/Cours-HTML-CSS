
# HTML
## Les balises

### Balise html
Balise principale dans laquelle se trouve tout le contenu du site

### Balise head
Balise qui contient ce qui n'apparaît pas sur le site.
Elle contient notamment la meta, le title; îcone de l'onglet 
```
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title> Titre </title>
        link rel="shortcut icon" href="image"
        <link rel="stylesheet" href="./style.css" />
    </head>
```

### Balise body
Balise qui contient tout ce qui sera visible sur le site.


## Balise nav

On y ajoute généralement un ul:

```
<nav>
    <ul>
        <li></li>
        <li></li>
        <li></li>
    </ul>
</nav>
```
## Balise header
Partie comportant, en principe, les informations principale du site (qui ne se répèteront pas)

```
<header>
    <h1></h1>
    <p></p>
</header>
```
## Balise main
Partie comportant les informations globales du site.
```
<section class="section1">
    <h2>
        <ol>
            <li></li>
            <li></li>
        </ol>
    </h2>
</section>

<section class="section2">
    <h3>></h3>
    <img src="./image.png" height="200" alt="image-section/>
</section>
```
## Les tableaux
On doit d'abord lui mettre un ***border*** pour qu'il puisse être visible sur le site.

### L'en-tête du tablea (thead)
```
    <table border="4"></table>
```
 Pour l'entête du tableau on ajour une balise ***thead**
 ```
    <thead> </thead>
```
Pour créer une ligne (row) on ajoute une balise ***tr*** à l'intérieur du ***thead*** 
```
    <thead> 
        <tr> </tr>
    </thead>
```
On ajoute ensuite des colonnes à ces lignes avec la balise ***th***.
```
    <thead> 
        <tr>
            <th> Colonne 1 </th>
            <th> Colonne 2 </th>
            <th> Colonne 3 </th>
        </tr>
    </thead>
```
Une fois les lignes et colonnes assignés au tableau on va mettre en page le tableau dans la balise ***tableau***.
Cellspacing permet de mettre de l'espace entre les cellules et Cellpadding permet de faire des écarts entre les bords:
```
    <table 
        border="4"
        cellpadding="10"
        cellspacing="4" 
        style="text-align: center"   
    > </table>
```

### Le corps du tableau (tbody)

Il s'agira donc ici de la deuxièle ligne du tableau. On ajoute alors un nouveau ***tr***

```
    <tbody> 
        <tr> 
            <td> Cell 1</td>
            <td> Cell 2</td>
            <td> Cell 3</td>
        </tr>
        <tr> 
            <td> Cell 4</td>
            <td> Cell 5</td>
            <td> Cell 6</td>

        </tr>
    </tbody>
```
Pour donner à une cellule deux cases verticalement il faut dans la balise concernée un ***rowspan***:
```
    <tbody> 
        <tr> 
            <td rowspan="2"> Cell 1</td>
            <td> Cell 2</td>
            <td> Cell 3</td>
        </tr>
        <tr> 
            <td> Cell 4</td>
            <td> Cell 5</td>
            <td> Cell 6</td>

        </tr>
    </tbody>
```
Pour donner à une cellule deux cases horizontalement il faut ajouter dans la balise concernée un ***colspan***:
```
    <tbody> 
        <tr> 
            <td> Cell 1</td>
            <td> Cell 2</td>
            <td> Cell 3</td>
        </tr>
        <tr> 
            <td colspan="2"> Cell 4</td>
            <td> Cell 5</td>
            <td> Cell 6</td>

        </tr>
    </tbody>
```
## Les liens
Pour ajourter des liens
```
<a href="https://htmmlcheatsheet.com">
```
Pour créer un nouvel onglet il faut ajouter dans la balise ***target ="_blank"***
```
<a href="https://htmlcheatsheet.com"
    target="_blank">
```
Pour ajouter une îcone on ajoute la balise ***<i>***:
```
<h2><i>&#8594;</i> Les liens </h2>
```
## Les vidéos

Pour ajouter une vidéo il faut utiliser la balise ***<video></video>*** :
```
<video src="./video.mp4"></video>
```
On peut y ajouter des options ***autoplay*** pour lire automatiquement la vidéo, ***muted*** pour désactiver le son de la vidéo et ***loop*** pour activer la lecture en boucle:

```
<video src="./video.mp4"
        height="200"
        autoplay
        muted
        loop>
</video>
```
## Les images

On utlise la balise ***<img/>*** avec un attribut ***src***.
```
<img src="./image.png">
```
## Les audios

On utilise la balise ***<audio></audio>***
```
<audio controls>
     <source src="sound.mp3" type="audio/mpeg">

</audio>
```
