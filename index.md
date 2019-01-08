# Rédaction de la documentation CSS

## Les conventions a respecter :

### L'indentation :
L'indentation se fait avec 4 espaces

### Le nommage de fichiers :
On essaye de suivre au mieux le nommage BEM (ajouter un lien de documentation sur BEM). Le nom des class et des id se fait en anglais.

Pour les class contenant du javascript, préfixer la class par "js-".

Exemple :
```css
.js-toogle
```

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
!important

Il est correct d'utiliser !important sur des classes d'assistance uniquement. Vous pouvez aussi faire de la prévention en ajoutant !important dans le cas où vous savez que la règle sera **toujours ** prioritaire, par exemple .error {color: red !important;}.

**Utiliser !important pour sortir d'une situation périlleuse n'est pas conseillé**. Dans la mesure du possible, retravaillez votre CSS et essayez de lutter contre ces problèmes en réusinant vos sélecteurs. Garder vos sélecteurs courts en évitant les IDS vous aidera énormément.

## Guide de style :
h1 - h2 - h3 
