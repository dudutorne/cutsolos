# cutsolos

cutsolos és una web app per treure solos d'orella (saxo, violí, trompeta, guitarra…). Penges una cançó, tries on és
el solo i l'app el talla en frases que surten com els pads d'un launchpad: les pots escoltar una a una, juntar-ne
unes quantes, repetir-les en bucle i alentir-les sense que canviï el to.

Funciona a l'iPhone, a l'iPad i al Mac des del navegador, i es pot instal·lar com una app que funciona sense connexió.
L'àudio no es puja enlloc: es queda al dispositiu.

Creada per **Edu Torné**. Llicència [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Com s'utilitza

- **Pujar una cançó:** «Tria l'àudio» (MP3, M4A, WAV…). Si és una cançó sencera, primer marques on comença i on acaba
  el solo («El solo comença aquí» / «Acaba aquí», o arrossegant els marcadors).
- **Frases:** l'app segueix la melodia del solista i talla on respira, encara que la banda soni de fons. El control
  **llargues ↔ curtes** tria la llargada de les frases.
- **Pads:**
  - Un toc: sona la frase. Un altre toc: s'atura.
  - Mantén premut i arrossega: tries unes quantes frases seguides, que queden com a grup. Amb el ratolí, n'hi ha prou
    d'arrossegar.
  - Doble toc a qualsevol pad: atura-ho tot i desfà el grup.
  - Triple toc: el grup (o la frase) sona en bucle.
- **Tempo:** −0,15 / +0,15 i «Original». Es pot canviar mentre sona.
- **Barra inferior:** bucle, torna-hi i atura.
- **Editar frases (llapis):** moure l'inici i el final, dividir, unir amb la següent i esborrar. Si sona una frase, el
  llapis l'obre directament. Cada llargada de frase guarda les seves edicions.
- **Mode concentració (quatre quadrats, a dalt a la dreta):** només els pads, grans, per practicar sense mirar el
  mòbil. La pantalla no s'apaga. Per sortir, la creu petita de la cantonada de dalt a l'esquerra.
- **Les meves cançons:** tot es desa al dispositiu (tros del solo, frases, grup, tempo). Toca el nom de la cançó per
  canviar-lo. El logo torna a la llista.

## Instal·lar-la

- **iPhone / iPad:** obre la web amb Safari → Compartir → **Afegeix a la pantalla d'inici**.
- **Mac:** Safari → Fitxer → **Afegeix al Dock**, o a Chrome, la icona d'instal·lar de la barra d'adreces.

## Tecnologia

Un sol fitxer `index.html` amb HTML, CSS i JavaScript, sense dependències. Web Audio per analitzar l'àudio
(detecció de la melodia predominant per suma d'harmònics), IndexedDB per desar les cançons i un service worker
(`sw.js`) perquè funcioni sense connexió.
