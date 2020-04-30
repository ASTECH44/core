# Diseño
**Inicio → Diseño**

Esta página le permite configurar la visualización de toda su domótica de una manera muy fina.
Lleva tiempo pero su único límite es tu imaginación.

> **Tip**
>
> Es posible ir directamente a un diseño gracias al submenú.

> **Important**
>
> Todas las acciones se realizan haciendo clic derecho en esta página, tenga cuidado de hacerlo bien en el diseño. Al crear, debe hacerlo en el medio de la página (para asegurarse de estar en el diseño).

En el menú (clic derecho), encontramos las siguientes acciones :

- **Designs** : Muestra la lista de sus diseños y le permite acceder a ellos..
- **Edition** : Cambiar al modo de edición.
- **Pantalla completa** : Le permite usar toda la página web, lo que eliminará el menú Jeedom de la parte superior.
- **Añadir gráfico** : Agregar un gráfico.
- **Añadir texto / html** : Le permite agregar texto o código html / JavaScript.
- **Agregar escenario** : Agregar un escenario.
- **Agregar enlace**
    - **Hacia una vista** : Agregar un enlace a una vista.
    - **Hacia un diseño** : Agregar un enlace a otro diseño.
- **Agregar equipo** : Agrega equipo.
- **Añadir pedido** : Agregar un pedido.
- **Añadir imagen / cámara** : Le permite agregar una imagen o una transmisión desde una cámara.
- **Agregar área** : Le permite agregar un área transparente en la que se puede hacer clic que puede ejecutar una serie de acciones al hacer clic (dependiendo o no del estado de otro comando).
- **Agregar resumen** : Agrega información de un objeto o resumen general.
- **Affichage**
    - **Aucune** : No muestra ninguna cuadrícula.
    - **10x10** : Muestra una cuadrícula de 10 por 10.
    - **15x15** : Muestra una cuadrícula de 15 por 15.
    - **20x20** : Muestra una cuadrícula de 20 por 20.
    - **Magnetizar los elementos** : Agrega magnetización entre los elementos para que sea más fácil pegarlos.
    - **Imán en la rejilla** : Agregue una magnetización de los elementos a la cuadrícula (atención : dependiendo del zoom del elemento, esta funcionalidad puede funcionar más o menos).
    - **Ocultar elemento resaltado** : Ocultar resaltado alrededor de elementos.
- **Eliminar diseño** : Eliminar diseño.
- **Crea un diseño** : Le permite agregar un nuevo diseño.
- **Diseño duplicado** : Duplica el diseño actual.
- **Configura el diseño** : Acceso a la configuración del diseño..
- **Sauvegarder** : Guarde el diseño (tenga en cuenta que también hay copias de seguridad automáticas durante ciertas acciones).

> **Important**
>
> La configuración de los elementos de diseño se realiza haciendo clic en ellos..

## Configuración de diseño

Encontrado aquí :

- **General**
    - **Nom** : El nombre de su diseño.
    - **Position** : La posición del diseño en el menú.. Le permite ordenar los diseños..
    - **Fondo transparente** : Hace el fondo transparente. Atención si la casilla está marcada, no se usa el color de fondo.
    - **Color de fondo** : Diseño de color de fondo.
    - **Código de acceso* : Código de acceso a su diseño (si está vacío, no se requiere código).
    - **Icono** : Un icono para ello (aparece en el menú de opciones de diseño).
    - **Image**
        - **Envoyer** : Le permite agregar una imagen de fondo al diseño.
        - **Eliminar imagen** : Eliminar imagen.
- **Tailles**
    - **Tamaño (WxH)** : Le permite establecer el tamaño en píxeles de su diseño..

## Configuración general de elementos.

> **Note**
>
> Dependiendo del tipo de elemento, las opciones pueden cambiar.

### Configuraciones de pantalla comunes

- **Profondeur** : Le permite elegir el nivel de profundidad
- **Posición X (%)** : Coordenada horizontal del elemento..
- **Posición Y (%)** : Coordenada vertical del elemento..
- **Ancho (px)** : Ancho del elemento en píxeles.
- **Altura (px)** : Altura del elemento en píxeles.

