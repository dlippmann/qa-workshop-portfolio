# Sesión 1
## Charter
Explorar la gestión del carrito de compras en la PetStore, usando cambios de estado y combinaciones de acciones (agregar, eliminar, modificar), para descubrir inconsistencias, pérdida de datos y comportamientos inesperados.
## ÁREAS
Carrito de compras – JPetStore

## INICIO
22/04/2026 – (Duración estimada: 40 minutos)

## TESTER
DAVID LIPPMANN
## DESGLOSE DE TAREAS
*15 min: Agregar productos al carrito en distintos escenarios
*15 min: modificacion de cantidades y eliminacion de articulos
*10 min: navegar en el sistema, validaciones y confirmar la compra
## ARCHIVOS DE DATOS
productos propios de la store
## NOTAS DE PRUEBA
*se realizó el checkout de articulos sin existencias en el stock, el sistema permitio seguir con el prcoceso.
*se realizó el checkout de articulos que superen la cantidad en el stock, el sistema permitio seguir con el prcoceso.
*se forzó el sistema a errores de tipos de datos, el mismo no alerta al usuario sobre los errores
## LISTA DE RIESGOS
*no se notifica al usuario de los cambios en el carrito
*informacion incosistente en el carrito
**mala experiencia del usuario
## DEFECTOS (BUGS)
1*riesgo alto: permite proceder a la compra de articulos sin existencias
2*riesgo alto: permite proceder a la compra de articulos en cantidades que superen las del stock
3*riesgo medio:en caso de agregar un numero negativo en la cantidad el sistema lo borro directamente del carrito, sin alertar al usuario
4*riesgo bajo:en caso de agregar un numero decimal, el sistema lo agrega con numero "1" sin alertar al usuario
## INCIDENTES (ISSUES)
el menú del carrito no opera correctamente