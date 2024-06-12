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
ou
```
(display:"Mon image)
```


Pour des raisons pratiques, ajouter y la balise "image".


#### Modifier le CSS de l'histoire (IMG et SVG)

Pour centrer l'image :\
Il faut ajouter le code CSS suivant dans le CSS général de l'histoire.

```css
/* centre une image basiquement */
img {
    display: block;
    margin: auto;
}

```

#### ASCII Art

Pose des problème à cause de l'interprétation des caractères.\
Même avec les balises "pre".

Il faut donc trouver un autre moyen.
C'est la proposition que je fais avec le projet Twine-ASCII.


#### SVG

Ne fonctionne pas.
Essais en cours.

___
