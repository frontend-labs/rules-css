#rules-css

Estándares css, para un optimo trabajo en equipo.
####categorías
- Base
- Vista(v)
- Bloque(b)
- Elemento(e)
- Modificador(m)
- Utilidades(u)
- Estado(is_)

#####Sintaxis
Se coloca la letra correspondiente a cada categoria '[v]' como prefijo, seguidamente se coloca el nombre que sele asigna.

####Regla de la Base
Una regla base se aplica a los selectores padres, hijos junto a las
pseudo-clases, no se incluye ningun selector de tipo 'clase' o 'ID'.
Dichos estilos son la configuración de inicio.

####Regla de la vista:
La vista es un conjunto de bloques y elementos,

```html
/* teniendo una vista llamada 'help' */
<div class="vHelp">

</div>
```

####Regla del bloque:
Un bloque es un conjunto de elementos independiente
#####Sintaxis
La letra 'b' se coloca como prefijo, seguidamente se coloca el nombre de la vista.
```html
/* teniendo un bloque llamado 'search' */
<div class="bSearch">

</div>
```

####Regla del elemento:
Un elemento es dependiente o independiente de un ambito, dependiendo el escenario.
```css
/**/

```
####Regla de Estado :
Situación temporal de un elemento.

######Ejemplos
- is_disable
-	is_collapsed
-	is_error
-	is_success
```css
.navbar.is_collapsed
  background-color tomato
```
