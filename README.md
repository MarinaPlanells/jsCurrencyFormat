jsCurrencyFormat
================

- [Ir a la versión española](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README_ES.md)
- [Anar a la versió catalana](https://github.com/MarinaPlanells/jsCurrencyFormat/blob/master/README_CAT.md)

jsCurrencyFormat is a plugin that converts content in HTML objects to it's currency format using the locale, a Boolean to indicate if you wants to show currency or not and an Int for de number of decimals to show

Right now the plugin supports formats to this country codes:

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

The codes for countries will be based on the `ISO 3166-1`

It will be more country currency formats supported ASAP. You can see the open Issue's to know what countries will come next.

Code example to format a number for spanish currency without the Euro symbol:

```html
<p><span class="num">256984.25</span></p>
<p><input class="num" value="256984.25"/></p>
```

```js
    $(document).ready(function(){
        $('.num').currencyFormatter();
    });
```

But if we want to format the same HTML code to french format with the Euro symbol, we only have to pass this two parameters to the plugin:

```js
    $(document).ready(function(){
        $('.num').currencyFormatter({
                lang: 'fr',
                showCurrency: true
            });
    });
```

Right now the plugin accept this parameters:

Parameter | values | default value
---------- | ------- | ---------
lang | ISO 3166-1 | es
showCurrency | Boolean | false
decimalsNumber | Int | 2

jsCurrencyFormatter is a jQuery plugin, make sure you have the jquery library too.

```html
<script type="text/javascript" src="./js/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./js/currencyFormatter.min.js"></script>
```
