Aquí está la parte más importante de la automatización del hogar. : los escenarios.
Verdadero cerebro de la domótica, es lo que hace posible interactuar con
el mundo real de una "manera inteligente".

La página de gestión de escenarios
================================

Gestion
-------

Para acceder, nada más simple, solo ve a Herramientas ->
Escenarios. Encontrará allí la lista de escenarios para su Jeedom también
solo funciones para gestionarlos mejor :

-   **Ajouter** : Crea un escenario. Se describe el procedimiento.
    en el siguiente capitulo.

-   **Deshabilitar escenarios** : Deshabilita todos los escenarios..

-   **Ver variables** : Veamos las variables, su valor también
    que el lugar donde se usan. Tambien puedes
    crear un. Las las variables se describen en un capítulo de
    esta página.

-   **Resumen** : Le permite tener una visión general de todos
    los escenarios. Puedes cambiar los valores **actif**,
    **visible**, **lanzamiento múltiple**, **modo síncrono**, **Log** et
    **Timeline** (estos parámetros se describen en el siguiente capítulo).
    También puede acceder a los registros para cada escenario y
    comenzar individualmente.

-   **Probador de expresión** : Le permite ejecutar una prueba en un
    expresión de su elección y mostrar el resultado.

Mis escenarios
-------------

En esta sección encontrarás el **lista de escenarios** que usted
he creado. Se clasifican de acuerdo a **groupes** que tienes
definido para cada uno de ellos. Cada escenario se muestra con su **nom**
y su **objeto padre**. La **escenarios atenuados** son los que son
discapacitado.

Como en muchas páginas de Jeedom, coloque el mouse a la izquierda de
la pantalla muestra un menú de acceso rápido (desde
tu perfil, siempre puedes dejarlo visible). Usted puede
entonces **chercher** su escenario, pero también en **ajouter** uno por esto
menu.

Editar un escenario
=====================

Después de hacer clic en **Ajouter**, debes elegir el nombre de tu
escenario y se le redirige a su página de configuración general.
En la parte superior, hay algunas funciones útiles para administrar nuestro escenario.
:

-   **ID** : Al lado de la palabra **General**, este es el identificador de escenario.

-   **statut** : Estado actual de su escenario.

-   **variables** : Ver las variables.

-   **Expression** : Muestra el probador de expresiones..

-   **Realizar** : Le permite iniciar el escenario manualmente (recuerde
    no guardar antes!). Los desencadenantes por lo tanto no son
    no tomado en cuenta.

-   **Supprimer** : Eliminar escenario.

-   **Sauvegarder** : Guardar los cambios realizados.

-   **Template** : Le permite acceder y aplicar plantillas.
    al guión del mercado. (explicado al final de la página).

-   **Exporter** : Obtenga una versión de texto del guión.

-   **Log** : Muestra los registros del escenario..

-   **Dupliquer** : Copie el escenario para crear uno
    nuevo con otro nombre.

-   **Liens** : Le permite ver el gráfico de los elementos vinculados.
    con el guión.

Pestaña General
--------------

En la pestaña **General**, encontramos los principales parámetros de
nuestro escenario :

-   **Nombre del escenario** : El nombre de tu escenario.

-   **Nombre para mostrar** : El nombre utilizado para su visualización..

-   **Groupe** : Le permite organizar los escenarios, clasificándolos en
    grupos.

-   **Actif** : Activa el escenario.

-   **Visible** : Se usa para hacer visible el escenario.

-   **Objeto padre** : Asignación a un objeto padre.

-   **Segundos de tiempo de espera (0 = ilimitado)** : El tiempo máximo de ejecución
    autorizado

-   **Lanzamiento múltiple** : Marque esta casilla syo desea
    el escenario se puede iniciar varias veces al mismo tiempo.

-   **Modo síncrono** : Inicie el escenario en el hilo actual en lugar de un hilo dedicado. Aumenta la velocidad de lanzamiento del escenario pero puede hacer que el sistema sea inestable.

-   **Log** : El tipo de registro deseado para el escenario.

-   **Sigue en la línea de tiempo** : Realiza un seguimiento del escenario.
    en la linea de tiempo.

-   **Description** : Le permite escribir un pequeño texto para describir
    tu escenario.

-   **Modo de escenario** : El escenario puede ser programado, activado o
    ambos al mismo tiempo. Luego tendrá la opción de indicar el (los)
    disparador (es) (tenga cuidado, hay un límite para el número de disparadores posibles por escenario de 15) y la programación (s).

