jsCurrencyFormat
================

Scroll down for your language. Available languages: Spanish, English, Catalan.

Spanish
-------

jsCurrencyFormat, es un plugin que pasándole a) el 'locale' de un idioma, y b) si se quiere mostrar el símbolo de la moneda, te devuelve el numero contenido en el objeto formateado al tipo de moneda de ese país.

Actualmente soporta el formato para los locales:

- es
- en
- fr
- de
- it

Próximamente se irán añadiendo más paises.

Por ejemplo para formatear un número con el formato español sin moneda, dado este HTML:

```HTML
<p><span class="num">256984.25</span></p>
<p><input class="num" value="256984.25"/></p>
```

Bastaría con los paramétros por defecto:

```JS
<script>
    $(document).ready(function(){
        $('.num').each(function(){
            $(this).currencyFormatter();
        });
    });
</script>
```

Si lo quisiéramos en el formato de moneda francesa, mostrando el símbolo de la moneda, bastaría con pasarle los dos únicos parámetros del plugin:

```JS
<script>
    $(document).ready(function(){
        $('.num').each(function(){
            $(this).currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
        });
    });
</script>
```

jsCurrencyFormatter es un plugin de jQuery, asegurate de llamar al archivo de jQuery antes que al de jsCurrencyFormatter.

```HTML
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```

English
-------

jsCurrencyFormat, is a plugin to which you can pass a) the 'locale' of a language and b) if you want to show the symbol of the coin, and it returns the number that is contained in the object formatted to the currency of that country.

Currently it supports format for those locales:

- es
- en
- fr
- de
- it

More countries coming soon.

For example, to format a number with the spanish format without currently, given this HTML:

```HTML
<p><span class="num">256984.25</span></p>
<p><input class="num" value="256984.25"/></p>
```

You only need the default parameters:

```JS
<script>
    $(document).ready(function(){
        $('.num').each(function(){
            $(this).currencyFormatter();
        });
    });
</script>
```

If we want it in french currency, showing the currency symbol, it's enough to pass to the plugin the only two parameters it has:

```JS
<script>
    $(document).ready(function(){
        $('.num').each(function(){
            $(this).currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
        });
    });
</script>
```

jsCurrencyFormatter is a jQuery plugin. Make sure to call the jQuery file before the jsCurrencyFormatter file.

```HTML
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```

Catalan
-------

jsCurrencyFormat, és un plugin que passant-li a) el 'locale' d'un idioma, i b) si es vol mostrar el símbol de la moneda, et retorna el nombre contingut en l'objecte formatejat al tipus de moneda d'aquell pais.

Actualment suporta el format pels següents locales:

- es
- en
- fr
- de
- it

Properament s'aniran afegint nous països.

Per exemple per formatejar un nombre amb el format espanyol sense moneda, donat aquest HTML:

```HTML
<p><span class="num">256984.25</span></p>
<p><input class="num" value="256984.25"/></p>
```

N'hi hauria prou amb els paràmetres per defecte:

```JS
<script>
    $(document).ready(function(){
        $('.num').each(function(){
            $(this).currencyFormatter();
        });
    });
</script>
```

So el volem en el format de moneda francesa, mostrant el símbol de la moneda, n'hi hauria prou amb passar-li els dos únics paràmetres del plugin:

```JS
<script>
    $(document).ready(function(){
        $('.num').each(function(){
            $(this).currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
        });
    });
</script>
```

jsCurrencyFormatter és un plugin de jQuery, assegura't de cridar l'arxiu de jQuery abans que al de jsCurrencyFormatter.

```HTML
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```
