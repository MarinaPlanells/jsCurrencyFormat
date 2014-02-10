jsCurrencyFormat
================

jsCurrencyFormat, es un plugin que pasándole el 'locale' de un idioma, y si se quiere mostrar el símbolo de la moneda te devuelve el numero contenido en el objeto formateado al tipo de moneda de ese país.

Actualmente soporta el formato para los locales

- es
- en
- fr
- de
- it

Próximamente se irán añadiendo más paises

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

Si lo quisiéramos en el formato de moneda francesa, mostrando el símbolo de la moneda, bastaría con pasar-le los dos únicos parámetros del plugin:

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