> **Tip**
>
> Atención : puedes tener un máximo de 28
> disparadores / programación para un escenario.

Pestaña Escenario
---------------

Aquí es donde construirás tu escenario. Tenemos que empezar
por **agregar un bloque**, con el botón de la derecha. Una vez un bloque
creado, puedes agregar otro **bloc** o un **action**.

> **Tip**
>
> En condiciones y acciones, es mejor favorecer comillas simples (&#39;) en lugar de dobles (")

### Bloques

Aquí están los diferentes tipos de bloques disponibles. :

-   **If / Then / O** : Le permite realizar acciones.
    bajo condiciones.

-   **Action** : Le permite lanzar acciones simples sin
    sin condiciones.

-   **Boucle** : Le permite realizar acciones repetidamente
    1 hasta un número definido (o incluso el valor de un sensor, o un
    número aleatorio ...).

-   **Dans** : Inicia una acción en X minuto (s) (0 es un
    valor posible). La peculiaridad es que las acciones se lanzan
    en segundo plano, para que no bloqueen el resto del escenario.
    Entonces es un bloque sin bloqueo.

-   **A** : Permite decirle a Jeedom que inicie las acciones del bloque en un
    tiempo dado (en la forma hhmm). Este bloque no es bloqueante. Ex :
    0030 para 00:30, o 0146 para 1h46 y 1050 para 10h50.

-   **Code** : Le permite escribir directamente en código PHP (solicitud
    cierto conocimiento y puede ser arriesgado pero permite no tener
    sin restricciones).

-   **Commentaire** : Le permite agregar comentarios a su escenario.

Cada uno de estos bloques tiene sus opciones para manejarlos mejor :

-   La casilla de verificación a la izquierda le permite deshabilitar completamente
    bloquear sin eliminarlo.

-   La flecha doble vertical a la izquierda le permite mover todo
    bloque por arrastrar y soltar.

-   El botón, en el extremo derecho, le permite eliminar todo el bloque.

#### Syo / Entonces / De lo contrario bloquea, Bucle, In y A

> **Note**
>
> En bloques Syo / Entonces / De lo contrario, flechas circulares ubicadas
> a la izquierda del campo de condición permite activar o no el
> repetición de acciones syo la evaluación de la condición da el mismo
> resultado que la evaluación anterior.

Para las condiciones, Jeedom trata de asegurarse de que podamos
escribir tanto como sea posible en lenguaje natural sin dejar de ser flexible. Tres
los botones están disponibles a la derecha de este tipo de bloque para
seleccione un elemento para probar :

-   **Encuentra un pedido** : Le permite buscar un pedido en
    todos los disponibles en Jeedom. Una vez que se encuentra el pedido,
    Jeedom abre una ventana para preguntarte qué prueba quieres
    actuar en ello. Syo eliges **No poner nada**,
    Jeedom agregará el pedido sin comparación. Usted puede también
    elegir **et** o **ou** delante **Ensuite** para encadenar pruebas
    en diferentes equipos.

-   **Buscar un escenario** : Permite buscar un escenario
    para probar.

-   **Busca equipo** : Lo mismo para el equipo..

> **Tip**
>
> Hay una lista de etiquetas que permiten el acceso a las las variables.
> del guión u otro, o por hora, fecha, un
> número aleatorio, .... Vea más adelante los capítulos sobre comandos y
> etiquetas.

Una vez que se complete la condición, debe usar el botón
"agregar ", izquierda, para agregar un nuevo **bloc** o un
**action** en el bloque actual.

> **Tip**
>
> NO DEBE utilizar [] en pruebas de condición, solo son posibles paréntesis ()

#### Código de bloque

> **Important**
>
> Tenga en cuenta que las etiquetas no están disponibles en un bloque de código.

Controles (sensores y actuadores):
-   cmd::byString ($ cadena); : Devuelve el objeto de comando correspondiente.
  -   $string : Enlace al pedido deseado : #[objeto] [equipo] [comando] # (por ejemplo, : #[Lapartamento] [Lalarma] [Lactivo] #)
-   cmd::BYIdentificación ($ id); : Devuelve el objeto de comando correspondiente.
  -   $id : Identificación de pedido
-   $cmd->execCmd($options = null); : Ejecute el comando y devuelva el resultado..
  -   $options : Opciones para ejecutar el comando (puede ser específico del complemento), opción básica (subtipo de comando) :
    -   mensaje : $option = array('title' => 'titre du mensaje , 'message' => 'Mon message');
    -   color : $option = array('color' => 'couleur en hexadécimal');
    -   deslizador : $option = array('slider' => 'valeur voulue de 0 à 100');

Registro :
-   log::add ( &#39;nombre&#39; &#39;nivel&#39;, &#39;mensaje&#39;);
  -   nombre de archivo : Nombre del archivo de registro.
  -   nivel : [depuración], [yonformación], [error], [evento].
  -   mensaje : Mensaje para escribir en los registros.

Guión :
-   $scenario->getName(); : Devuelve el nombre del escenario actual.
-   $scenario->getGroup(); : Devuelve el grupo de escenarios..
-   $scenario->getIsActive(); : Devuelve el estado del escenario..
-   $scenario->setIsActive($active); : Le permite activar o no el escenario.
  -   $active : 1 activo, 0 no activo.
-   $scenario->setOnGoing($onGoing); : Digamos syo el escenario se está ejecutando o no.
  -   $onGoing => 1 en cours , 0 arrêté.
-   $scenario->save(); : Guardar cambios.
-   $scenario->setData($key, $value); : Guardar un dato (Variable).
  -   $key : clave de valor (int o cadena).
  -   $value : valor a almacenar (int, cadena, matriz u objeto).
-   $scenario->getData($key); : Obtener datos (Variable).
  -   $key => clave de valor (int o cadena).
-   $scenario->removeData($key); : Eliminar datos.
-   $scenario->setLog($message); : Escribir un mensaje en el registro del escenario.
-   $scenario->persistLog(); : Forzar la escritura del registro (de lo contrario, se escribe solo al final del escenario). Tenga cuidado, esto puede retrasar un poco el escenario.

### Las acciones

Las acciones agregadas a los bloques tienen varias opciones. En el orden :

-   Una cabaña **paralelas** para que este comando se inicie en paralelo
    otros comandos también seleccionados.

-   Una cabaña **activado** para que este comando se tenga en cuenta
    cuenta en el escenario.

-   Una **flecha doble vertical** para mover la acción. Basta con
    arrastrar y soltar desde allí.

-   Un botón para eliminar la acción..

-   Un botón para acciones específicas, cada vez con el
    descripción de esta acción.

-   Un botón para buscar un comando de acción.

> **Tip**
>
> Dependiendo del comando seleccionado, podemos ver diferentes
> campos adicionales mostrados.

Posibles sustituciones
===========================

Disparadores
----------------

Hay desencadenantes específicos (distintos de los proporcionados por
comandos) :

-   #start# : activado al (re) inicio de Jeedom,

-   #begin_backup# : evento enviado al inicio de una copia de seguridad.

-   #end_backup# : evento enviado al final de una copia de seguridad.

-   #BEGIN_UPDATE# : evento enviado al inicio de una actualización.

-   #END_UPDATE# : evento enviado al final de una actualización.

-   #begin_restore# : evento enviado al inicio de una restauración.

-   #restauración_final# : evento enviado al final de una restauración.

-   #user_connect# : inicio de sesión de usuario

También puede desencadenar un escenario cuando una variable se establece en
día poniendo : #variable (nombre_variable) # o usando la API HTTP
descrito
[aquí](https://jeedom.github.io/core/fr_FR/api_http).

Operadores de comparación y enlaces entre condiciones
-------------------------------------------------------

Puede usar cualquiera de los siguientes símbolos para
comparaciones en condiciones :

-   == : igual a,

-   \> : estrictamente mayor que,

-   \>= : mayor o igual que,

-   < : estrictamente menor que,

-   <= : menor o igual que,

-   != : diferente de, no es igual a,

-   cerillas : contiene (por ejemplo, :
    [Baño] [Hidrometría] [estado] coincide con "/ wy /"),

-   no (... coincide ...) : no contiene (por ejemplo, :
    no ([Baño] [Hidrometría] [estado] coincide con "/ húmedo /")),

Puedes combinar cualquier comparación con operadores
siguiente :

-   &amp;&amp; / ET / y / AND / y : et,

-   \|| / OR / o / OR / o : ou,

-   \|^ / XOR / xor : o exclusivo.

Etiquetas
--------

Una etiqueta se reemplaza durante la ejecución del escenario por su valor. Vosotras
puede usar las siguientes etiquetas :

> **Tip**
>
> Para mostrar los ceros a la izquierda, use el
> Función de fecha (). Ver
> [aquí](http://php.net/manual/fr/function.date.php).

-   #seconde# : Segundo actual (sin ceros a la izquierda, ej. : 6 para
    08:07:06),

-   #heure# : Hora actual en formato de 24 h (sin ceros a la izquierda),
    ex : 8 para 08:07:06 o 17 para 17:15),

-   #heure12# : Hora actual en formato de 12 horas (sin ceros a la izquierda),
    ex : 8 para 08:07:06),

-   #minute# : Minuto actual (sin ceros a la izquierda, ej. : 7 para
    08:07:06),

-   #jour# : Día actual (sin ceros a la izquierda, ej. : 6 para
    06.07.2017),

