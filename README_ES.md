jsCurrencyFormat
================

[Go to english version](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README.md)

jsCurrencyFormat, es un plugin que pasándole el 'locale' de un idioma, y si se quiere mostrar el símbolo de la moneda te devuelve el numero contenido en el objeto formateado al tipo de moneda de ese país.

Actualmente soporta el formato para los locales

- es
- uk
- fr
- de
- it

Los códigos para el formato seran los códigos de país de la `ISO 3166-1`

Próximamente se irán añadiendo más paises

Por ejemplo para formatear un número con el formato español sin moneda, dado este HTML:

```html
<p><span class="num">256984.25</span></p>
<p><input class="num" value="256984.25"/></p>
```

Bastaría con los paramétros por defecto:

```js
    $(document).ready(function(){
        $('.num').currencyFormatter();
    });
```

Si lo quisiéramos en el formato de moneda francesa, mostrando el símbolo de la moneda, bastaría con pasar-le los dos únicos parámetros del plugin:

```js
    $(document).ready(function(){
        $('.num').currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
    });
```

jsCurrencyFormatter es un plugin de jQuery, asegurate de llamar al archivo de jQuery antes que al de jsCurrencyFormatter

```html
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```
