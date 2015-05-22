#rules-css

Estándares css, para un optimo trabajo en equipo.
####categorías
- Base
- Módulo
- Estado

####Regla de la Base
Una regla base se aplica a los selectores padres, hijos junto a las
pseudo-clases, no se incluye ningun selector de tipo 'clase' o 'ID'.
Dichos estilos son la configuración de inicio.

####Regla de el Módulo :
Un módulo tiene un numero de elementos, y no es recomendable usar 'nesting'.
Ejemplos .- Navigation Drawer, carousel, etc.

####Regla de Estado :
Situación temporal de un elemento.

######Ejemplos
- is_disable
-	is_collapsed
-	is_error
-	is_success
```
.navbar.is_collapsed
  background-color tomato
```
