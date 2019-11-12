# GAMERetro

Le fichier [fonts.css](assets/css/fonts.css) contiend les importations des polices du dossier [fonts](assets/fonts).

Le fichier [index.css](assets/css/index.css) contiend les régles de style.

Ce fichier est composé de trois grandes parties :
1. en-tête
2. le corp
   1. le Tchat principal
   2. l'Info-bulle
3. le pied de page





- ligne 103 on trouve le clip-path qui me permet de faire une forme de bulle de sms pour le Tchat, que je trouve joli, et qui m'a permis de mieux comprendre comment fonctionnait le polygon() de clip-path.
```html
<article>
  <div id="titreContainer">
    <div id="sms"></div>
    <h2>Tchat</h2>
  </div>
  <iframe src="https://gameretro.alwaysdata.net"></iframe>
</article>
```
```css
#sms{
    background-color: red;
    width: 30px;
    height: 30px;
    clip-path: polygon(0 0,100% 0,100% 50%,30% 50%,10% 70%,10% 50%,0 50%);
}
```