### Remove

Eliminar elemento

### Duplicado

Le permite duplicar el elemento.

### Cerradura

Le permite bloquear el elemento para que ya no se pueda mover o cambiar de tamaño.

## Gráfico

### Configuraciones de pantalla específicas

- **Período** : Le permite elegir el período de visualización
- **Mostrar subtítulo** : Muestra la leyenda..
- **Mostrar navegador** : Muestra el navegador (segundo gráfico más claro debajo del primero).
- **Mostrar selector de período** : Muestra el selector de período en la esquina superior izquierda..
- **Mostrar barra de desplazamiento** : Muestra la barra de desplazamiento..
- **Fondo transparente** : Hace el fondo transparente.
- **Bordure** : Le permite agregar un borde, tenga cuidado, la sintaxis es HTML (tenga cuidado, debe usar la sintaxis CSS, por ejemplo : sólido 1px negro).

### Configuración avanzada

Le permite elegir los comandos para graficar.

## Text / html

### Configuraciones de pantalla específicas

- **Icono** : Icono que se muestra delante del nombre del diseño.
- **Color de fondo** : le permite cambiar el color de fondo o hacerlo transparente, no olvide cambiar &quot;Predeterminado&quot; a NO.
- **Color del texto** : le permite cambiar el color de los iconos y textos (tenga cuidado de establecer el valor predeterminado en No)..
- **Alrededor de los ángulos** : permite redondear los ángulos (no olvides poner%, ex 50%).
- **Bordure** : le permite agregar un borde, tenga cuidado con la sintaxis HTML (debe usar la sintaxis CSS, por ejemplo : sólido 1px negro).
- **Tamaño de fuente** : le permite cambiar el tamaño de fuente (ex 50%, debe poner el signo%).
- **Alineación de texto** : permite elegir la alineación del texto (izquierda / derecha / centrado).
- **Gras** : texto en negrita.
- **Texte** : Texto en código HTML que estará en el elemento.

> **Important**
>
> Si coloca código HTML (especialmente Javascript), tenga cuidado de verificarlo antes porque puede hacerlo si hay un error o si sobrescribe un componente de Jeedom y bloquea completamente el diseño y solo tendrá que eliminarlo. directamente en la base de datos.

## Guión

*No hay configuraciones de visualización específicas*

## Enlace

### Configuraciones de pantalla específicas

- **Nom** : Apellidobre del enlace (texto mostrado).
- **Lien** : Enlace al diseño o vista en cuestión.
- **Color de fondo** : Le permite cambiar el color de fondo o hacerlo transparente, no olvide cambiar &quot;Predeterminado&quot; a NO.
- **Color del texto** : Le permite cambiar el color de los iconos y textos (tenga cuidado de establecer el valor predeterminado en No).
- **Redondee los ángulos (no olvide poner%, ex 50%)** : Permite redondear los ángulos, no olvides poner el%.
- **Borde (sintaxis CSS de atención, ej. : sólido 1px negro)** : Le permite agregar un borde, tenga cuidado con la sintaxis es HTML.
- **Tamaño de fuente (ex 50%, debe poner el signo%)** : Le permite cambiar el tamaño de fuente.
- **Alineación de texto** : Permite elegir la alineación del texto (izquierda / derecha / centrado).
- **Gras** : Texto en negrita.

## Equipo

### Configuraciones de pantalla específicas

- **Mostrar nombre de objeto** : Marque para mostrar el nombre del objeto principal del dispositivo.
- **Ocultar nombre** : Marque para ocultar el nombre del equipo.
- **Color de fondo** : Le permite elegir un color de fondo personalizado, mostrar el equipo con un fondo transparente o usar el color predeterminado.
- **Color del texto** : Le permite elegir un color de fondo personalizado o usar el color predeterminado.
- **Arrondis** : Valor en píxeles del redondeo de los ángulos del mosaico del equipo..
- **Bordure** : Definición CSS de un borde de mosaico de equipo. Ex : 1px negro sólido.
- **Opacité** : Opacidad del mosaico del equipo, entre 0 y 1. Atención : se debe definir un color de fondo.
- **CSS personalizado** : Reglas CSS para aplicar en el equipo.
- **Aplicar CSS personalizado en** : Selector de CSS en el que aplicar CSS personalizado.

