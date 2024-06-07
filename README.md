# img2base64

HTML file to transform image to Base64.\
All in French for the moment.

## Installation

Télécharger le fichier puis l'ouvrir dans un navigateur.


## Utilisation

CLiquer sur le bouton pour charger un fichier image.

Apparîtra en-dessous le code img en base 64.

Préférable de petites images.


### Exemple avec Twine

#### Convertir

* Convertisser l'image
* Enregistrer dans un fichier html

#### Insérer l'image dans Twine

Dans votre histoire Twine.
* Créer un nouveau passage
* Nommer votre passage, par exemple "Mon image"
* "Ranger" ce passage dans une zone où vous mettrez toutes les images
* Ajouter une balise de couleur, appeller là "Image" par exemple, ça permet de les distinguer du reste

Ouvrer un passage dans lequel vous voulez mettre l'image.
Mettre le code :

```
(print:"Mon image)
```

Pour des raisons pratiques, ajouter y la balise "image".

#### Remarques

Vous pouvez procéder de même avec :
* des images SVG
* des images ASCII Art

L'ASCII Art c'est du texte, donc prend peut de place.\
Mais le passage conteneur nécessite un peu de travail.

#### Modifier le CSS de l'histoire (IMG et SVG)

Pour centrer l'image :\
Il faut ajouter le code CSS suivant dans le CSS général de l'histoire.

```css
/* centre une image basiquement */
img {
    display: block;
    margin: auto;
}

/* centre un SVG basiquement */
svg {
    display: block;
    margin: auto;
}
```

#### ASCII Art

Dans le passage, il faut du HTML.

```html
<div class="ASCII">
    <pre>

Le code ASCII Art ici

    </pre>
</div>
```
Il faut ajouter le code CSS suivant dans le CSS général de l'histoire.

```css
/* centre l'ASCII */
.ASCII {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
}
/* tag pour l'ASCII */
pre {
    font-family: 'Courier New', monospace;
    white-space: pre;
}
```

NB: pas encore testé.

___