cambios
=========

4.0.0
=====
- Rediseño completo de temas (Core 2019 Light / Dark / Legacy).
- Posibilidad de cambiar el tema automáticamente según la hora.
- En dispositivos móviles, el tema puede cambiar según el brillo (requiere activar * sensor adicional genérico * en cromo, página de cromo:// flags). <br/><br/>
- Mejora y reorganización del menú principal..
- Menú de complementos : La lista de categorías y complementos ahora está ordenada alfabéticamente.
- Menú de herramientas : Adición de un botón para acceder al probador de expresión.
- Menú de herramientas : Adición de un botón para acceder a las variables. <br/><br/>
- Los campos de búsqueda ahora admiten acentos.
- Los campos de búsqueda (panel de control, escenarios, objetos, widgets, interacciones, complementos) ahora están activos cuando se abre la página, lo que le permite escribir una búsqueda directamente.
- Agregue un botón X en los campos de búsqueda para cancelar la búsqueda..
- Durante una búsqueda, la tecla * escape * cancela la búsqueda.
- salpicadero : En el modo de edición, el campo de búsqueda y sus botones están deshabilitados y se arreglan.
- salpicadero : En el modo de edición, un clic en un botón * expandir * a la derecha de los objetos cambia el tamaño de los mosaicos del objeto a la altura del más alto. Ctrl + clic los reduce a la altura del más bajo.
- salpicadero : La ejecución de la orden en un mosaico ahora se indica mediante el botón * actualizar*. Si no hay ninguno en el mosaico, aparecerá durante la ejecución.
- salpicadero : Los mosaicos indican un comando de información (historial, que abrirá la ventana Historial) o acción al pasar el mouse.
- salpicadero : La ventana de historial ahora le permite abrir este historial en Análisis / Historial.
- salpicadero : La ventana de historial conserva su posición / dimensiones cuando se vuelve a abrir otro historial.
- Ventana de configuración de comandos: Ctrl + clic en &quot;Guardar&quot; cierra la ventana después.
- Ventana de configuración del equipo: Ctrl + clic en &quot;Guardar&quot; cierra la ventana después.
- Agregar información de uso al eliminar equipos.
- objetos : Opción agregada para usar colores personalizados.
- objetos : Agregar menú contextual en pestañas (cambio rápido de objeto).
- interacciones : Agregar menú contextual en pestañas (cambio rápido de interacción).
- plugins : Agregar menú contextual en pestañas (cambio rápido de equipo).
- plugins : En la página de administración de complementos, un punto naranja indica complementos no estables.
- Mejoras de tabla con filtro y opción de clasificación.
- Posibilidad de asignar un ícono a una interacción.
- Cada página de Jeedom ahora tiene un título en el idioma de la interfaz (pestaña del navegador).
- Prevención del autocompletado en los campos &#39;Código de acceso&#39;.
- Gestión de funciones * Página anterior / Página siguiente * del navegador. <br/><br/>
- Reproductores : Rediseño del sistema de widgets (menú Herramientas / Reproductores).
- Reproductores : Posibilidad de reemplazar un widget con otro en todos los comandos que lo usan.
- Reproductores : Posibilidad de asignar un widget a múltiples comandos.
- Reproductores : Agregar widget numérico de información horizontal.
- Reproductores : Agregar un widget vertical numérico de información.
- Reproductores : Adición de una brújula de información numérica / widget de viento (gracias @thanaus).
- Reproductores : Agregar un widget de lluvia de información numérica (gracias @thanaus)
- Reproductores : Visualización del widget de obturador de información / acción proporcional al valor. <br/><br/>
- configuración : Mejora y reorganización de pestañas.
- configuración : Se agregaron muchos * consejos sobre herramientas * (ayuda).
- configuración : Agregar un motor de búsqueda.
- configuración : Agregar un botón para vaciar el caché del widget (pestaña Caché).
- configuración : Opción agregada para deshabilitar el caché del widget (pestaña Caché).
- configuración : Capacidad para centrar el contenido de los mosaicos verticalmente (pestaña Interfaz).
- configuración : Adición de un parámetro para la purga global de las historias (Comandos Tab).
- configuración : Cambie de # mensaje # a # asunto # en Configuración / Registros / Mensajes para evitar la duplicación del mensaje.
- configuración : Posibilidad en los resúmenes de agregar una exclusión de los pedidos que no se hayan actualizado durante más de XX minutos (ejemplo para el cálculo de los promedios de temperatura si un sensor no ha elevado nada durante más de 30 minutos, se excluirá del cálculo ) <br/><br/>
- guión : La coloración de los bloques ya no es aleatoria, sino por tipo de bloque..
- guión : Posibilidad mediante Ctrl + clic en el botón * ejecución * para guardarlo, iniciarlo y mostrar el registro (si el nivel de registro no está activado * Ninguno *).
- guión : Confirmación de eliminación de bloque. Ctrl + clic para evitar la confirmación.
- guión : Adición de una función de búsqueda en los bloques de Código. Buscar : Ctrl + F luego Enter, Siguiente resultado : Ctrl + G, resultado anterior : Ctrl + Shift + G
- guión : Capacidad para condensar bloques.
- guión : La acción &#39;Agregar bloque&#39; cambia a la pestaña Escenario si es necesario.
- guión : Nuevas funciones de copiar / pegar en bloque. Ctrl + clic para cortar / reemplazar.
- guión : Ya no se agrega un nuevo bloque al final del escenario, sino después del bloque donde estaba antes de hacer clic, determinado por el último campo en el que hizo clic.
- guión : Implementación de un sistema Deshacer / Rehacer (Ctrl + Shift + Z / Ctrl + Shift + Y).
- guión : Eliminar escenario compartido.
- guión : Mejora de la ventana de gestión de plantillas de escenarios. <br/><br/>
- Análisis / Equipamiento : Adición de un motor de búsqueda (pestaña Baterías, búsqueda de nombres y padres).
- Análisis / Equipamiento : Ahora se puede hacer clic en el área de calendario / días del equipo para acceder directamente al cambio de batería (s).
- Análisis / Equipamiento : Adición de un campo de búsqueda. <br/><br/>
- Centro de actualizaciones : Advertencia en la pestaña &#39;Núcleo y complementos&#39; y / u &#39;Otros&#39; si hay una actualización disponible. Cambie a &#39;Otros&#39; si es necesario.
- Centro de actualizaciones : diferenciación por versión (estable, beta, ...).
- Centro de actualizaciones : Además de una barra de progreso durante la actualización. <br/><br/>
- Resumen de domótica : El historial de eliminación ahora está disponible en una pestaña (Resumen - Historial).
- Resumen de domótica : Revisión completa, posibilidad de ordenar objetos, equipos, pedidos.
- Resumen de domótica : Adición de equipos e ID de pedidos, en pantalla y en búsqueda.
- Resumen de domótica : Exportación CSV de objeto primario, id, equipo y su id, comando.
- Resumen de domótica : Posibilidad de hacer visibles o no uno o más pedidos. <br/><br/>
- diseño : Posibilidad de especificar el orden (posición) de * Diseños * y * Diseños 3D * (Editar, Configurar diseño).
- diseño : Adición de un campo CSS personalizado en los elementos de * diseño*.
- diseño : Desplazamiento de las opciones de visualización en Diseño de la configuración avanzada, en la configuración de visualización de * Diseño*. Esto para simplificar la interfaz y permitir tener diferentes parámetros por * Diseño*.
- diseño : Mover y cambiar el tamaño de los componentes en * Diseño * tiene en cuenta su tamaño, con o sin magnetización. <br/><br/>
- Reducción general (estilos CSS / en línea, refactorización, etc.) y mejoras de rendimiento.
- Elimine Font Awesome 4 para mantener solo Font Awesome 5.
- Actualización de Libs : jquery 3.4.1, CodeMiror 5.46.0, clasificador de tabla 2.31.1.
- Numerosas correcciones de errores.
- Agregar un sistema de configuración masiva (utilizado en la página Equipo para configurar Alertas de comunicaciones en ellos)

>**IMPORTANTE**
>
>Si después de la actualización tiene un error en el tablero, intente reiniciar su caja para que tenga en cuenta las nuevas adiciones de componentes

>**IMPORTANTE**
>
>El complemento de widgets no es compatible con esta versión de Jeedom y ya no será compatible (porque las funciones se han asumido internamente en el núcleo). Más información [aquí] (https://www.jeedom.com/blog/4368-les-widgets-en-v4)

3.3.38
=====

- Se agregó compatibilidad global de Jeedom DNS con conexión a Internet 4G. (Importante : si está utilizando Jeedom DNS y tiene una conexión 4G, debe verificar en la configuración de Jeedom DNS la casilla correspondiente).
- Correcciones ortográficas.
- Arreglo de seguridad

3.3.37
=====

- Correcciones de errores.

3.3.36
=====

- Adición de redondeo en el número de días desde el último cambio de batería.
- Correcciones de errores

3.3.35
=====

- Correcciones de errores.
- Posibilidad de instalar complementos directamente desde el mercado en línea.

3.3.34
=====
- Se corrigió un error que podía evitar que la batería volviera a funcionar
- Corrección de un error en las etiquetas en las interacciones.
- El estado de &quot;tiempo de espera&quot; (no comunicación) del equipo ahora tiene prioridad sobre el estado de advertencia o peligro
- Corrección de errores en las copias de seguridad en la nube


3.3.33
=====

- Correcciones de errores

3.3.32
=====

- Correcciones de errores
- Soporte móvil para controles deslizantes en diseños
- INTELIGENTE : optimización de la gestión de swap

3.3.31
=====

- Correcciones de errores

3.3.30
=====

- Corrección de un error en la visualización de sesiones de usuario.
- Actualización de la documentación
- Eliminación de la actualización de gráficos en tiempo real, luego de numerosos errores reportados
- Corrección de un error que podría impedir la visualización de ciertos registros.
- Corrección de un error en el servicio de monitoreo.
- Corrección de un error en la página &quot;Análisis del equipo&quot;, la fecha de actualización de la batería ahora es correcta
- Mejora de la acción remove_inat en escenarios

3.3.29
=====

- Corrección de la desaparición de la fecha de la última verificación de actualizaciones
- Se corrigió un error que podía bloquear las copias de seguridad en la nube
- Corrección de un error en el cálculo del uso de las variables si es de forma variable (toto, mavaleur)

3.3.28
=====

- Se corrigió un error de rueda infinita en la página de actualizaciones
- Varias correcciones y optimizaciones.

3.3.27
=====

- Corrección de un error en la traducción de los días en francés.
- Estabilidad mejorada (reinicio automático del servicio MySql y watchdog para verificar la hora de inicio)
- Correcciones de errores
- Deshabilitar acciones en pedidos al editar diseños, vistas o paneles

3.3.26
=====

- Correcciones de errores
- Corrección de un error en el lanzamiento múltiple del escenario
- Corrección de un error en las alertas sobre el valor de los pedidos.

3.3.25
=====
- Corrección de errores
- Cambiar la línea de tiempo al modo de tabla (debido a errores en la biblioteca independiente de Jeedom)
- Adición de clases para soportes de color en el complemento de modo

3.3.24
=====
-   Corrección de un error en la pantalla del número de actualización.
-	Se eliminó la edición del código html de la configuración avanzada de comandos debido a demasiados errores
-	Correcciones de errores
-	Mejora de la ventana de selección de iconos.
-	Actualización automática de la fecha de cambio de batería si la batería es más del 90% y 10% más alta que el valor anterior
-	Adición de un botón en la administración para restablecer los derechos y lanzar una verificación de Jeedom (derecha, cron, base de datos ...)
-	Eliminación de opciones de visibilidad avanzadas para equipos en el tablero de instrumentos / vista / diseño / móvil. Ahora, si desea ver o no el equipo en el tablero de instrumentos / móvil, simplemente marque o no la casilla de visibilidad general. Para vistas y diseño, simplemente coloque o no el equipo en él

3.3.22
=====
- Correcciones de errores
- Reemplazo de pedidos mejorado (en vistas, plan y plan3d)
- Se corrigió un error que podía evitar abrir ciertos equipos de complemento (alarma o tipo virtual)

3.3.21
=====
- Se corrigió un error por el cual la visualización de la hora podía exceder las 24 h
- Corrección de un error en la actualización de los resúmenes de diseño.
- Corrección de un error en la gestión de los niveles de alertas en ciertos widgets durante la actualización del valor
- Se corrigió la visualización del equipo desactivado en algunos complementos
- Corrección de un error al indicar el cambio de batería en Jeedom
- Visualización mejorada de registros al actualizar Jeedom
- Corrección de errores al actualizar una variable (que no siempre iniciaba los escenarios o no activaba una actualización de los comandos en todos los casos)
- Se corrigió un error en las copias de seguridad de la nube, o la duplicidad no se instalaba correctamente
- Mejora de TTS interno en Jeedom
- Mejora del sistema de verificación de sintaxis cron


3.3.20
=====
- Corrección de un error en los escenarios o podrían permanecer bloqueados en &quot;en progreso&quot; mientras están desactivados
- Se solucionó un problema con el lanzamiento de un escenario no planificado
- Corrección de errores de zona horaria

3.3.19
=====
- Corrección de errores (especialmente durante la actualización)


3.3.18
=====
- Correcciones de errores

3.3.17
=====
- Corrección de un error en las copias de seguridad de samba

3.3.16
=====
- Posibilidad de eliminar una variable.
- Adición de una pantalla 3D (beta)
- Rediseño del sistema de respaldo en la nube (respaldo incremental y encriptado).
- Agregar un sistema integrado de toma de notas (en Análisis -&gt; Nota).
- Adición de la noción de etiqueta en el equipo (se puede encontrar en la configuración avanzada del equipo).
- Adición de un sistema de historial sobre la eliminación de pedidos, equipos, objetos, vista, diseño, diseño 3D, escenario y usuario..
- Adición de la acción jeedom_reboot para iniciar un reinicio de Jeedom.
- Agregar opción en la ventana de generación cron.
- Ahora se agrega un mensaje si se encuentra una expresión no válida al ejecutar un escenario.
- Agregar un comando en los escenarios : value (orden) permite tener el valor de una orden si no está dada automáticamente por jeedom (caso cuando se almacena el nombre de la orden en una variable).
- Adición de un botón para actualizar los mensajes del centro de mensajes..
- Agregue en la configuración de la acción sobre el valor de un comando un botón para buscar una acción interna (escenario, pausa ...).
- Adición de una acción &quot;Restablecer a cero del IS&quot; en los escenarios
- Posibilidad de agregar imágenes en segundo plano en las vistas
- Posibilidad de agregar imágenes de fondo en objetos
- La información de actualización disponible ahora está oculta para usuarios no administradores
- Soporte mejorado para () en el cálculo de expresiones
- Posibilidad de editar los escenarios en modo texto / json
- Además en la página de salud de una verificación de espacio libre para el tmp Jeedom
- Posibilidad de agregar opciones en informes
- Adición de un latido por complemento y reinicio automático de daemon en caso de problemas
- Adición de oyentes en la página del motor de tareas
- optimizaciones
- Posibilidad de consultar los registros en versión móvil (wepapp)
- Adición de una etiqueta de acción en los escenarios (ver documentación)
- Posibilidad de tener una vista de pantalla completa agregando &quot;&amp; fullscreen = 1&quot; en la url
- Adición de la última comunicación en los escenarios (para tener la última fecha de comunicación de un equipo)
- Actualización en tiempo real de gráficos (simple, no calculado o líneas de tiempo)
- Posibilidad de eliminar un elemento de la configuración de diseño.
- Posibilidad de tener un informe sobre el nivel de la batería (informe del equipo)
- Los widgets de escenario ahora se muestran por defecto en el tablero
- Cambie el tono de los widgets por horizontal 25 a 40, vertical 5 a 20 y margen 1 a 4 (puede restablecer los valores anteriores en la configuración de jeedom, pestaña widget)
- Posibilidad de poner un icono en los escenarios.
- Visualización de widgets móviles en una sola columna.
- Incorporación de la gestión de demonios en el motor de tareas.
- Adición de la función color_gradient en los escenarios.

3.2.16
=====
- Corrección de un error al instalar dependencias de ciertos complementos en Smart

3.2.15
=====
- Corrección de un error al guardar el equipo.

3.2.14
=====
- Preparación para evitar un error al cambiar a 3.3.X
- Corrección de un problema al solicitar soporte para complementos de terceros

3.2.12
=====
- Correcciones de errores
- optimizaciones

3.2.11
=====
- Correcciones de errores.

3.2.10
=====
- Correcciones de errores.
- Sincronización mejorada con el mercado.
- Mejora del proceso de actualización en particular en la copia de archivos que ahora comprueba el tamaño del archivo copiado.
- Corrección de errores en las funciones stateDuration, lastStateDuration y lastChangeStateDuration (gracias @kiboost).
- Optimización del cálculo del gráfico de enlaces y el uso de variables..
- Mejora de la ventana de detalles de la tarea cron que ahora muestra el escenario, así como la acción a realizar para las tareas doIn (gracias @kiboost).

3.2.9
=====
- Correcciones de errores
- Corrección de un error en los íconos del editor de archivos y en el probador de expresiones
- Corrección de errores en los oyentes.
- Adición de una alerta si un complemento bloquea crons
- Corrección de un error en el sistema de monitoreo en la nube si la versión del agente es inferior a 3.XX

3.2.8
=====
- Correcciones de errores
- Adición de una opción en la administración de Jeedom para especificar el rango de ip local (útil en instalaciones de tipo docker)
- Corrección de un error en el cálculo del uso de variables.
- Adición de un indicador en la página de salud que indica el número de procesos que se matan por falta de memoria (en general indica que la libertad está demasiado cargada)
- Editor de archivos mejorado

3.2.7
=====
- Correcciones de errores
- Actualización de documentos
- Posibilidad de usar las etiquetas en las condiciones de los bloques &quot;A&quot; e &quot;IN&quot;
- Corrección de errores de categorías de mercado para widgets / scripts / escenarios...

3.2.6
=====
- Correcciones de errores
- Actualización de documentos
- Estandarización de los nombres de ciertos pedidos en los escenarios.
- Optimización del rendimiento

3.2.5
=====
- Correcciones de errores
- Reactivación de interacciones (inactivo debido a la actualización)

3.2.4
=====
- Correcciones de errores
- Corrección de un error en cierto modal en español
- Corrección de un error de cálculo en time_diff
- Preparación para el futuro sistema de alerta.

3.2.3
=====
- Corrección de errores en funciones mín. / Máx.....
- Exportación mejorada de gráficos y visualización en modo tabla

3.2.2
=====
- Eliminación del antiguo sistema de actualización de widgets (en desuso desde la versión 3.0). Atención, si su widget no utiliza el nuevo sistema, existe el riesgo de mal funcionamiento (duplicación del mismo en este caso). Ejemplo de widget [aquí] (https://github.com/jeedom/core/tree/beta/core/template/dashboard)
- Posibilidad de mostrar los gráficos en forma de tabla o exportarlos en csv o xls
- Los usuarios ahora pueden agregar su propia función php para escenarios. Ver documentación de escenarios para implementación
- JEED-417 : adición de una función time_diff en los escenarios
- Adición de un retraso configurable antes de la respuesta en las interacciones (permite esperar a que se produzca la retroalimentación de estado, por ejemplo)
- JEED-365 : Eliminación del &quot;comando de información del usuario&quot; para ser reemplazado por acciones en el mensaje. Le permite iniciar varios comandos diferentes, iniciar un escenario ... Atención, si tenía un &quot;comando de información del usuario&quot;, debe reconfigurarse.
- Agregue una opción para abrir fácilmente un acceso al soporte (en la página del usuario y al abrir un ticket)
- Corrección de un error de derechos después de la restauración de una copia de seguridad
- Actualizando traducciones
- Actualización de la biblioteca (jquery y highcharts)
- Posibilidad de prohibir un pedido en interacciones automáticas
- Interacciones automáticas mejoradas
- Corrección de errores en el manejo de sinónimos de interacciones
- Adición de un campo de búsqueda de usuario para conexiones LDAP / AD (hace que Jeedom AD sea compatible)
- Correcciones ortográficas (gracias a dab0u por su enorme trabajo)
- JEED-290 : Ya no podemos conectarnos con los identificadores predeterminados (admin / admin) de forma remota, solo la red local está autorizada
- JEED-186 : Ahora podemos elegir el color de fondo en los diseños
- Para el bloque A, posibilidad de poner una hora entre las 12:01 a.m. y las 12:59 a.m. simplemente poniendo los minutos (ex 30 para las 12:30 a.m.)
- Agregar sesiones activas y dispositivos registrados a la página de perfil de usuario y a la página de administración de usuarios
- JEED-284 : la conexión permanente ahora depende de un usuario único y una clave periférica (y ya no ese usuario)
- JEED-283 : agregando un modo * rescue * a jeedom agregando &amp; rescue = 1 en la url
- JEED-8 : adición del nombre del escenario en el título de la página durante la edición
- Optimización de los cambios organizacionales (tamaño de los widgets, posición del equipo, posición de los comandos) en el tablero y las vistas. Tenga en cuenta ahora que las modificaciones solo se guardan al salir del modo de edición.
- JEED-18 : Agregar registros al abrir un ticket para admitir
- JEED-181 : adición de un comando de nombre en los escenarios para tener el nombre del comando o del equipo u objeto
- JEED-15 : Agregue batería y alerta en la aplicación web
- Corrección de errores para mover objetos de diseño en Firefox
- JEED-19 : Durante una actualización, ahora es posible actualizar el script de actualización antes de la actualización
- JEED-125 : enlace agregado a la documentación de restablecimiento de contraseña
- JEED-2 : Gestión del tiempo mejorada durante un reinicio
- JEED-77 : Adición de gestión de variables en la API http
- JEED-78 : adición de la función de etiqueta para escenarios. Tenga en cuenta que en escenarios que usan etiquetas, cambie de \ #montag \ # a etiqueta (montag)
- JEED-124 : Corregir la gestión de los tiempos de espera del escenario.
- Correcciones de errores
- Capacidad para desactivar una interacción.
- Agregar un editor de archivos (reservado para usuarios experimentados)
- Adición de genéricos Tipos &quot;Luz de estado&quot; (binario), &quot;Temperatura de color de luz&quot; (Información), &quot;Temperatura de color de luz&quot; (Acción)
- Capacidad para hacer que las palabras sean obligatorias en una interacción.

3.1.7
=====
- Corrección de errores (especialmente en historiales y funciones estadísticas)
- Mejora del sistema de actualización con una página de notas de la versión (que debe verificar usted mismo antes de cada actualización
    día !!!!)
- Corrección de un error que recuperó los registros durante las restauraciones.

3.1
===
- Correcciones de errores
- Optimización global de Jeedom (al cargar clases de complementos, tiempo casi dividido por 3)
- Soporte de Debian 9
- Modo de una página (cambio de página sin volver a cargar toda la página, solo la parte que cambia)
- Adición de una opción para ocultar los objetos en el tablero, pero que permite tenerlos siempre en la lista.
- Al hacer doble clic en un nodo en el gráfico de enlace (a excepción de las variables), aparece su página de configuración
- Posibilidad de colocar texto a la izquierda / derecha / centro en diseños para texto / vista / elementos de diseño
- Agregar resúmenes de objetos en el tablero (lista de objetos a la izquierda)
- Adición de interacciones &quot;prevent-me-if&quot;
- Revisión de la página de inicio del escenario
- Agregar un historial de comandos para SQL o comandos del sistema en la interfaz Jeedom
- Posibilidad de tener las gráficas de historias de pedidos en la aplicación web (presionando prolongadamente el pedido)
- Adición del progreso de la actualización de la aplicación web
- Recuperación en caso de error de actualización de la aplicación web
- Eliminación de escenarios &quot;simples&quot; (redundante con configuración avanzada de comandos)
- Agregue sombreado en gráficos para distinguir días
- Rediseño de la página de interacciones.
- Rediseño de la página de perfil
- Rediseño de la página de administración.
- Agregar una &quot;salud&quot; en los objetos
- Corrección de errores en el nivel de batería del equipo.
- Adición de un método en el núcleo para la gestión de comandos muertos (luego debe implementarse en el complemento)
- Posibilidad de registrar comandos de texto
- En la página de historial ahora puede graficar un cálculo
- Agregar una gestión de fórmulas de cálculo para historiales
- Actualización de toda la documentación. :
    - Todos los documentos han sido revisados
    - Eliminación de imágenes para facilitar la actualización y
        plurilingüe
- Más opciones posibles para configurar los tamaños de área en las vistas
- Posibilidad de elegir el color del texto del resumen del objeto
- Adición de una acción remove \ _inat en los escenarios que permite cancelar toda la programación de los bloques DANS / A
- Capacidad en los diseños de widgets al pasar el mouse para elegir la posición del widget
- Agregar un parámetro de respuesta \ _cmd en las interacciones para especificar la identificación del comando que se usará para responder
- Agregar una línea de tiempo en la página del historial (se debe activar la atención en cada comando y / o escenario que desee que aparezca)
- Posibilidad de vaciar los eventos de la línea de tiempo.
- Posibilidad de vaciar las IP prohibidas
- Corrección / mejora de la gestión de cuentas de usuario
    - Posibilidad de eliminar una cuenta de administrador básica
    - Evitar que el último administrador vuelva a la normalidad
    - Se agregó seguridad para evitar la eliminación de la cuenta con la que estamos conectados
- Posibilidad en la configuración avanzada del equipo de poner las órdenes en los widgets en modo tabla eligiendo la casilla para cada orden o poniéndola
- Posibilidad de reorganizar los widgets de equipo desde el tablero (en modo de edición, haga clic derecho en el widget)
- Cambiar el tono de los widgets (de 40 \ * 80 a 10 \ * 10). Tenga en cuenta que esto afectará el diseño en su tablero / vista / diseño
- Posibilidad de dar un tamaño de 1 a 12 a los objetos en el tablero
- Posibilidad de iniciar de forma independiente las acciones de los escenarios (y el modo de tipo de complemento / alarma si es compatible) en paralelo con los demás
- Posibilidad de agregar un código de acceso a un diseño
- Adición de un perro guardián independiente de Jeedom para verificar el estado de MySql y Apache

3.0.11
======
- Se corrigieron errores en las solicitudes de &quot;tiempo de espera&quot;

3.0.10
======
- Corrección de errores en la interfaz para configurar interacciones

3.0
===
- Supresión del modo esclavo
- Posibilidad de desencadenar un escenario en un cambio de una variable
- Las actualizaciones variables ahora activan la actualización de los comandos del equipo virtual (se requiere la última versión del complemento)
- Posibilidad de tener un icono en los comandos de tipo de información
- Habilidad en los comandos para mostrar el nombre y el ícono
- Adición de una acción &quot;alerta&quot; sobre escenarios : mensaje en libertad
- Adición de una acción &quot;emergente&quot; en escenarios : mensaje para validar
- Los widgets de comandos ahora pueden tener un método de actualización que evita una llamada ajax a Jeedom
- Los widgets de escenario ahora se actualizan sin llamadas ajax para obtener el widget
- El resumen global y las partes ahora se actualizan sin una llamada ajax
- Un clic en un elemento de un resumen de automatización del hogar lo lleva a una vista detallada del mismo.
- Ahora puede poner comandos de tipo de texto en los resúmenes
- Cambio del control deslizante bootstraps a control deslizante (corrección del error del evento de controles deslizantes dobles)
- Guardado automático de vistas al hacer clic en el botón &quot;ver resultado&quot;
- Posibilidad de tener los documentos localmente
- Los desarrolladores externos pueden agregar su propio sistema de administración de tickets
- Rediseño de la configuración de derechos de usuario (todo está en la página de administración de usuarios)
- Actualización de Libs : jquery (en 3.0), jquery mobile, hightstock y clasificador de tablas, font-awesome
- Gran mejora en los diseños.:
    - Ahora se puede acceder a todas las acciones desde un
        clic derecho
    - Posibilidad de agregar un solo pedido
    - Posibilidad de agregar una imagen o secuencia de video
    - Posibilidad de agregar zonas (ubicación en la que se puede hacer clic) :
        - Área de tipo macro : lanzar una serie de acciones al hacer clic
        - Área de tipo binario : inicia una serie de acciones cuando se hace clic en ellas según el estado de un pedido
        - Área de tipo de widget : muestra un widget al hacer clic o al pasar el mouse sobre el área
    - Optimización general de código
    - Posibilidad de mostrar una cuadrícula y elegir su tamaño (10x10,15x15 o 30x30)
    - Posibilidad de activar una magnetización de los widgets en la cuadrícula
    - Posibilidad de activar una magnetización de los widgets entre ellos.
    - Ciertos tipos de widgets ahora se pueden duplicar
    - Posibilidad de bloquear un artículo
- Los complementos ahora pueden usar su propia clave API
- Al agregar interacciones automáticas, Jeedom intentará comprender la oración, ejecutar la acción y responder
- Se agregó administración de demonios en la versión móvil
- Adición de gestión cron en versión móvil
- Adición de cierta información de salud en la versión móvil
- Agregar módulos en alerta a la página de la batería
- Los objetos sin widget se ocultan automáticamente en el tablero
- Adición de un botón en la configuración avanzada de un dispositivo / comando para ver sus eventos
- Los disparadores de escenarios ahora pueden ser condiciones
- Un doble clic en la línea de comando (en la página de configuración) ahora abre su configuración avanzada
- Posibilidad de prohibir ciertos valores para un pedido (en su configuración avanzada)
- Adición de campos de configuración en la retroalimentación de estado automática (por ejemplo, volver a 0 después de 4 min) en la configuración avanzada de un comando
- Agregar una función valueDate en escenarios (ver documentación de escenarios)
- Posibilidad en los escenarios de modificar el valor de un pedido con la acción &quot;evento&quot;
- Adición de un campo de comentario sobre la configuración avanzada de un dispositivo
- Adición de un sistema de alerta en pedidos de 2 niveles. : alerta y peligro. La configuración está en la configuración avanzada de comandos (tipo de información, por supuesto). Puede ver los módulos en alerta en la página Análisis → Equipo. Puede configurar las acciones en alerta en la página de configuración general de Jeedom
- Adición de un área de &quot;tabla&quot; en las vistas que permite mostrar una o más columnas por cuadro. Los cuadros también admiten código HTML
- Jeedom ahora puede ejecutarse sin derechos de root (experimental). Tenga cuidado porque sin derechos de root tendrá que ejecutar manualmente los scripts para las dependencias de complementos
- Optimización de los cálculos de expresión (cálculo de etiquetas solo si está presente en la expresión)
- Adición en la función API para acceder al resumen (global y objeto)
- Capacidad para restringir el acceso a cada clave API basada en IP
- Posibilidad en la historia de hacer agrupaciones por hora o año.
- El tiempo de espera en el comando de espera ahora puede ser un cálculo
- Corrección de un error si hay &quot;en los parámetros de una acción
- Cambie a sha512 para el hash de contraseña (se compromete sha1)
- Se corrigió un error en la administración de la memoria caché que lo hacía crecer indefinidamente
- Corrección del acceso al documento de complementos de terceros si no tienen un documento local
- Las interacciones pueden tener en cuenta la noción de contexto (dependiendo de la solicitud anterior y de la anterior)
- Posibilidad de ponderar palabras según su tamaño para el análisis de la comprensión.
- Los complementos ahora pueden agregar interacciones
- Las interacciones ahora pueden devolver archivos además de la respuesta
- Posibilidad de ver en la página de configuración de complementos las funcionalidades de estos complementos (interactuar, cron ...) y desactivarlos individualmente
- Las interacciones automáticas pueden devolver valores de resúmenes
- Capacidad para definir sinónimos de objetos, equipos, comandos y resúmenes que se utilizarán en respuestas contextuales y resúmenes
- Jeedom sabe cómo gestionar varias interacciones relacionadas (contextualmente) en una. Deben estar separados por una palabra clave (por defecto y). ejemplo : &quot;¿Cuánto está haciendo en el dormitorio y en la sala de estar?&quot; o &quot;Encienda la luz en la cocina y el dormitorio&quot;.
- El estado de los escenarios en la página de edición ahora se actualiza dinámicamente
- Posibilidad de exportar una vista en PDF, PNG, SVG o JPEG con el comando &quot;informe&quot; en un escenario
- Posibilidad de exportar un diseño en PDF, PNG, SVG o JPEG con el comando &quot;informe&quot; en un escenario
- Posibilidad de exportar un panel de un complemento en PDF, PNG, SVG o JPEG con el comando &quot;informe&quot; en un escenario
- Agregar una página de administración de informes (para volver a descargarlos o eliminarlos)
- Corrección de un error en la fecha del último informe de un evento para ciertos complementos (alarma)
- Error de pantalla fijo con Chrome 55
- Optimización de la copia de seguridad (en un RPi2 el tiempo se divide por 2)
- Optimización de catering
- Optimización del proceso de actualización.
- Estandarización de tmp jeedom, ahora todo está en / tmp / jeedom
- Posibilidad de tener un gráfico de los diferentes enlaces de un escenario, equipo, objeto, comando o variable
- Posibilidad de ajustar la profundidad de los gráficos del enlace de acuerdo con el objeto original
- Posibilidad de tener registros de escenarios en tiempo real (ralentiza la ejecución de escenarios)
- Capacidad para pasar etiquetas al iniciar un escenario
- Optimización de la carga de escenarios y páginas mediante acciones con opción (configuración de tipo del complemento o modo de alarma)

2.4.6
=====
- Manejo mejorado de los valores de pedido repetido

2.4.5
=====
- Correcciones de errores
- Comprobación de actualizaciones optimizada

2.4
---
- Optimización general
    - Agrupación de consultas SQL
    - Eliminar solicitudes innecesarias
    - Almacenamiento en caché de Pid, estado y último lanzamiento de escenarios
    - Almacenamiento en caché de Pid, estado y último lanzamiento de crons
    - En el 99% de los casos, más solicitudes de escritura en la base en operación nominal (por lo tanto, excepto la configuración de Jeedom, modificaciones, instalación, actualización ...)
- Eliminación de fail2ban (porque se omite fácilmente al enviar una dirección IP falsa), esto hace que Jeedom sea más rápido
- Adición en las interacciones de una opción sin categoría para que uno pueda generar interacciones en equipos sin categoría
- Adición en los escenarios de un botón de elección de equipo en los comandos de tipo deslizante
- Actualización de Bootstrap en 2.3.7
- Adición de la noción de resumen de automatización del hogar (permite saber de inmediato la cantidad de luces encendidas, las puertas abiertas, las persianas, las ventanas, la energía, las detecciones de movimiento ...). Todo esto está configurado en la página de gestión de objetos.
- Agregar pedidos previos y posteriores a un pedido. Le permite activar una acción antes o después de otra acción.. También puede permitir que el equipo se sincronice para que, por ejemplo, 2 luces siempre se enciendan juntas con la misma intensidad.
- Optimización de escucha
- Adición de modal para mostrar la información en bruto (atributo del objeto en la base) de un equipo o un pedido
- Posibilidad de copiar el historial de un pedido a otro pedido
- Posibilidad de reemplazar una orden con otra en todo Jeedom (incluso si la orden a reemplazar ya no existe)

2.3
---
- Corrección de filtros en el mercado.
- Corrección de casillas de verificación en la página de edición de vista (en un área gráfica)
- Corrección del historial de casillas de verificación, visible e inverso en la tabla de comandos
- Corrección de un problema con la traducción de javascripts
- Agregar una categoría de complemento : objeto comunicante
- Agregar GENERIC \ _TYPE
- Eliminación de filtros nuevos y superiores en la ruta del mercado de complementos
- Cambiar el nombre de la categoría predeterminada en la ruta de complementos del mercado a &quot;Superior y nuevo&quot;
- Corrección de filtros gratuitos y de pago en la ruta del mercado de complementos
- Corrección de un error que podría conducir a una duplicación de las curvas en la página del historial.
- Corrección de un error en el tiempo de espera de los escenarios.
- corrección de un error en la visualización de widgets en las vistas que tomaron la versión del tablero
- Corrección de un error en los diseños que podría utilizar la configuración de los widgets del tablero en lugar de los diseños.
- Corrección de errores de copia de seguridad / restauración si el nombre de la libertad contiene caracteres especiales
- Optimización de la organización de la lista de tipos genéricos.
- Visualización mejorada de la configuración avanzada del equipo.
- Corrección de la interfaz de acceso de respaldo desde
- Guardar la configuración durante la prueba de mercado
- Preparación para la eliminación de bootstrapswtich en complementos
- Corrección de un error en el tipo de widget solicitado para los diseños (panel en lugar de dplan)
- corrección de errores en el controlador de eventos
- Cambio aleatorio de la copia de seguridad por la noche (entre 2h10 y 3h59) para evitar preocupaciones de sobrecarga del mercado
- Fix widget market
- Corrección de un error en el acceso al mercado (tiempo de espera)
- Corrección de un error en la apertura de entradas.
- Corrección de un error de página en blanco durante la actualización si / tmp es demasiado pequeño (tenga cuidado de que la corrección surta efecto en la actualización n + 1)
- Adición de una etiqueta * jeedom \ _name * en los escenarios (da el nombre de la libertad)
- Correcciones de errores
- Mover todos los archivos temporales a / tmp
- Envío mejorado de complementos (dos2unix automático en archivos \ *. Sh)
- Rediseño de la página de registro.
- Agregar un tema darksobre para dispositivos móviles
- Capacidad para que los desarrolladores agreguen opciones de configuración de widgets en widgets específicos (sonos, koubachi y otros)
- Optimización de registros (gracias @ kwizer15)
- Posibilidad de elegir el formato de registro
- Diversas optimizaciones del código (gracias @ kwizer15)
- Pasaje en módulo de la conexión con el mercado (permitirá tener libertad sin ningún enlace al mercado)
- Agregar un archivo &quot;repo&quot; (módulo de conexión como la conexión con el mercado) (permite enviar un zip que contiene el complemento)
- Adición de un &quot;repositorio&quot; de github (permite usar github como fuente de complemento, con sistema de gestión de actualizaciones)
- Adición de un URL &quot;repositorio&quot; (permite usar URL como fuente del complemento)
- Adición de un &quot;repositorio&quot; de Samba (utilizable para enviar copias de seguridad en un servidor de samba y recuperar complementos)
- Adición de un &quot;repositorio&quot; FTP (utilizable para enviar copias de seguridad en un servidor FTP y recuperar complementos)
- Adición para cierto &quot;repositorio&quot; de la posibilidad de recuperar el núcleo de la libertad
- Agregar pruebas de código automáticas (gracias @ kwizer15)
- Posibilidad de mostrar / ocultar paneles de complementos en dispositivos móviles o de escritorio (tenga cuidado ahora de forma predeterminada, los paneles están ocultos)
- Posibilidad de deshabilitar las actualizaciones de complementos (así como la verificación)
- Capacidad para forzar la versificación de actualizaciones de complementos
- Ligero rediseño del centro de actualizaciones
- Posibilidad de desactivar la búsqueda automática de actualizaciones
- Se corrigió un error que restablecía todos los datos a 0 después de un reinicio
- Capacidad para configurar el nivel de registro de un complemento directamente en la página de configuración del complemento
- Posibilidad de consultar los registros de un complemento directamente en la página de configuración de este
- Supresión del inicio de depuración de demonios, ahora el nivel de registro del demonio es el mismo que el del complemento
- Limpieza de terceros de Lib
- Supresión de la voz receptiva (función dicha en los escenarios que funcionaban cada vez menos)
- Se corrigieron varias vulnerabilidades de seguridad
- Adición de un modo síncrono en los escenarios (anteriormente modo rápido)
- Posibilidad de ingresar manualmente la posición de los widgets en% en los diseños
- Rediseño de la página de configuración de complementos
- Capacidad para configurar la transparencia de los widgets.
- Se agregó la acción jeedom \ _poweroff en escenarios para detener la libertad
- Retorno del escenario de acción \ _retorno para volver a una interacción (u otra) desde un escenario
- Pasando por encuestas largas para actualizar la interfaz en tiempo real
- Corrección de un error durante la actualización de varios widgets
- Optimización de la actualización de widgets de comando y equipo
- Adición de una etiqueta * begin \ _backup *, * end \ _backup *, * begin \ _update *, * end \ _update *, * begin \ _restore *, * end \ _restore * en los escenarios

2.2
---
- Correcciones de errores
- Simplificación del acceso a configuraciones de complementos desde la página de salud
- Adición de un icono que indica si el demonio se inicia en depuración o no
- Adición de una página de configuración del historial global (accesible desde la página del historial)
- Corrección de errores de Docker
- Capacidad para autorizar a un usuario a conectarse solo desde una computadora en la red local
- Revisión de la configuración de widgets (tenga cuidado, probablemente tendrá que reanudar la configuración de algunos widgets)
- Refuerzo del manejo de errores en widgets
- Capacidad para reordenar vistas
- Revisión de gestión de temas

2.1
---
- Rediseño del sistema de caché Jeedom (uso de caché de doctrina). Esto permite, por ejemplo, conectar Jeedom a un servidor redis o memcached. De forma predeterminada, Jeedom utiliza un sistema de archivos (y ya no es la base de datos MySQL que le permite descargarlo un poco), está en / tmp, por lo que se recomienda si tiene más de 512 MB de RAM para montar el / tmp a tmpfs (en RAM para un uso más rápido y con menos desgaste de la tarjeta SD, recomiendo un tamaño de 64 MB). Tenga cuidado al reiniciar Jeedom, el caché se vacía, por lo que debe esperar a que vuelva a aparecer toda la información.
- Rediseño del sistema de registro (uso de monolog) que permite
integración con sistemas de registro (tipo syslog (d))
- Optimización de la carga del tablero
- Se corrigieron muchas advertencias
- Posibilidad durante una llamada API a un escenario para pasar etiquetas en la url
- Soporte Apache
- Optimización de Docker con soporte oficial de Docker
- Optimización para sinología
- Soporte + optimización para php7
- Rediseño del menú Jeedom
- Eliminar toda la parte de administración de red : wifi, ip fija ... (seguramente volverá como un complemento). TENGA CUIDADO, no se elimina el modo maestro / esclavo jeedom
- Se eliminó la indicación de la batería en los widgets
- Adición de una página que resume el estado de todos los equipos con batería
- Rediseño del DNS de Jeedom, uso de openvpn (y por lo tanto del complemento openvpn)
- Actualizar todas las bibliotecas
- interacción : ajout d'un système d'analyse syntaxique (permet de supprimer les interactions avec de grosses erreurs de syntaxe type « le chambre »)
- Supresión de la actualización de la interfaz por nodejs (cambiar a extraer cada segundo en la lista de eventos)
- Posibilidad de aplicaciones de terceros para solicitar eventos a través de la API
- Refonte du système « d'action sur valeur » avec possibilité de faire plusieurs actions et aussi l'ajout de toutes les actions possibles dans les scénarios (attention il faudra peut-être toutes les reconfigurer suite à la mise à jour)
- Posibilidad de desactivar un bloque en un escenario
- Adición para desarrolladores de un sistema de ayuda de información sobre herramientas. Il faut sur un label mettre la classe « help » et mettre un attribut data-help avec le message d'aide souhaité. Cela permet à Jeedom d'ajouter automatiquement à la fin de votre label une icône « ? » et au survol d'afficher le texte d'aide
- Cambio del proceso de actualización principal, ya no solicitamos el archivo del Mercado sino directamente a Github ahora
- Adición de un sistema centralizado para instalar dependencias en complementos
- Rediseño de la página de administración de complementos
- Agregar direcciones mac de las diferentes interfaces
- Se agregó una conexión de autenticación doble
- Eliminación de la conexión de hash (por razones de seguridad)
- Agregar un sistema de administración del sistema operativo
- Adición de widgets estándar de Jeedom
- Ajout d'un système en beta pour trouver l'IP de Jeedom sur le réseau (il faut connecter Jeedom sur le réseau, puis aller sur le market et cliquer sur « Mes Jeedoms » dans votre profil)
- Adición a la página de escenarios de un probador de expresión
- Revisión del sistema de intercambio de escenarios.

2.0
---
- Rediseño del sistema de caché Jeedom (uso de caché de doctrina). Esto permite, por ejemplo, conectar Jeedom a un servidor redis o memcached. De forma predeterminada, Jeedom utiliza un sistema de archivos (y ya no es la base de datos MySQL que le permite descargarlo un poco), está en / tmp, por lo que se recomienda si tiene más de 512 MB de RAM para montar el / tmp a tmpfs (en RAM para un uso más rápido y con menos desgaste de la tarjeta SD, recomiendo un tamaño de 64 MB). Tenga cuidado al reiniciar Jeedom, el caché se vacía, por lo que debe esperar a que vuelva a aparecer toda la información.
- Rediseño del sistema de registro (uso de monolog) que permite
integración con sistemas de registro (tipo syslog (d))
- Optimización de la carga del tablero
- Se corrigieron muchas advertencias
- Posibilidad durante una llamada API a un escenario para pasar etiquetas en la url
- Soporte Apache
- Optimización de Docker con soporte oficial de Docker
- Optimización para sinología
- Soporte + optimización para php7
- Rediseño del menú Jeedom
- Eliminar toda la parte de administración de red : wifi, ip fija ... (seguramente volverá como un complemento). TENGA CUIDADO, no se elimina el modo maestro / esclavo jeedom
- Se eliminó la indicación de la batería en los widgets
- Adición de una página que resume el estado de todos los equipos con batería
- Rediseño del DNS de Jeedom, uso de openvpn (y por lo tanto del complemento openvpn)
- Actualizar todas las bibliotecas
- interacción : ajout d'un système d'analyse syntaxique (permet de supprimer les interactions avec de grosses erreurs de syntaxe type « le chambre »)
- Supresión de la actualización de la interfaz por nodejs (cambiar a extraer cada segundo en la lista de eventos)
- Posibilidad de aplicaciones de terceros para solicitar eventos a través de la API
- Refonte du système « d'action sur valeur » avec possibilité de faire plusieurs actions et aussi l'ajout de toutes les actions possibles dans les scénarios (attention il faudra peut-être toutes les reconfigurer suite à la mise à jour)
- Posibilidad de desactivar un bloque en un escenario
- Adición para desarrolladores de un sistema de ayuda de información sobre herramientas. Il faut sur un label mettre la classe « help » et mettre un attribut data-help avec le message d'aide souhaité. Cela permet à Jeedom d'ajouter automatiquement à la fin de votre label une icône « ? » et au survol d'afficher le texte d'aide
- Cambio del proceso de actualización principal, ya no solicitamos el archivo del Mercado sino directamente a Github ahora
- Adición de un sistema centralizado para instalar dependencias en complementos
- Rediseño de la página de administración de complementos
- Agregar direcciones mac de las diferentes interfaces
- Se agregó una conexión de autenticación doble
- Eliminación de la conexión de hash (por razones de seguridad)
- Agregar un sistema de administración del sistema operativo
- Adición de widgets estándar de Jeedom
- Ajout d'un système en beta pour trouver l'IP de Jeedom sur le réseau (il faut connecter Jeedom sur le réseau, puis aller sur le market et cliquer sur « Mes Jeedoms » dans votre profil)
- Adición a la página de escenarios de un probador de expresión
- Revisión del sistema de intercambio de escenarios.
