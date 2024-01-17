En el bloque de importaciones se puede colocar el codigo JavaScript
Los estilos del con el mismo nombre no crean conflicto en los distintos archivos.

npx astro add --help

Los slots son como los children en React

Web para buscar iconos https://tabler.io/icons

Se puede utilizar lenguaje markdown en Astro
Los archivos markdown tambien pueden utilizar layouts y estos se configuran en la cabecera.

(Chequear concepto de content collections)

Se puede hacer fetching de datos utilizando javascript
Las impresiones en consola se hacen en la terminal, ya que Astro no ejecuta codigo javascript en el lado del cliente.

Buscar extension paa que me salgan los console.log en el codigo fuente como ventanas emergentes (SE LLAMA CONSOLE NINJA)

Web para tipar los datos https://app.quicktype.io/

Tambien se pueden crear paginas dinamicas en Astro

Con getstaticpath se pueden pasar las rutas de forma dinamica colocandolas a mano, o llamando a una api externa para recuperarlas todas, pero no es la manera adecuada (Ver minuto 1:19:00) del video. (ESTO SE UTILIZA CUANDO ES UN NUMERO FINITO CONOCIDO DE PRODUCTOS O DE PAGINAS QUE SE DESEAN GENERAR YA QUE ES RAPIDO, SI FUERAN MILLONES, HABRIA PROBLEMAS DE RENDIMIENTO, NO TIENE SENTIDO PARA PAGINAS DINAMICAS).

Lo ideal de manera dinamica es usar SSR (Server Side Rendering)
Esto se activa en el astro.config.mjs en la linea output: 'server',
(Necesita obligatoriamente un servidor para funcionar)

Se puede utilizar output: 'hybrid' y colocar la linea export const prerender=false solamente en las paginas que necesiten hacer uso del servidor

Tambien se puede acceder a cookies y proteger las rutas (Ver minuto 1:26:00) (Solo se puede hacer cuando se utilice el servidor, no es posible en paginas estaticas)

INVESTIGAR VIEW TRANSITION
Importando el componente en el Layout y colocandolo en el head, se aplican transiciones a las paginas y asi simular una SPA

Para utilizar frameworks interactivos se tiene que utilizar "client:visible" en donde se vaya a utilizar el componente mismo

La informacion puede persista la informacion entre paginas con un transition:persist en el componente
