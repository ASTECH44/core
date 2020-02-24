El submenú de administración de complementos le permite manipular complementos, excepto
conocer : descárguelos, actualícelos y actívelos, ...

Gestión de complementos 
===================

Puede acceder a la página de complementos desde Complementos → Administrar
plugins. Una vez que hacemos clic en él, encontramos la lista de
complementos en orden alfabético y un enlace al mercado. Complementos
deshabilitados están en gris.

> **punta**
>
> Como en muchos lugares de Jeedom, coloca el mouse en el extremo izquierdo
> abre un menú de acceso rápido (puedes
> desde tu perfil siempre déjalo visible). Aquí el menú
> permite tener la lista de complementos ordenados por categorías.

Al hacer clic en un complemento, accede a su configuración. Arriba tu
encuentre el nombre del complemento, luego entre paréntesis, su nombre en Jeedom
(ID) y, finalmente, el tipo de versión instalada (estable, beta).

> **importante**
>
> Al descargar un complemento, está deshabilitado de forma predeterminada.
> Entonces tienes que activarlo tú mismo.

Arriba a la derecha, algunos botones. :

-   **documentación** : Permite el acceso directo a la página de
    documentación del complemento

-   **cambios** : permite ver el registro de cambios del complemento si existe

-   **Enviar al mercado** : permite enviar el complemento en el mercado
    (solo disponible si usted es el autor)

-   **detalles** : permite encontrar la página de complementos en el mercado

-   **remove** : Elimina el complemento de tu Jeedom. Ten cuidado, esto
    también elimina permanentemente todo el equipo de este complemento

Abajo a la izquierda, hay un área de estado con :

-   **estatus** : permite ver el estado del complemento (activo / inactivo)

-   **versión** : la versión del complemento instalado

-   **autor** : autor del complemento

-   **acción** : Le permite habilitar o deshabilitar el complemento

-   **Versión Jeedom** : Indica la versión mínima requerida de Jeedom
    para el complemento

-   **licencia** : Indica la licencia del complemento que generalmente será
    AGPL

A la derecha, encontramos el área de registro que le permite definir 

-   el nivel de registros específicos del complemento (encontramos esta misma posibilidad en
Administración → Configuración en la pestaña de registros, en la parte inferior de la página)

-   ver los registros del complemento

-   latido del corazón : cada 5 minutos, Jeedom comprueba si al menos un dispositivo de complemento se ha comunicado en los últimos X minutos (si desea desactivar la funcionalidad, simplemente ponga 0)

-   Reiniciar demonio : si el latido sale mal, entonces Jeedom reiniciará el demonio

Si el complemento tiene dependencias y / o un demonio, estas áreas
adicionales se muestran debajo de las áreas mencionadas anteriormente.

dependencias :

-   **apellido** : generalmente será local

-   **estatus** : le dirá si las dependencias están bien o no

-   **instalación** : instalará o reinstalará
    dependencias (si no lo hace manualmente y son
    KO, Jeedom se cuidará solo después de un tiempo)

-   **Última instalación** : fecha de la última instalación de
    dependencias

demonio :

-   **apellido** : generalmente será local

-   **estatus** : te dirá si el demonio está bien o no

-   **configuración** : estará bien si todos los criterios para el demonio
    se cumplen los turnos o darán lugar a un bloqueo

-   **(Re) Inicio** : permite lanzar o relanzar al demonio

-   **Parar** : permite detener al demonio (solo en caso
    la gestión automática está deshabilitada)

-   **Gestión automática** : permite activar o desactivar la gestión
    automático (que permite a Jeedom gestionar el demonio y el
    revivir si es necesario. A menos que se indique lo contrario, es aconsejable
    dejar activa la gestión automática)

-   **Último lanzamiento** : fecha del último lanzamiento del demonio

> **punta**
>
> Algunos complementos tienen una parte de configuración. Si es así,
> aparecerá debajo de las dependencias y zonas de daemon descritas anteriormente.
> En este caso, consulte la documentación del complemento en
> pregunta sobre cómo configurarlo.

A continuación, hay un área de funcionalidad. Esto te permite ver
si el complemento utiliza una de las funciones principales de Jeedom, como :

