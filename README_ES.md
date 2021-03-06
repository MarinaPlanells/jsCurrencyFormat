jsCurrencyFormat
================

- [Go to english version](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README.md)
- [Anar a la versió catalana](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README_CAT.md)

jsCurrencyFormat, es un plugin que pasándole el 'locale' de un idioma, el número de decimales y si se quiere mostrar el símbolo de la moneda te devuelve el numero contenido en el objeto formateado al tipo de moneda de ese país.

Actualmente soporta el formato para los locales

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

Los códigos para el formato seran los códigos de país de la `ISO 3166-1`

Próximamente se irán añadiendo más paises

Por ejemplo para formatear un número con el formato español sin moneda y a dos decimales, dado este HTML:

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

Si lo quisiéramos en el formato de moneda francesa, mostrando el símbolo de la moneda, bastaría con pasar-le los parámetros del plugin:

```js
    $(document).ready(function(){
        $('.num').currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
    });
```

Actualmente el plugin soporta los siguientes parámetros:

Parámetro | valores | valor por defecto
---------- | ------- | ---------
lang | ISO 3166-1 | es
showCurrency | Boolean | false
decimalsNumber | Int | 2

jsCurrencyFormatter es un plugin de jQuery, asegurate de llamar al archivo de jQuery antes que al de jsCurrencyFormatter

```html
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```
