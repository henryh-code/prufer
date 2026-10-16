# Prüfer Industrieofenbau – website

Statische website (HTML, CSS, een beetje JS – geen build-stap). Talen: EN en NL, plus Duitse juridische pagina's.

```
index.html            kiest EN of NL op basis van de browsertaal
en/  nl/              index, company, references, customers, contact
impressum.html        Duits (aanpassen na juridische controle)
datenschutz.html      Duits, nog een plaatshouder
assets/css/style.css  alle stijlen (kleuren bovenaan in :root)
assets/js/main.js     menu, scroll-animatie, contactformulier (mailto)
assets/img/           logo en foto's: allemaal PLAATSHOUDERS
```

Lokaal bekijken: `python3 -m http.server` in deze map en open `http://localhost:8000/`.

## Nog te vervangen
- `assets/img/logo*.svg`, `ph-*.svg` en `favicon.svg`: echte logo en foto's.
- `en|nl/references.html`: inhoud van de oude pagina Referenties.
- `datenschutz.html`: Datenschutzerklärung (de oude `disclaimer.html`).
- `impressum.html`: verwijzing naar MDStV vervangen door de huidige wet (§ 5 DDG / § 18 MStV), juridisch laten controleren.
- Nederlandse teksten zijn een vertaling van de Engelse (machinevertaalde) tekst van de oude site; laten nalopen.
- Klantenlijst is overgenomen zoals op de oude site (o.a. "Kwaniyang", "Pennang", "Poscoe", "Isccor" controleren).
- Contactformulier opent het e-mailprogramma (mailto); geen serverscript.
