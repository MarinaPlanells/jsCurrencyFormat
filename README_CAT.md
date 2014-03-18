jsCurrencyFormat
================

[Go to english version](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README.md)
[Ir a la versión española](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README_ES.md)

jsCurrencyFormat és un pugin que converteix el contingut d'objectes HTML al seu format de moneda utilitzant el locale. Un booleà li indica si vols mostrar el símbol de moneda o no.

Els valors per defecte són: `lang = 'es'` i `showCurrency = false`

Actualment el plugin suporta els formats dels següents codis de país:

- es
- uk
- fr
- de
- it
- ie
- be
- lu
- nl
- gr
- de
- us

Els codis dels països es basaràn en l'estàndard `ISO 3166-1`

Aviat suportarà més codis de país. Pots mirar les `Issue's` de github per veure quins seran els propers.

Code d'exemple for formatejar un número a moneda espanyola sense el símbol d'Euro:

```html
<p><span class="num">256984.25</span></p>
<p><input class="num" value="256984.25"/></p>
```

```js
    $(document).ready(function(){
        $('.num').currencyFormatter();
    });
```

Però si volem formatejar el mateix codi HTML al format francès, i amb el símbol de moneda, només cal passar-li un parell de paràmetres al plugin:

```js
    $(document).ready(function(){
        $('.num').currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
    });
```

jsCurrencyFormatter és un plugin de jQuery, assegura't de tenir les llibreries jquery també:

```html
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```
