# GAMERetro

Le fichier [fonts.css](assets/css/fonts.css) contiend les importations des polices du dossier [fonts](assets/fonts).

Le fichier [index.css](assets/css/index.css) contiend les régles de style.

Ce fichier est composé de trois grandes parties :
1. en-tête
2. le corp
   1. le Tchat principal
   2. l'Info-bulle
3. le pied de page





- index.css ligne 103 on trouve le `clip-path` qui me permet de faire une forme de bulle de sms pour le Tchat, que je trouve joli, et qui m'a permis de mieux comprendre comment fonctionnait le `polygon()` de `clip-path`.
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

- index.html ligne 30 on trouve une balise `<marquee></marquee>` qui est une balise dépréciée. Mais elle est cool.
- index.html ligne 39 le tchat est en fait une `<iframe>` d'un site que j'ai hébergé spécialement pour l'occasion. Vous pouvez aller voir [juste ici](https://gameretro.alwaysdata.net).
- index.css ligne [173](https://github.com/lostsh/gameretro/blob/79516f614a8f61f4d7ed9e2a4c1d451f4d445700/assets/css/index.css#L173) a [189](https://github.com/lostsh/gameretro/blob/79516f614a8f61f4d7ed9e2a4c1d451f4d445700/assets/css/index.css#L189) on peut voir le positionnement des images :
```css
#mes_photo table, table tr, table tr td figure{
    margin: 0;
    padding: 0;
}
#mes_photo table tr:nth-child(1) td figure img{
    width: 100%;
}
#mes_photo table tr:nth-child(2) td figure img{
    height: 7em;
}
#Bpacman, #Bspace{
    float: right;
}
#Bgalaga, #Bcentiped{
    float: left;
}
```
