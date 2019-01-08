# Rédaction de la documentation CSS

## Les conventions à respecter :

### L'indentation :
L'indentation se fait avec 4 espaces

### Le nommage de fichiers :
On essaye de suivre au mieux le nommage BEM (ajouter un lien de documentation sur BEM). Le nom des class et des id se fait en anglais.

La convention de nommage suit ce modèle :

```css
.block{}
.block__element{}
.block--modifieur{}
```

- `.block` représente le niveau supérieur d'une abstraction ou d'un composant.
- `.block__element` représente un descendant de .bloc puisqu'il contribue à former .bloc dans son ensemble.
- `.block--modifieur` représente un état ou une version différente de .block.

Exemple :
```css
.navigation {}
.navigation__right {}
.navigation--hover {}
```
Pour les ancres javascript, préfixer la class par `"js-*"`.

Exemple :
```css
.js-toogle
```


### Le format :
- un seul sélecteur par ligne,
- un espace entre le sélecteur et l'accolade ouvrante,
- pas d'espace entre la propriété et les deux points,
- un espace entre les deux points et la valeur,
- pas d'espace entre la fin de la valeur et le point virgule,
- fermeture d'accolade sur une autre ligne,
- Saut de ligne entre chaque règle.

Exemple :
```css
.selecteur1,
.selecteur2,
.selecteur3 {
  propriete: valeur;
}
```

### Les commentaires : 
D'une manière géréral, éviter les commentaires en fin de ligne. Si la ligne est trop longue, il y a une chance non nulle qu'il ne soit pas vu (en fonction de la taille de l'écran, le réglage de notre éditeur préféré, etc).

Il arrive parfois qu'une partie du css est été pensé pour un style de balise. Par exemple, pour une class `link` on aurait tendance à noter :
```css
a.link {
  color: red;
}
```
Pour éviter de trop cloisonner le code, on va plutôt mettre en commentaire la/les balises les plus adapté pour cette class :
```css
/*a*/.link {
  color: red;
 }
 ```
 
 Ainsi, cela indique clairement quels sont les balises sur lesquelles théoriquement on devrait retrouver ce genre de class, sans pour autant anéantir toute chance de l'appliquer ailleurs.
 

### L'utilisation du !important :

Vous pouvez faire de la prévention en ajoutant !important dans le cas où vous savez que la règle sera **toujours ** prioritaire, par exemple .error {color: red !important;}.

**Utiliser !important pour sortir d'une situation périlleuse n'est pas conseillé**. Dans la mesure du possible, retravaillez votre CSS et essayez de lutter contre ces problèmes en faisant une refacto de vos sélecteurs.

## Guide de style : (A faire pour les 2 thèmes ?)

### Palette de couleurs :

### Les titres :
(donné la police, la taille, la couleur)

h1 : 
h2 : 
h3 : 
h4 :
h5 :
h6 :

### La grille :

### Les breakpoints :

### Les font-icons :

### Les formulaires et les messages d'erreur :

### Les liens et les boutons :

### Les images :

## Les composants CSS :
(recupération de la liste sur la page Design Guidelines de Confluence)
- autocomplete
- dropDown
- contactChip
- infoTip
- lightbox
- multiComboboxes
- searchUser
- sharePanel
- tooltip

