# Apuntes_U1
Apuntes de la unidad 1
Unidad I: Interfaz Gráfica de Usuario (GUI)
La Interfaz Gráfica de Usuario es el conjunto de elementos visuales que permiten la interacción entre el humano y la máquina. En el ecosistema de Flet, esto se abstrae mediante una estructura de árbol de controles que se renderizan de forma nativa.

1.1 Creación de Interfaz Gráfica para Usuarios
La creación de una GUI no es solo "dibujar" botones; es un proceso de arquitectura de software. En Flet, la creación se basa en el concepto de Controles (Widgets).

El Contenedor Raíz (Page): Toda interfaz en Flet comienza con el objeto page. Es el lienzo donde se montan los demás elementos.

Estructura Jerárquica: Las interfaces se construyen anidando componentes. Un Column o un Row actúan como contenedores de diseño (layout) que organizan otros controles.

Declaratividad: A diferencia de librerías antiguas (como Tkinter), Flet utiliza un enfoque declarativo. Tú defines cómo quieres que se vea el estado de la interfaz, y el framework se encarga de actualizar los píxeles.

1.2 Tipos de Eventos
Los eventos son señales enviadas por el sistema o por la interacción del usuario que notifican que "algo ha sucedido". En el desarrollo de GUIs, podemos categorizarlos de la siguiente manera:

Eventos de Entrada (Input Events): * Click/Tap: El más común. Activado al presionar un botón.

Cambio (Change): Ocurre cuando el usuario escribe en un campo de texto o mueve un slider.

Eventos de Estado (State Events): * Carga (On Load): Cuando la página termina de renderizarse.

Redimensión (On Resize): Cuando el usuario cambia el tamaño de la ventana.

Eventos de Enfoque (Focus Events):

On Focus / On Blur: Cuando un elemento gana o pierde la selección del cursor.

1.3 Manejo de Eventos
El manejo de eventos (Event Handling) es el mecanismo de programación que "escucha" los eventos y ejecuta una función de respuesta (llamada Callback).

En Flet, el manejo de eventos sigue este flujo:

Definición del Handler: Se crea una función (normalmente con un parámetro e que contiene los datos del evento).

Asignación: Se vincula la función a la propiedad específica del control (ej. on_click=mi_funcion).

Actualización de la UI: Dentro del manejador, es crucial llamar a page.update() para que los cambios realizados en el código se reflejen visualmente en la pantalla del usuario.

Nota técnica: Flet maneja los eventos de forma asíncrona por defecto, lo que permite que la interfaz no se "congele" mientras se procesan datos pesados.

1.4 Manejo de Componentes Gráficos de Control
Los componentes de control son los ladrillos de la interfaz. Se dividen según su propósito:

A. Controles de Entrada de Datos
Permiten al usuario enviar información al programa.

TextField: Para entradas de texto.

Checkbox y Switch: Para opciones booleanas (sí/no).

Dropdown: Para seleccionar una opción de una lista.

B. Controles de Visualización
Muestran información al usuario.

Text: Etiquetas de texto con formato.

Image: Despliegue de recursos visuales.

Icon: Representaciones gráficas simbólicas.

C. Controles de Layout (Organización)
Determinan la posición y el flujo de los elementos.

Container: Permite añadir márgenes, bordes, colores de fondo y alineación.

Stack: Permite encimar elementos (uno sobre otro).

ListView: Para manejar listas largas de elementos con scroll.

Bibliografía (Formato APA)
Flet. (s.f.). Introduction to Flet. Recuperado 24 de febrero de 2024, de https://flet.dev/docs/

Flet. (s.f.). Controls Reference. Recuperado 24 de febrero de 2024, de https://flet.dev/docs/controls/

Sommerville, I. (2011). Ingeniería de software (9.ª ed.). Pearson Educación.

Python Software Foundation. (s.f.). Tkinter — Python interface to Tcl/Tk. Recuperado de https://docs.python.org/3/library/tkinter.html
