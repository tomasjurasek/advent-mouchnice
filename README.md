# Adventní okénka v Mouchnicích

Statická stránka s adventním kalendářem obce. Stačí nahrát na libovolný hosting (GitHub Pages, Netlify, web obce…) – žádný build ani server.

## Soubory

- `index.html` – stránka s mapou, klikacími domečky a modálním oknem
- `okenka.js` – **obsah okének** (nadpis, text, volitelně obrázek) – tady se upravují texty
- `img/mapa.jpg` – obrázek mapy

## Úprava obsahu

V `okenka.js` přepište texty. Text může obsahovat HTML (odkazy, tučné písmo), prázdný řádek dělá nový odstavec. Obrázek přidáte takto:

```js
7: { nadpis: "Rozsvícení stromku", text: "…", obrazek: "img/den7.jpg" },
```

## Chování

- Okénko č. N se odemkne N. prosince (rok nastavíte v `index.html` v konstantě `ROK_ADVENTU`). Zamčené okénko ukáže, kolik dní zbývá.
- Dnešní okénko jemně bliká, otevřená okénka dostanou „nálepku“ (pamatuje si to prohlížeč).
- `index.html?test` odemkne všechna okénka – pro kontrolu obsahu před adventem.
- `index.html#12` rovnou otevře okénko č. 12 (hodí se pro sdílení na Facebooku apod.).