-   #mois# : Mes actual (sin ceros a la izquierda, ej. : 7 para
    06.07.2017),

-   #annee# : Año actual,

-   #time# : Hora y minuto actual (por ejemplo, : 1715 para las 5.15 p.m.),

-   #timestamp# : Número de segundos desde el 1 de enero de 1970,

-   #date# : Día y mes. Atención, el primer número es el mes..
    (por ejemplo, : 1215 para el 15 de diciembre),

-   #semaine# : Número de semana (por ejemplo, : 51),

-   #sjour# : Nombre del día de la semana (por ejemplo, : Samedi),

-   #njour# : Número de día de 0 (domingo) a 6 (sábado),

-   #smois# : Nombre del mes (por ejemplo, : Janvier),

-   #IP# : IP interna de Jeedom,

-   #hostname# : Nombre de la máquina Jeedom,

-   #trigger# : Tal vez el nombre del comando que inició el escenario, &#39;api&#39; syo la API inició el lanzamiento, &#39;horario&#39; syo se inició mediante programación, &#39;usuario&#39; syo se inició manualmente

También tiene las siguientes etiquetas adicionales syo su script ha sido
desencadenado por una interacción :

-   #query# : interacción que desencadenó el escenario,

-   #profil# : perfil del usuario que inició el escenario
    (puede estar vacío).

