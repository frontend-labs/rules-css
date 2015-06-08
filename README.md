#rules-css

Estándares css, para un optimo trabajo en equipo.

####categorías
- Base
- Vista(v)
- Bloque(b)
- Elemento(e)
- Utilidades(u)
- Estado(is_)

####Sintaxis
Se coloca la letra correspondiente a cada categoria '[v]' como prefijo, seguidamente se coloca el nombre que se le asigna utilizando camelCase, 
diferente son los estados que comienzan con un 'is_', seguido de su nombre respectivo.

####Regla de la Base
Una regla base se aplica a los selectores padres, hijos junto a las
pseudo-clases, no se incluye ningun selector de tipo 'clase' o 'ID'.
Dichos estilos son la configuración de inicio.

####Regla de la vista:
La vista es un conjunto de bloques y elementos.

```html
/* teniendo una vista llamada 'help' */
<div class="vHelp">

</div>
```

####Regla del bloque:
Unidad independiente de la aplicación, compuesto por elementos.

```html
/* teniendo un bloque llamado 'search' donde su ambito es la vista 'home' */
<div class="vHome_bSearch">

</div>
```

####Regla del elemento:
Un elemento es parte de un bloque.
Los elementos pueden ser dependientes del ambito para su existencia, 
tambien hay elementos globales la cual no dependeran de su ambito para existir.

Elementos dependientes a su ambito.
```html
<button class="vHome_bRegister_eBtnPrimary">
	
</button>
```
Elementos independientes a un ambito.
```html
<button class="eBtnPrimary">
	
</button>
```

####Regla de la utilidad:
Las utilidades se pueden aplicar directamente en cualquier categoria.
```html
<button class="vHome_bWrapper uClearFix">
	
</button>
```

####Regla de Estado :
Situación temporal de un elemento.

```html
<button class="eBtnPrimary is_disable">
	
</button>
```
