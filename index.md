# Rédaction de la documentation CSS

## Les conventions a respecter :

### L'indentation :
L'indentation se fait avec 4 espaces

### Le nommage de fichiers :
On essaye de suivre au mieux le nommage BEM (ajouter un lien de documentation sur BEM).

La convention de nommage suit ce modèle :

```css
.block{}
.block__element{}
.block--modifieur{}
```

`.block` représente le niveau supérieur d'une abstraction ou d'un composant.
`.block__element` représente un descendant de .bloc puisqu'il contribue à former .bloc dans son ensemble.
`.block--modifieur` représente un état ou une version différente de .block.

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