> **Important**
>
> Cuando un escenario se desencadena por una interacción, es
> necesariamente se ejecuta en modo rápido.

Funciones de cálculo
-----------------------

Hay varias funciones disponibles para el equipo. :

-   promedio (orden, período) y promedio entre (orden, inicio, fin)
    : Proporcione el promedio del pedido durante el período.
    (período = [mes, día, hora, min] o [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    entre las 2 terminales requeridas (en la forma Ymd H:i:s o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   min (orden, período) y minBetween (orden, inicio, fin) :
    Dar el pedido mínimo durante el período
    (período = [mes, día, hora, min] o [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    entre las 2 terminales requeridas (en la forma Ymd H:i:s o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   max (orden, período) y maxBetween (orden, inicio, fin) :
    Dar el máximo del pedido durante el período
    (período = [mes, día, hora, min] o [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    entre las 2 terminales requeridas (en la forma Ymd H:i:s o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   duración (orden, valor, período) y
    durationbetween (valor de comando, inicio, fin) : Dar la duración en
    minutos durante los cuales el equipo tenía el valor seleccionado en el
    período (período = [mes, día, hora, min] o [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    entre las 2 terminales requeridas (en la forma Ymd H:i:s o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   estadísticas (orden, cálculo, período) y
    statisticsBetween (control, cálculo, inicio, fin) : Dar el resultado
    diferentes cálculos estadísticos (suma, recuento, estándar),
    varianza, promedio, min, max) durante el período
    (período = [mes, día, hora, min] o [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    entre las 2 terminales requeridas (en la forma Ymd H:i:s o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   tendencia (comando, período, umbral) : Da la tendencia de
    orden durante el período (período = [mes, día, hora, min] o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   stateDuration (control) : Da duración en segundos
    desde el último cambio de valor. Devuelve -1 syo ninguno
    el historial no existe o syo el valor no existe en el historial.
    Devuelve -2 syo el pedido no está registrado.

-   lastChangeStateDuration (valor de comandos) : Dar la duración en
    segundos desde el último cambio de estado al valor pasado
    como un parámetro. Devuelve -1 syo ninguno
    el historial no existe o syo el valor no existe en el historial.
    Devuelve -2 syo el pedido no está registrado

-   lastStateDuration (valor de comandos) : Da duración en segundos
    durante el cual el equipo ha tenido recientemente el valor elegido.
    Devuelve -1 syo no existe un historial o syo el valor no existe en el historial.
    Devuelve -2 syo el pedido no está registrado

-   stateChanges (orden, [valor], punto) y
    stateChangesBetween (comando, [valor], inicio, fin) : Dar el
    cantidad de cambios de estado (a un cierto valor syo se indica,
    o en total de lo contrario) durante el período (período = [mes, día, hora, min] o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    entre las 2 terminales requeridas (en la forma Ymd H:i:s o
    [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   lastBetween (mando, inicio, fin) : Devuelve el último valor.
    registrado para el equipo entre los 2 terminales requeridos (bajo el
    forma Ymd H:i:s o [expresión
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   variable (variable, predeterminada) : Obtenga el valor de un
    variable o el valor predeterminado deseado :

-   escenario (escenario) : Devuelve el estado del escenario.. 1 en progreso, 0
    syo se detiene y -1 syo está deshabilitado, -2 syo el escenario no existe y -3
    syo el estado no es consistente. Para tener el nombre &quot;humano&quot; del escenario, puede usar el botón dedicado a la derecha de la búsqueda del escenario.

-   lastScenarioExecution (escenario) : Da duración en segundos
    desde el lanzamiento del último escenario :

-   collectDate (CMD [tamaño]) : Devuelve la fecha de los últimos datos.
    para el comando dado como parámetro, el segundo parámetro opcional
    permite especificar el formato de retorno (detalles
    [aquí](http://php.net/manual/fr/function.date.php)) Un retorno de -1
    significa que no se puede encontrar el pedido y -2 que el pedido no es
    sin tipo de información

-   ValueDate (CMD [tamaño]) : Devuelve la fecha de los últimos datos.
    para el comando dado como parámetro, el segundo parámetro opcional
    permite especificar el formato de retorno (detalles
    [aquí](http://php.net/manual/fr/function.date.php)) Un retorno de -1
    significa que no se puede encontrar el pedido y -2 que el pedido no es
    sin tipo de información

-   eqEnable (equipo) : Devuelve el estado del equipo.. -2 si
    no se puede encontrar el equipo, 1 syo el equipo está activo y 0 syo no lo está
    está inactivo

-   valor (cmd) : Devuelve el valor de un pedido syo Jeedom no lo proporciona automáticamente (caso al almacenar el nombre del pedido en una variable)    

-   etiqueta (de lunes [por defecto]) : Se utiliza para recuperar el valor de una etiqueta o
    el valor predeterminado syo no existe :

-   nombre (tipo, control) : Se usa para recuperar el nombre del comando,
    equipo u objeto. El tipo vale cmd, eqLogic o
    objeto.

-   lastCommunication (equipo, [tamaño]) : Devuelve la fecha de la última comunicación.
    para el equipo dado como parámetro, el segundo parámetro opcional
    permite especificar el formato de retorno (detalles
    [aquí](http://php.net/manual/fr/function.date.php)) Un retorno de -1
    significa que no se puede encontrar el equipo

-   color_gradient (couleur_debut, couleur_fin, valuer_min, valeur_max, valor) : Devuelve un color calculado con respecto al valor en el rango color_comienzo / color_end. El valor debe estar entre min_value y max_value

Los períodos e intervalos de estas funciones también pueden
utilizar con [expresiones
PHP](http://php.net/manual/fr/datetime.formats.relative.php) comme par
ejemplo :

-   Ahora : maintenant

-   Hoy : 00:00 hoy (permite por ejemplo obtener
    resultados del día syo está entre &#39;Hoy&#39; y &#39;Ahora&#39;)

-   Lunes pasado : el lunes pasado a las 00:00

-   Hace 5 dias : Hace 5 dias

-   Ayer mediodia : ayer mediodia

-   Etcétera.

Aquí hay ejemplos prácticos para comprender los valores devueltos por
estas diferentes funciones :

| Zócalo con valores :           | 000 (por 10 minutos) 11 (por 1 hora) 000 (por 10 minutos)    |
|--------------------------------------|--------------------------------------|
| promedio (tomando, periodo)             | Devuelve el promedio de 0 y 1 (puede  |
|                                      | ser influenciado por las encuestas)      |
| promedio Entre (\# [Baño] [Hidrometría] [Humedad] \#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Devuelve el pedido promedio entre el 1 de enero de 2015 y el 15 de enero de 2015                         |
| min (salida, periodo)                 | Devuelve 0 : el tapón se apagó durante el período              |
| minBetween (\# [Baño] [Hidrometría] [Humedad] \#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Devuelve el pedido mínimo entre el 1 de enero de 2015 y el 15 de enero de 2015                         |
| max (decisión, período)                 | Devuelve 1 : el enchufe estaba bien iluminado en el período              |
| maxBetween (\# [Baño] [Hidrometría] [Humedad] \#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Devuelve el máximo del pedido entre el 1 de enero de 2015 y el 15 de enero de 2015                         |
| duración (enchufe, 1 período)          | Devuelve 60 : el enchufe estuvo encendido (a 1) durante 60 minutos en el período                              |
| duración Entre (\# [Salón] [Tomar] [Estado] \#, 0, Último lunes, ahora)   | Devuelve la duración en minutos durante la cual el socky estuvo apagado desde el lunes pasado.                |
| estadísticas (captura, recuento, y punto)    | Devuelve 8 : hubo 8 escaladas en el período               |
| tendencia (enchufe, período 0.1)        | Devuelve -1 : tendencia a la baja    |
| stateDuration (enchufe)               | Devuelve 600 : el enchufe ha estado en su estado actual durante 600 segundos (10 minutos)                             |
| lastChangeStateDuration (captura, 0)   | Devuelve 600 : el zócalo se apagó (cambie a 0) por última vez hace 600 segundos (10 minutos)     |
| lastChangeStateDuration (captura, 1)   | Devuelve 4200 : el zócalo se encendió (cambie a 1) por última vez hace 4200 segundos (1h10)                               |
| lastStateDuration (captura, 0)         | Devuelve 600 : el enchufe ha estado apagado por 600 segundos (10 minutos)     |
| lastStateDuration (captura, 1)         | Devuelve 3600 : el zócalo se encendió por última vez durante 3600 segundos (1 h)           |
| stateChanges (captura, y punto)        | Devuelve 3 : el enchufe cambió de estado 3 veces durante el período            |
| stateChanges (captura, 0, periodo)      | Devuelve 2 : el zócalo se ha apagado (yendo a 0) dos veces durante el período                              |
| stateChanges (captura, 1 período)      | Devuelve 1 : el enchufe se enciende (cambie a 1) una vez durante el período                              |
| lastBetween (\# [Baño] [Hidrometría] [Humedad] \#, ayer, hoy) | Devuelve la última temperatura registrada ayer.                    |
| variable (plop, 10)                  | Devuelve el valor de la variable plop o 10 syo está vacía o no existe                         |
| escenario (\# [Baño] [Luz] [Lauto] \#) | Devuelve 1 en progreso, 0 syo se detiene y -1 syo está desactivado, -2 syo el escenario no existe y -3 syo el estado no es consistente                         |
| lastScenarioExecution (\# [Baño] [Luz] [Lauto] \#)   | Devuelve 300 syo el escenario se inició por última vez hace 5 minutos                                  |
| collectDate (\# [Baño] [Hidrometría] [Humedad] \#)     | Devoluciones 2015-01-01 17:45:12          |
| valueDate (\# [Baño] [Hidrometría] [Humedad] \#) | Devoluciones 2015-01-01 17:50:12          |
| eqEnable (\# [n] [basílica] \#)       | Devuelve -2 syo no se encuentra el equipo, 1 syo el equipo está activo y 0 syo está inactivo          |
| etiqueta (de lunes toto)                   | Devuelve el valor de "montag" syo existe, de lo contrario devuelve el valor "toto"                               |
| nombre (eqLogic, \# [Baño] [Hidrometría] [Humedad] \#)     | Hidrometría de devoluciones                  |

Funciones matematicas
---------------------------

Una caja de herramientas de funciones genéricas también se puede utilizar para
realizar conversiones o cálculos :

-   rand (1,10) : Dar un número aleatorio del 1 al 10.

-   randText (texto1, texto2, texto ... ..) : Devuelve uno de
    textos al azar (texto separado por uno;). No hay
    límite en el número de texto.

-   randomColor (min, max) : Da un color aleatorio entre 2
    terminales (0 =&gt; rojo, 50 =&gt; verde, 100 =&gt; azul).

-   gatillo (control) : Se usa para descubrir el desencadenante del escenario
    o para saber syo es el pedido realizado como parámetro el que tiene
    desencadenó el escenario.

-   triggerValue (control) : Se usa para averiguar el valor de
    desencadenante de escenario.

-   ronda (valor [decimal]) : Redondo arriba, [decimal]
    número de decimales después del punto decimal.

-   impor (valor) : Le permite saber syo un número es impor o no..
    Devuelve 1 syo es impor 0 de lo contrario.

-   mediana (comando1, comando2 ....comandoN) : Devuelve la mediana
    valores.

-   time_op (tiempo, valor) : Le permite realizar operaciones a tiempo,
    con tiempo = tiempo (por ejemplo, : 1530) y valor = valor para agregar o para
    restar en minutos.

-   `time_between (hora, inicio, fin)` : Permite probar syo es un momento
    entre dos valores con `tiempo = time` (por ejemplo, : 1530), `inicio = tiempo`,` fin = tiempo`.
    Los valores iniciales y finales pueden estar a caballo entre la medianoche.

-   `time_diff (fecha1, fecha1 [, formato])` : Se usa para descubrir la diferencia entre 2 fechas (las fechas deben estar en el formato AAALa / MM / DD HH:MM:SS).
    Por defecto (syo no pone nada para el formato), el método devuelve el número total de días. Puedes preguntarlo en segundos (s), minutos (m), horas (h). Ejemplo en segundos `time_diff (2018-02-02 14:55:00,2018-02-25 14:55:00,s)`

-   `formatTime (hora)` : Formatea el retorno de una cadena
    `# tiempo #`.

-   piso (tiempo / 60) : Convierte de segundos a minutos, o
    minutos a horas (piso (tiempo / 3600) por segundos
    en horas)

Y ejemplos prácticos :


| Ejemplo de funcion                  | Resultado devuelto                    |
|--------------------------------------|--------------------------------------|
| randText (es # [sala de estar] [ojo] [temperatura] #; La temperatura es # [sala de estar] [ojo] [temperatura] #; Actualmente tenemos # [sala de estar] [ojo] [temperatura] #) | la función devolverá uno de estos textos al azar en cada ejecución.                           |
| randomColor (40,60)                 | Devuelve un color aleatorio cercano al verde.   
| gatillo (# [Baño] [Hidrometría] [Humedad] #)   | 1 syo es bueno \# \ [Baño \] \ [Hidrometría \] \ [Humedad \] \# que inició el escenario de lo contrario 0  |
| triggerValue (# [Baño] [Hidrometría] [Humedad] #) | 80 syo la hidrometría de \# \ [Baño \] \ [Hidrometría \] \ [Humedad \] \# es 80%.                         |
| redondo (# [Baño] [Hidrometría] [Humedad] # / 10) | Devuelve 9 syo el porcentaje de humedad y 85                     |
| impor (3)                             | Devuelve 1                            |
| mediana (15,25,20)                   | Devuelve 20                           |
| time_op (# tiempo #, -90)               | syo son las 4:50 p.m., regrese : 1 650-1 130 = 1520                          |
| formatTime (1650)                   | Devuelve 4:50 p.m.                        |
| piso (130/60)                      | Devuelve 2 (minutos syo 130 s, u horas syo 130 m)                      |

Pedidos específicos
=========================

Además de los comandos de automatización del hogar, tiene acceso a las siguientes acciones :

-   **Pause** (Sueño) : Pausa de x segundo (s).

-   **variable** (Variable) : Creación / modificación de una variable o valor.
    de una variable.

-   **Eliminar variable** (Delete_variable) : Le permite eliminar una variable.

-   **Guión** (Escenario) : Te permite controlar escenarios. La parte de las etiquetas
    permite enviar etiquetas al escenario, ej. : montag = 2 (ten cuidado allí
    solo use letras de la a a la z. No letras mayúsculas, no
    acentos y sin caracteres especiales). Obtenemos la etiqueta en el
    escenario objetivo con la función de etiqueta (montag). El comando &quot;Restablecer SI&quot; permite restablecer el estado de &quot;SI&quot; (este estado se utiliza para la no repetición de las acciones de un &quot;SI&quot; syo pasa por segunda vez consecutiva en él)

-   **Stop** (Stop) : Detener el escenario.

-   **Attendre** (Espere) : Espere hasta que la condición sea válida.
    (máximo 2 h), el tiempo de espera es en segundos (s).

-   **Ir al diseño** (Gotodesign) : Cambiar el diseño que se muestra en todos
    navegadores por diseño solicitado.

-   **Agregar un registro** (Log) : Le permite agregar un mensaje a los registros.

-   **Crear mensaje** (Mensaje) : Agrega un mensaje en el centro
    de mensajes.

-   **Activar / Desactivar Ocultar / mostrar equipo** (Equipo) : Permite
    modificar las propiedades de un dispositivo
    visible / invisible, activo / inactivo.

-   **Hacer una solicitud** (Ask) : Le permite decirle a Jeedom que pregunte
    una pregunta al usuario. La respuesta se almacena en un
    variable, luego simplemente pruebe su valor. Por el momento,
    solo sms y complementos de holgura son compatibles. Ten cuidado, esto
    la función está bloqueando. Mientras no haya respuesta o el
    no se alcanza el tiempo de espera, el escenario espera.

-   **Detener Jeedom** (Jeedom_poweroff) : Pídale a Jeedom que cierre.

-   **Reiniciar Jeedom** (Jeedom_reboot) : Pedirle a Jeedom que reinicie.

-   **Devolver un texto / datos** (Scenario_return) : Devuelve un texto o un valor
    para una interacción por ejemplo.

-   **Icono** (Icono) : Permite cambiar el ícono de representación del escenario.

-   **Alerte** (Alerta) : Le permite mostrar un pequeño mensaje de alerta en todos
    navegadores que tienen abierta una página de Jeedom. Usted puede
    más, elige 4 niveles de alerta.

-   **Pop-up** (Emergente) : Permite mostrar una ventana emergente que debe ser absolutamente
    validado en todos los navegadores que tienen una página abierta de libertad.

-   **Rapport** (Informe) : Exportar una vista en formato (PDF, PNG, JPEG
    o SVG) y enviarlo a través de un comando de tipo de mensaje.
    Tenga en cuenta que syo su acceso a Interny está en HTTPS sin firmar, esto
    la funcionalidad no funcionará. Se requiere HTTP o HTTPS firmado.

-   **Eliminar bloque IN / La programado** (Remove_inat) : Le permite eliminar el
    programación de todos los bloques IN y La del escenario.

-   **Evento** (Event) : Le permite insertar un valor en un comando de tipo de información arbitrariamente

-   **Tag** (Tag) : Le permite agregar / modificar una etiqueta (la etiqueta solo existe durante la ejecución actual del escenario a diferencia de las las variables que sobreviven al final del escenario)

Plantilla de escenario
====================

Esta funcionalidad le permite transformar un escenario en una plantilla para
por ejemplo, aplícalo en otro Jeedom o compártelo en el
Mercado. También es a partir de ahí que puedes recuperar un escenario
del mercado.

![scenario15](../images/scenario15.JPG)

Entonces verás esta ventana :

![scenario16](../images/scenario16.JPG)

La partir de ahí, tienes la posibilidad :

-   Enviar una plantilla a Jeedom (archivo JSON de antemano
    recuperado),

-   Consulte la lista de escenarios disponibles en el mercado,

-   Crear una plantilla a partir del escenario actual (no olvides
    dar un nombre),

-   Para consultar las plantillas actualmente presentes en su Jeedom.

Al hacer clic en una plantilla, obtienes :

![scenario17](../images/scenario17.JPG)

En la cima puedes :

-   **Partager** : compartir la plantilla en el mercado,

-   **Supprimer** : eliminar plantilla,

-   **Descargar** : recuperar la plantilla como un archivo JSON
    para enviarlo de vuelta a otro Jeedom por ejemplo.

La continuación, tiene la parte para aplicar su plantilla a
escenario actual.

Desde un Jeedom a otro o de una instalación a otra,
los pedidos pueden ser diferentes, Jeedom te pregunta el
correspondencia de órdenes entre los presentes durante la creación
de la plantilla y los presentes en casa. Solo necesita completar el
las órdenes de partido se aplican.

Adición de la función php
====================

> **IMPORTANT**
>
> Agregar funciones PHP está reservado para usuarios avanzados. El más mínimo error puede bloquear tu Jeedom

## Configurar

Vaya a la configuración de Jeedom, luego OS / DB e inicie el editor de archivos.

Vaya a la carpeta de datos, luego php y haga clic en el archivo user.function.class.php.

Es en esta clase que debe agregar sus funciones, encontrará allí un ejemplo de función básica.

> **IMPORTANT**
>
> Syo tiene un problema, siempre puede volver al archivo original y copiar el contenido de user.function.class.sample.php en user.function.class.php
