# Luonnontieteiden mallit

Interaktiivisia HTML-malleja kemian ja fysiikan opetukseen. Sivusto julkaistaan GitHub Pagesissa.

## Rakenne

```
index.html          etusivu, jossa on linkit kaikkiin malleihin
mallit/             yksi itsenäinen HTML-tiedosto jokaista mallia kohden
  ioniyhdisteet.html
.nojekyll           kertoo GitHub Pagesille, että tiedostot julkaistaan sellaisenaan
```

## Uuden mallin lisääminen

1. Tallenna malli kansioon `mallit/`, esim. `mallit/heiluri.html`.
2. Lisää mallin alkuun paluulinkki: `<a href="../index.html">← Kaikki mallit</a>`.
3. Lisää `index.html`-tiedoston `MALLIT`-listaan uusi rivi:
   ```js
   {nimi:'Heiluri',aine:'Fysiikka',kurssi:'FY2',kuvaus:'...',url:'mallit/heiluri.html'},
   ```
4. Commitoi ja pushaa. Sivusto päivittyy noin minuutissa.

## GitHub Pagesin käyttöönotto (kerran)

1. Luo GitHubiin uusi **public**-repo, esim. `luonnontiede-mallit`, ja pushaa tämä kansio sinne.
2. Repon asetuksista: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main` ja kansio `/ (root)` → Save.
3. Sivusto löytyy osoitteesta `https://<käyttäjänimi>.github.io/luonnontiede-mallit/`.
