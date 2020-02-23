# copias de seguridad
**Configuración → Sistema → Copias de seguridad**

Jeedom ofrece la posibilidad de ser guardado y restaurado desde o desde diferentes ubicaciones.
Esta página permite la gestión de copias de seguridad, restaura.


Encontrará, a la izquierda, los parámetros y botones de acción. A la derecha está el estado en tiempo real de la acción en curso (copia de seguridad o restauración), si ha lanzado una..

## copias de seguridad

- **copias de seguridad** : Le permite iniciar una copia de seguridad de forma manual e inmediata (útil si desea realizar un cambio crítico. Esto te permitirá volver). También tiene un botón para iniciar una copia de seguridad sin enviar el archivo a la nube (requiere una suscripción, ver más abajo). Enviar una copia de seguridad a la nube puede llevar un tiempo. Por lo tanto, esta opción evita la pérdida excesiva de tiempo..

- **Ubicación de respaldo** : Indica la carpeta en la que Jeedom copia las copias de seguridad.. Se recomienda no cambiarlo.. Si está en un camino relativo, su origen es donde está instalado Jeedom.

- **Número de días de almacenamiento de copias de seguridad.** : Número de días de respaldo para mantener. Una vez que este período haya pasado, las copias de seguridad se eliminarán. Tenga cuidado de no poner demasiados días, de lo contrario su sistema de archivos puede estar saturado.

- **Tamaño total máximo de copias de seguridad (MB)** : Limita el espacio ocupado por todas las copias de seguridad en la carpeta de copias de seguridad. Si se excede este valor, Jeedom eliminará las copias de seguridad más antiguas hasta que caiga por debajo del tamaño máximo. Sin embargo, mantendrá al menos una copia de seguridad.

## Copias de seguridad locales

- **Copias de seguridad disponibles** : Lista de copias de seguridad disponibles.

- **Restaurar copia de seguridad** : Inicia la restauración de la copia de seguridad seleccionada anteriormente..

- **Eliminar copia de seguridad** : Elimine la copia de seguridad seleccionada anteriormente, solo en la carpeta local.

- **Enviar una copia de seguridad** : Le permite enviar un archivo ubicado en la computadora que está utilizando actualmente a la carpeta de copias de seguridad (por ejemplo, para restaurar un archivo recuperado previamente en un nuevo Jeedom o para reinstalarlo).

- **Descargar copia de seguridad** : Descargue el archivo de la copia de seguridad seleccionada anteriormente en su computadora.

## Copias de seguridad del mercado

- **Enviar copias de seguridad** : Dígale a Jeedom que envíe copias de seguridad a la nube de Market, tenga en cuenta que debe haberse suscrito.

- **Enviar una copia de seguridad** : Enviar un archivo de respaldo ubicado en su computadora a la nube.

- **Copias de seguridad disponibles** : Lista de copias de seguridad disponibles en la nube.

- **Restaurar copia de seguridad** : Comienza a restaurar una copia de seguridad en la nube.

## Copias de seguridad de Samba

- **Enviar copias de seguridad** : Le dice a Jeedom que envíe las copias de seguridad al recurso compartido de samba configurado aquí Configuración → Sistema → Configuración : Actualizaciones.

- **Copias de seguridad disponibles** : Lista de copias de seguridad de samba disponibles.

- **Restaurar copia de seguridad** : Comienza a restaurar la copia de seguridad de samba seleccionada anteriormente.

> **punta**
>
> Dependiendo de lo que se active, en la página Configuración → Sistema → Configuración : Actualizaciones, puedes ver más o menos secciones.

> **punta**
>
> Al reinstalar Jeedom y haber tomado la suscripción de copia de seguridad de Cloud de Market, debe ingresar su cuenta de Market en su nuevo Jeedom (Configuración → Sistema → Configuración : Actualizaciones) luego ven aquí para comenzar la restauración.

> **punta**
>
> Es posible, en caso de problemas, hacer una copia de seguridad en la línea de comando :
>  `sudo php /usr/share/nginx/www/jeedom/install/backup.php`
> o `sudo php / var / www / html / install / backup.php` dependiendo de su sistema.

> **punta**
>
> También es posible restaurar una copia de seguridad de la línea de comandos (de forma predeterminada, Jeedom restaura la copia de seguridad más reciente presente en el directorio de copia de seguridad) :
> `sudo php /usr/share/nginx/www/jeedom/install/restore.php` o
> `sudo php /var/www/html/install/restore.php`.

# Lo que se guarda ?

Durante una copia de seguridad, Jeedom realizará una copia de seguridad de todos sus archivos y la base de datos. Esto, por lo tanto, contiene toda su configuración (equipo, controles, historial, escenarios, diseño, etc.).

A nivel de protocolo, solo la Z-Wave (OpenZwave) es un poco diferente porque no es posible guardar las inclusiones. Estos se incluyen directamente en el controlador, por lo que debe mantener el mismo controlador para encontrar sus módulos Zwave.

> **nota**
>
> El sistema en el que está instalado Jeedom no está respaldado. Si ha cambiado la configuración de este sistema (incluso a través de SSH), depende de usted encontrar una manera de recuperarlos si tiene alguna inquietud..

# Copia de seguridad en la nube

La copia de seguridad en la nube le permite a Jeedom enviar sus copias de seguridad directamente al mercado. Esto le permite restaurarlos fácilmente y asegurarse de no perderlos.. The Market conserva las últimas 6 copias de seguridad. Para suscribirte solo ve a tu página **perfil** en el mercado, luego en la pestaña **mis copias de seguridad**. Puede, desde esta página, recuperar una copia de seguridad o comprar una suscripción (durante 1, 3, 6 o 12 meses).

> **punta**
>
> Puede personalizar el nombre de los archivos de copia de seguridad desde la pestaña **Mis jeedoms**, sin embargo evitando personajes exóticos.

# Frecuencia de respaldos automáticos

Jeedom realiza una copia de seguridad automática todos los días a la misma hora. Es posible modificarlo, desde el &quot;Motor de tareas&quot; (la tarea se denomina **Jeedom backup**), pero no se recomienda. De hecho, se calcula en relación con la carga del mercado.
