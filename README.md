#rules-css

Estándares css, para un optimo trabajo en equipo.

####Categorías
[#] | categoria | prefijo
----- | ----- | -----
1|Base| None
2|Vista| v
3|Bloque| b
4|ELemento| e
5|Utilidades| u
6|Estado| is_

####Sintaxis
Se coloca la letra correspondiente a cada categoría como prefijo, seguidamente se coloca el nombre que se le asigna utilizando camelCase,
diferente son los estados que comienzan con un **(is_)**, seguido de su nombre respectivo.

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
Un bloque es parte de una vista y contenedor de uno o más elementos.
Los bloques son dependientes de un ambito para su existencia como tambien son independientes de un ambito cuando nescesitemos reutilizar dicho bloque en otras vistas.

Bloque dependiente de su ambito.
```html
/* teniendo un bloque llamado 'search' donde su ambito es la vista 'home' */
<div class="vHome_bSearch">

</div>
```
Bloque independientes a un ambito.
```html
<div class="bRegister">

</div>
```
####Regla del elemento:
Un elemento es parte de un bloque.
Un elemento al igual que un bloque puede ser dependiente o independiente de un ambito.

Elemento dependiente de su ámbito.
```html
<ul class="bTab">
  <li class="bTab_eItem">
    <a href="#" class="bTab_eTarget is_activeTab">mi tab</a>
  </li>
</ul>
```
Elemento independientes a un ámbito.
```html
<button class="eBtnPrimary">
  mi boton
</button>
```
####Regla de la utilidad:
Las utilidades se pueden aplicar directamente en cualquier clase.
```html
<div class="vHome_bMessage uClearFix">

</div>
```
####Regla de Estado :
Otorga y anula un estilo, dicho estado siempre tiene que estar contiguo a una clase.
Un ejemplo podría ser un tab activo.
```html
<ul class="bTab">
  <li class="bTab_eItem">
    <a href="#" class="bTab_eTarget is_activeTab">mi tab</a>
  </li>
</ul>
```
