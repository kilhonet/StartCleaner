# StartCleaner

**Gestor gratuito de inicio para Windows: muestra en una sola pantalla los programas, tareas programadas y servicios que arrancan con el equipo, y los ordena de forma segura desactivándolos en lugar de borrarlos.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · Español · [Português (Brasil)](README.pt-BR.md) · [Français](README.fr.md)

> Este documento es una traducción. Si hay alguna diferencia, la [versión en coreano](README.ko.md) es la que prevalece.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Version](https://img.shields.io/badge/version-2.0.0-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/startcleaner?lang=es)

![Pantalla de StartCleaner](images/startcleaner-en.webp)

## Descripción general

Cada vez que enciende el PC, se abren con él aplicaciones de mensajería, asistentes de actualización y todo tipo de servicios. Cada uno es pequeño, pero juntos hacen que el arranque sea más lento y ocupan memoria.

StartCleaner reúne todo lo que se inicia automáticamente desde cuatro lugares — la carpeta de **Inicio**, el **Registro**, las **Tarea**s programadas y los **Servicio**s — y lo muestra en una sola lista. Seleccione un elemento que no necesite y pulse **Desactivar**: a partir del siguiente arranque ya no se iniciará. No se borra nada, solo se apaga, así que con un clic en **Habilitar** vuelve exactamente como estaba.

Los componentes que Windows realmente necesita están ocultos de antemano en la lista, por lo que es difícil desactivar por error algo que no se debe tocar.

## Funciones principales

- **Todo en una lista** — Vea en un solo lugar los elementos de inicio automático repartidos entre las carpetas de inicio, el registro, el Programador de tareas y los servicios.
- **Desactivar en lugar de borrar** — Apáguelos con **Desactivar** y recupérelos cuando quiera con **Habilitar**.
- **Elementos básicos de Windows ocultos** — Los componentes de Windows que no deben desactivarse no aparecen en la lista. Con conexión a internet, descarga la lista más reciente de elementos que ocultar.
- **Nombres fáciles de reconocer** — Muestra el nombre del producto y el icono de cada programa en lugar del nombre de archivo.
- **Eliminar del todo** — Las entradas que dejan programas que ya no usa se pueden desactivar y luego eliminar por completo de la lista.
- **Buscar información** — Haga doble clic en un elemento que no reconozca para buscarlo en la web.
- **Guardar la lista** — Guarda en un archivo de texto todos los elementos de inicio actuales.
- **Modo oscuro** — Los colores siguen el modo de aplicación de Windows (claro · oscuro).
- **9 idiomas** — Coreano · inglés · japonés · chino · ruso · italiano · francés · español · árabe.

## Descarga / Instalación

| Tipo | Enlace |
|---|---|
| Instalador | [Descargar](https://down.kilho.net/startcleaner?lang=es) |
| Portátil (ZIP) | [Descargar](https://down.kilho.net/startcleaner?lang=es&nosetup) |

El instalador abre StartCleaner en cuanto termina la instalación. Para la versión portátil, descomprima el ZIP y ejecute `StartCleaner.exe`. Las dos versiones tienen las mismas funciones.

Cambiar los elementos de inicio automático requiere permisos de administrador, por lo que Windows muestra una ventana de confirmación de administrador al ejecutarlo. Pulse **Sí**.

## Uso

### Primeros pasos

1. Ejecute StartCleaner y pulse **Sí** en la ventana de confirmación de administrador.
2. Los elementos que se inician con el equipo aparecen en la lista con su **Programa** y su **Origen**.
3. Haga clic una vez en el elemento que quiera apagar y pulse **Desactivar** abajo.
4. La fila se vuelve gris y el botón cambia a **Habilitar**. A partir del próximo inicio de Windows, ese elemento no se ejecutará.
5. Para volver a encenderlo, haga clic en la misma fila y pulse **Habilitar**.

Los elementos que desactiva no desaparecen de la lista de inmediato: se quedan en su sitio, en gris, para que pueda deshacer al momento lo que acaba de hacer.

### Distribución de la pantalla

| Elemento | Función |
|---|---|
| Pestaña **Inicio** | La pantalla con la lista de inicio automático |
| Logotipo de KILHO.net | Abre la página de StartCleaner |
| Columna **Programa** | Icono y nombre del programa (el nombre del producto, si lo tiene) |
| Columna **Origen** | Dónde está registrado el elemento — un icono y un nombre |
| Fila gris | Un elemento desactivado |
| **Todos los programas** | Al marcarla, muestra todo, incluidos los elementos desactivados |
| **Desactivar** / **Habilitar** | Apaga o enciende el elemento seleccionado. Aparece en gris hasta que se selecciona un elemento |
| Menú del clic derecho | **Eliminar** (solo elementos desactivados) · **Guardar lista** |

**Origen** — desde dónde se inicia cada elemento

| Origen | Significado |
|---|---|
| **Inicio** | Accesos directos y programas de la carpeta "Inicio" del menú Inicio (todos los usuarios · usuario actual) |
| **Registro** | Elementos que un programa registró para "ejecutarse al iniciar sesión" al instalarse |
| **Tarea** | Tareas registradas en el Programador de tareas que se ejecutan en momentos fijos (búsqueda de actualizaciones, etc.) |
| **Servicio** | Servicios en segundo plano que se inician automáticamente al arrancar Windows |

### Qué hacer cuando…

**Quiere saber qué se inicia junto con el PC**
Basta con ejecutar StartCleaner. Los elementos de inicio automático repartidos en cuatro lugares se reúnen en una lista, y la columna **Origen** le indica dónde está registrado cada uno. Si acaba de instalar un programa, pulse **F5** para volver a cargar la lista.

**No quiere que la mensajería o un asistente de actualización se abran cada vez que inicia sesión**
Haga clic en ese programa en la lista y pulse **Desactivar**. El programa no se elimina y sigue funcionando como siempre; solo deja de abrirse solo al iniciar Windows. Ábralo usted cuando lo necesite. Los elementos de **Inicio** y **Registro** también aparecen como "Deshabilitado" en la pestaña **Aplicaciones de arranque** del Administrador de tareas.

**Quiere volver a encender un elemento desactivado**
Marque **Todos los programas** y los elementos que desactivó antes aparecerán como filas grises. Haga clic en la fila y pulse **Habilitar**: se volverá a ejecutar desde el siguiente arranque.

**Quiere apagar tareas de actualización que se ejecutan en segundo plano**
Las filas cuyo **Origen** es **Tarea** son tareas registradas en el Programador de tareas. Aquí se encuentran muchas búsquedas de actualizaciones de navegadores y programas. Seleccione la tarea que quiere detener y pulse **Desactivar**: no se ejecutará aunque llegue su hora programada.

**Quiere que un servicio innecesario no arranque con el equipo**
Si pulsa **Desactivar** en una fila de **Servicio**, ese servicio no se iniciará al arrancar Windows, ni siquiera si otro programa lo llama. Si pulsa **Habilitar**, pasará a iniciarse automáticamente con Windows. Conviene comprobar a qué programa pertenece un servicio antes de desactivarlo — si no lo reconoce, búsquelo primero como se explica a continuación.

**No sabe qué es un elemento**
Haga doble clic en la fila y se abrirá el navegador con información sobre ese elemento. Úselo para comprobar qué hace un programa antes de desactivarlo.

**Quedan entradas de inicio de un programa que ya desinstaló**
Si el programa ya no está pero su nombre sigue en la lista, primero cambie la fila a **Desactivar** y luego haga clic derecho → **Eliminar**. Pulse **Sí** en la confirmación y el elemento se eliminará por completo de la lista. Los elementos eliminados no se pueden recuperar, así que elimine solo lo que esté seguro de no necesitar. El menú **Eliminar** no aparece en los elementos que siguen activos — lo más seguro es desactivarlo primero, usar el PC unos días y después eliminarlo.

**Quiere eliminar un servicio por completo**
Solo se pueden **Eliminar** los servicios cambiados a **Desactivar**. Un servicio en ejecución se detiene antes de eliminarse. Después aparece el aviso "Un servicio en ejecución se elimina por completo después de reiniciar": reinicie el PC una vez y quedará limpio del todo.

**Servicios en gris en Todos los programas**
**Todos los programas** también muestra en filas grises los servicios configurados para iniciarse solo cuando se necesitan. Si pulsa **Habilitar** en uno de ellos, se iniciará automáticamente cada vez que arranque Windows, así que déjelos como están salvo que los haya desactivado usted.

**Quiere guardar el estado actual antes de limpiar**
Haga clic derecho en la lista → **Guardar lista** y elija dónde guardarla. Todos los elementos de inicio automático, incluidos los elementos básicos de Windows ocultos en la lista, se guardan en un archivo de texto. Sirve para comparar el antes y el después, o para compararlo con otro PC.

**Por qué los elementos básicos de Windows no están en la lista**
Los servicios y tareas que Windows necesita para funcionar — audio, red, seguridad, etc. — están ocultos en la lista desde el principio. Desactivarlos podría impedir que Windows funcione bien, así que StartCleaner ni siquiera deja tocarlos. Siguen ocultos aunque marque **Todos los programas**.

**Recorrer la lista con el teclado**
Use **↑** · **↓** para moverse entre filas; la lista se desplaza para que la fila seleccionada siempre esté a la vista. **F5** vuelve a cargar la lista.

**Nombres cortados por ser demasiado largos**
Arrastre el borde de la ventana para ensancharla y la columna **Programa** se ensanchará con ella. También puede arrastrar el borde entre los encabezados de columna para ajustar el ancho usted mismo.

**Lo ejecuta de nuevo cuando ya está abierto**
Solo se ejecuta un StartCleaner a la vez. Si lo ejecuta otra vez con la ventana abierta, no se abre una copia nueva: la ventana que ya está abierta pasa al frente (y se restaura si estaba minimizada).

## Configuración

No hay nada que configurar. StartCleaner sigue por sí mismo lo siguiente:

| Elemento | Sigue |
|---|---|
| Idioma | La configuración regional de Windows (inglés si el idioma no es compatible) |
| Colores | El modo de aplicación de Windows (claro · oscuro) — los cambios se aplican al momento, incluso con StartCleaner abierto |

## Requisitos

- Windows 10 · Windows 11 (64 bits)
- Permisos de administrador — necesarios para cambiar los elementos de inicio automático. Al ejecutarlo aparece una ventana de confirmación.
- No hace falta instalar otros componentes.
- La conexión a internet solo se usa para los avisos de nuevas versiones y para descargar la lista de elementos básicos de Windows que ocultar. Sin conexión, funciona igual con su lista integrada.

## Actualizaciones

StartCleaner **no** se actualiza solo. Al iniciarse comprueba si hay una versión nueva y muestra un aviso; si pulsa **[Sí]**, abre la página de descarga y cierra el programa. Las versiones nuevas se publican manualmente tras una verificación interna y se anuncian en la [página de StartCleaner](https://kilho.net/startcleaner). Consulte el [aviso sobre la política de actualizaciones](https://en.kilho.net/archives/notice/2940).

## Licencia

StartCleaner es **freeware**. Puede usarlo gratis y sin restricciones en cualquier lugar — en la oficina, en casa, en organismos públicos o en la escuela — y redistribuirlo libremente.

## Enlaces

- Sitio web: <https://kilho.net/startcleaner>
- Foro: <https://kilho.top/forum/qna>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