### Comandos

La lista de comandos presentes en el equipo le permite, para cada comando,:
- Ocultar nombre del comando.
- Comando Ocultar.
- Mostrar el pedido con un fondo transparente.

### Configuración avanzada

Muestra la ventana de configuración avanzada del equipo (ver documentación **Resumen de domótica**).

## Orden

*No hay configuraciones de visualización específicas*

### Configuración avanzada

Muestra la ventana de configuración avanzada del equipo (ver documentación **Resumen de domótica**).

## Imagenn / Cámara

### Configuraciones de pantalla específicas

- **Afficher** : Define lo que desea mostrar, imagen fija o transmisión desde una cámara.
- **Image** : Le permite enviar la imagen en cuestión (si ha elegido una imagen).
- **Cámara** : Cámara para mostrar (si elige cámara).

## Zona

### Configuraciones de pantalla específicas

- **Tipo de area** : Aquí es donde eliges el tipo de área : Macro individual, macro binaria o widget al pasar el mouse.

### Macro individual

En este modo, un clic en la zona realiza una o más acciones. Aquí solo debe indicar la lista de acciones que debe hacer al hacer clic en el área.

### Macro binaria

En este modo, Jeedom ejecutará las acciones de encendido o apagado dependiendo del estado del comando que usted indique.. Ex : si el comando vale 0, entonces Jeedom ejecutará la (s) acción (es) activada (s) de lo contrario ejecutará la (s) acción (es) desactivada (s)

- **Información binaria** : Comando que proporciona el estado que se debe verificar para decidir qué acción hacer (activar o desactivar).

Solo tiene que poner las acciones a realizar para Activar y Desactivar.

### Widget de desplazamiento

En este modo, al pasar el mouse por encima o al hacer clic en el área Jeedom, se mostrará el widget en cuestión.

- **Equipement** : Widget para mostrar al pasar el mouse o al hacer clic.
- **Mostrar en paso elevado** : Si está marcado, muestra el widget al pasar el mouse.
- **Ver en un clic** : Si está marcado, el widget se muestra al hacer clic.
- **Position** : Le permite elegir dónde aparecerá el widget (predeterminado abajo a la derecha).

## Resumen

### Configuraciones de pantalla específicas

- **Lien** : Le permite indicar el resumen a mostrar (General para el global, de lo contrario indique el asunto).
- **Color de fondo** : Le permite cambiar el color de fondo o hacerlo transparente, no olvide cambiar &quot;Predeterminado&quot; a NO.
- **Color del texto** : Le permite cambiar el color de los iconos y textos (tenga cuidado de establecer el valor predeterminado en No).
- **Redondee los ángulos (no olvide poner%, ex 50%)** : Permite redondear los ángulos, no olvides poner el%.
- **Borde (sintaxis CSS de atención, ej. : sólido 1px negro)** : Le permite agregar un borde, tenga cuidado con la sintaxis es HTML.
- **Tamaño de fuente (ex 50%, debe poner el signo%)** : Le permite cambiar el tamaño de fuente.
- **Gras** : Texto en negrita.

## Preguntas frecuentes

>**Ya no puedo editar mi diseño**
>Si ha colocado un widget o una imagen que toma casi todo el diseño, debe hacer clic fuera del widget o imagen para acceder al menú haciendo clic con el botón derecho.

>**Eliminar un diseño que ya no funciona**
>En la parte de administración, luego OS / DB, haga &quot;select * from planHeader&quot;, recupere la identificación del diseño en cuestión y haga una &quot;eliminación de planHeader donde id = # TODO #&quot; y &quot;delete from plan where planHeader_id = # todo # &quot;reemplazando # TODO # con la identificación de diseño encontrada previamente.
