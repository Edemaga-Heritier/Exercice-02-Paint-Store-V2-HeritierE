# Instructions - ***⚒️ Exercice #02 - Paint Store***

Pour ce projet, suivez des instructions étape par étape pour améliorer une page Web dynamique et riche en couleurs pour une entreprise de peinture.
<br/>Il affiche des informations sur l'utilisation de la couleur dans une maison et des échantillons de couleurs avec une luminosité, une saturation et une teinte variables.

La page est presque prête à être publiée. Vous allez apporter les modifications suivantes liées aux couleurs :
* Échanger certaines couleurs nommées avec des valeurs de couleur hexadécimales.
* Ajouter des superpositions semi-transparentes à la bannière et au pied de page à l'aide de RGBA.
* Remplir la première colonne de couleur des échantillons d'échantillons en utilisant les couleurs HSL.
Les fichiers de document `index.html` et `style.css` existants du site web sont affichés dans l'éditeur de texte.
## Tâches
1. Dans `style.css`, recherchez les trois règles CSS qui utilisent la couleur nommée `orange`. Cette couleur n'est pas exactement la bonne orange pour correspondre à la marque du magasin de peinture. Remplacez `orange` par la couleur hexadécimale `#ff8000`.
    * La première occurrence de orange est l'arrière-plan de l'en-tête, sous le sélecteur `header`.
    * La deuxième occurrence est la couleur du texte pour le titre "Color Guide", sous le sélecteur `#color-guide h2`.
    * L'occurrence finale est dans le bouton du pied de page, sous le sélecteur `footer .button`.

2. Rendez le texte du titre principal de l'élément `h1` semi-transparent pour qu'il corresponde au thème du texte effrayant. Pour ce faire, définissez la propriété `color` avec `rgba()` pour rendre le texte noir (`0` pour les valeurs rouge, vert et bleu) avec une valeur alpha de `0.7`.
3. Donnez à l'image d'arrière-plan de l'en-tête une superposition `orange` semi-transparente pour simuler un filtre photographique.
Dans le sélecteur `#banner:before`, ajoutez une couleur de fond avec la valeur `rgba(255, 128, 0, 0.75)`.
4. Faites maintenant la même chose pour le pied de page, en ajoutant un calque semi-transparent au-dessus de l'image pour l'adoucir et l'assombrir.
Recherchez le sélecteur `footer:before` et ajoutez une couleur d'arrière-plan avec la même valeur semi-transparente que celle que vous avez utilisée pour l'élément `h1`.
5. Adoucissez les sous-titres qui disent « Saturation », « Luminosité » et « Teinte ». Actuellement, ils sont en noir par défaut.
Ajoutez une propriété à la règle `.color .swatches h4` pour changer la couleur du texte en valeur hexadécimale gris clair `#9b9b9b`.

6. Il y a trois balises `span` qui décrivent la « couleur de base » pour chaque section de couleur. Chacun d'eux relève d'une balise `<div>` avec une classe spécifique à la couleur. Actuellement, toutes ces couleurs de base sont décrites avec des valeurs hexadécimales. Changez-les en HSL.

    <br/>Par exemple, la valeur de la couleur dans la règle `.reds .base-color` est actuellement `#ff002b`. Remplacez-le par la valeur HSL `hsl(350, 100%, 50%)`.
    <br/>Vous pouvez trouver les valeurs de couleur de base pour les sections vertes et bleues dans le texte de la page Web. Mettez-les également à jour avec leur valeur HSL correspondante.
8. Dans chaque section (rouge, verte et bleue), il y a 15 cellules de couleur. Chaque cellule a sa propre règle spécifiant sa couleur dans `style.css`. Notez qu'au début de chaque échantillon de couleur, la première cellule est vide. Trouvez la règle pour chacune des cellules vides et remplissez la valeur `hsl()` qui complète le modèle.
<br/>Par exemple, le premier échantillon vide est `.reds .lightness .color-1`. Dans chaque valeur HSL de cette section, notez que la valeur de luminosité diminue de 15 points de pourcentage. En suivant le modèle, remplissez la valeur de la valeur d'arrière-plan pour cette cellule, `hsl(350, 100%, 80%)`.
<br/>Utilisez les modèles pour chacune des 8 autres rangées et remplissez la cellule manquante pour chaque rangée.
<br/>Dans style.css, il y a un commentaire au-dessus de la règle de chaque cellule vide qui décrit le modèle.

## Plus...

* Rassurez-vous que la dernière ligne de votre balise `<head>` est une balise `<style>` vide. Inclure les lignes suivantes à votre *`index.html`* à l'endroit indiqué comme suit :
    ```
      <!-- Ne pas modifier la ligne qui suit -->
      <style></style>
    ```

* Executez les tests avant de soumettre votre travail.
  
* Une fois soumis ici sur Replit, soumettre sur Google Classroom. L'échec de soumission peut être marqué comme un retard ou comme non fait.
