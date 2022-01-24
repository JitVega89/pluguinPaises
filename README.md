# pluguinPaises
plugin para wordpress que muestra listado de países de europa por medio de un shortcode **\[vass-wp-countries\]**

Mostrara una lista de paises europeos con el formato -> pais-capital-población -> Ejemplo: **Spain - Madrid - 47,351,567**

Crea un custom post llamado **countries**

## Instalación

1. Debes tener instalado y configurado Wordpress.

2. crear una carpeta de nombre **list-paises** dentro de (Document root)/wordpress/wp-content/plugins/ 

3. Antes de activar el plugin hay que modificar la linea 16 del arhivo **list-paises.php** en el cual hay que poner la ruta absoluta del 

   archivo **wp-load.php** que se encuentra en **wordpress/wp-load.php**

4. Una vez hemos compleado los pasos anteriores, ya podemos activar el plugin de nombre **Países**
5. ahora ya se puede usar el short code en un bloque Shortcode con el nombre **\[vass-wp-countries\]**. Que mostrara una lista de paises europeos

## Insert post y crontab

1. A partir de la linea 110 del arhivo **list-paises.php** esta pensado el código crear post sistematicamente de la información obtenida de la api

pero no he logrado montar correctamente la funcion **wp_insert_post()**

2. Tambien me falta consumir la api por medio de un cron.

ambos puntos faltan implementarlos. Que se implementaran en parches posteriores.