-   **Interact** : interacciones específicas

-   **cron** : un cron por minuto

-   **cron5** : un cron cada 5 minutos

-   **cron15** : un cron cada 15 minutos

-   **cron30** : un cron cada 30 minutos

-   **cronHourly** : un cron cada hora

-   **cronDaily** : un cron diario

> **punta**
>
> Si el complemento usa una de estas funciones, puede
> prohibirle que lo haga desmarcando la casilla &quot;activar&quot; que será
> presente siguiente.

Finalmente, podemos encontrar una sección de Panel que activará o
desactivar la visualización del panel en el tablero o en el dispositivo móvil si
el complemento ofrece uno.

Instalación de complementos 
========================

Para instalar un nuevo complemento, simplemente haga clic en el botón
&quot;Mercado&quot; (y que Jeedom está conectado a Internet). Después de un corto tiempo de
cargando obtendrá la página.

> **punta**
>
> Debe haber ingresado la información de su cuenta Market en
> administración (Configuración → Actualizaciones → pestaña Mercado) para
> encuentre los complementos que ya ha comprado, por ejemplo.

En la parte superior de la ventana tienes filtros :

-   **Abierto / De pago** : muestra solo gratis o
    los pagadores.

-   **Oficial / Recomendado** : muestra solo complementos
    funcionarios o asesores

-   **Instalado / No instalado** : muestra solo complementos
    instalado o no instalado

-   **Menú desplegable de categoría** : solo muestra
    ciertas categorías de complementos

-   **Buscar** : le permite buscar un complemento (en el nombre o
    descripción de la misma)

-   **nombre del usuario** : muestra el nombre de usuario utilizado para
    conexión al mercado y el estado de la conexión

> **punta**
>
> La pequeña cruz restablece el filtro en cuestión.

Una vez que haya encontrado el complemento que desea, simplemente haga clic en
este para traer su tarjeta. Esta hoja te da mucho
información sobre el complemento, incluido :

-   Si es oficial / recomendado o si está obsoleto (realmente necesita
    evite instalar complementos obsoletos)

-   4 acciones :

    -   **Instalar estable** : permite instalar el complemento en su
        versión estable

    -   **Instalar beta** : permite instalar el complemento en su
        versión beta (solo para probadores beta)

    -   **Instalar pro** : permite instalar la versión pro (muy
        poco usado)

    -   **remove** : si el complemento está instalado actualmente, esto
        botón para borrarlo

A continuación, encontrará la descripción del complemento, la compatibilidad
(si Jeedom detecta una incompatibilidad, se lo notificará), las revisiones
en el complemento (puedes calificarlo aquí) e información
complementario (el autor, la persona que realizó la última actualización
día, enlace al documento, número de descargas). Sobre la derecha
encontrará un botón &quot;cambios&quot; que le permite tener todo
historial de cambios, un botón de &quot;Documentación&quot; que regresa
a la documentación del complemento. Entonces tienes el idioma disponible
y la diversa información sobre la fecha de la última versión estable.

> **importante**
>
> Realmente no se recomienda poner un complemento beta en un
> Jeedom no beta, muchos problemas operativos pueden
> resultar.

> **importante**
>
> Algunos complementos son de pago, en este caso la hoja del complemento
> ofrecerá comprarlo. Una vez hecho esto, espere un
> diez minutos (tiempo de validación de pago), luego regresar
> en la hoja del complemento para instalarlo normalmente.

> **punta**
>
> También puede agregar un complemento a Jeedom desde un archivo o
> de un repositorio de Github. Esto requiere, en la configuración de
> Jeedom, active la función apropiada en &quot;Actualizaciones y
> archivos &quot;. Entonces será posible, colocando el mouse completamente
> izquierda, y cuando aparezca el menú de la página de complementos, haga clic en
> en &quot;Agregar de otra fuente&quot;. Luego puedes elegir el
> fuente &quot;Archivo&quot;. Atención, en el caso de la adición por un archivo
> zip, el nombre zip debe ser el mismo que el ID del complemento y de
> abriendo el ZIP debe estar presente una carpeta de plugin \ _info.
