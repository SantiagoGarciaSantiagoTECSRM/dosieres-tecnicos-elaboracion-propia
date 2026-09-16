
>[!WARNING]
>-EN ELABORACION ESTE REPOSITORIO AUN NO ESTA TERMINADO-<br>
>El dosier de [Manual de procedimientos], nunca esta terminado del todo, se revisa y amplia periodicamente.   
># Ultima revisión: 16-09-2026
 

<br>

---

*   **📚 Nombre del Dossier:** Manual Bash Linux
*   **🐧 Sistema Operativo Base:** Linux Mint 22.2
*   **✍️ Autor:** Fernando López Hernández            
*   **♻️ Re-maquetado:** Santiago Garcia Santiago
*   **✅ Estado:** Completado / Técnico



*|Descripcion:<br>
*|Rescatado de un dominio actualmente inhabilitado. Re-maquete el documento
*|para que pudiera ser manejable en los navegadores/visores actuales 
*|(el original era solo para "impresión")

---


<br>

<a href="https://github.com/SantiagoGarciaSantiagoTECSRM/dosieres-tecnicos-elaboracion-propia/blob/main/README.md">[📂 Indice Repositorio]</a> | [indice_contenidos](#dosier_03)  


<table style="margin: 0 auto; width: 50%; border-collapse: collapse; align:center;"">
  <tr>
    <th style="border: 1px solid black; padding: 8px;">  &emsp; &emsp;&emsp; &emsp; &emsp; &emsp; &emsp;  &emsp; &emsp; &emsp; &emsp;&emsp;|Instalacion de Retro_Arch en Linux| &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;  &emsp;  &emsp; &emsp; &emsp; </th> 
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;">
     <a href="https://github.com/SantiagoGarciaSantiagoTECSRM/dosieres-tecnicos-elaboracion-propia/blob/manual-bash-linux/%5Bpost%5DManual_Bash_Linux_DX%5BRepositorio_def%5D.pdf">[post]Manual_Bash_Linux_DX[Repositorio_def].pdf</a>
 
  </tr>
  
</table>
<hr>
<br>

---

<a name="dosier_03">Indice contenidos:</a> &emsp; (Enlace de descarga al comienzo de este documento)

## 🔍 Índice del Contenido

### 📑 Tema 01:   [Introducción a Bash] 
* |El shell que estamos usando|
* 🔶 |Expansión de nombres de ficheros y directorios|
    *   `🔸` Los comodines
    *   `🔸` El comodín tilde
    *   `🔸` El comodín llaves
    *   `🔸` Comodines extendidos
* |Los comandos internos de Bash|
* 🔶 |Redirecciones y pipes|
    *   `🔸` Operadores de redirección
    *   `🔸` Pipes
* |Ejecución secuencial y concurrente de comandos|
* 🔶 |Caracteres especiales y entrecomillado|
    *   `🔸` Entrecomillado
    *   `🔸` Caracteres de escape
    *   `🔸` Entrecomillar los entrecomillados
    *   `🔸` Texto de varias líneas

### 📑 Tema 02:   [Combinaciones de teclas]
* 🔶 |El historial de comandos|
     *   `🔸` El comando fc
     *   `🔸` Ejecutar comandos anteriores
     *   `🔸` Las teclas de control del terminal
* 🔶 |Modos de edición en la línea de comandos|
     *   `🔸` Moverse por la línea   
     *   `🔸` Borrar partes de la línea
     *   `🔸` Buscar en el historial
     *   `🔸` Autocompletar con el tabulador
* |La librería readline|
* 🔶 |El fichero de configuración|
     *   `🔸` Combinaciones de teclas
     *   `🔸` Variables de readline
     *   `🔸` Asignación de teclas de sesión

### 📑 Tema 03:   [Personalizar el entorno]
* |Los ficheros de configuración de Bash|
* |Los alias|
* |Las opciones de Bash|
* 🔶 |Las variables de entorno|
     *   `🔸` Variables y entrecomillado
     *   `🔸` Personalizar el prompt
     *   `🔸` Variables de entorno internas
     *   `🔸` Exportar variables


### 📑 Tema 04:   [Programación básica del shell]
* 🔶 |Scripts y funciones|
    *   `🔸` Scripts
    *   `🔸` Funciones
    *   `🔸` Orden de preferencia de los símbolos de Bash
* 🔶 |Variables del shell|
   *   `🔸` Los parámetros posiciónales
   *   `🔸` Variables locales y globales
   *   `🔸` Las variables $*, $@ y $#
   *   `🔸` Expansión de variables usando llaves
* 🔶 |Operadores de cadena|
   *   `🔸` Operadores de sustitución
   *   `🔸` Operadores de búsqueda de patrones
   *   `🔸` El operador longitud
* |Sustitución de comandos|

### 📑 Tema 05:   [Control de flujo]
* 🔶 |Las sentencias condicionales|
    *   `🔸` Las sentencias if, elif y else
    *   `🔸` Los códigos de terminación
    *   `🔸` Las sentencias return y exit
    *   `🔸` Operadores lógicos y códigos de terminación
    *   `🔸` Test condicionales
    *   `🔸` Comparación de cadenas
    *   `🔸` Comparación numérica de enteros
    *   `🔸` Comprobar atributos de ficheros
* |El bucle for y el comando xargs|
* |Los bucles while y until|
* |La sentencia case|
* |La sentencia select|

### 📑 Tema 06:   [Opciones de la línea decomandos expresiones aritméticas y arrays]
* 🔶 |Opciones de la línea de comandos|
    *   `🔸` La sentencia shift
    *   `🔸` El comando interno getopts
    *   `🔸` Variables con tipo
* 🔶 |Expresiones aritméticas|
    *   `🔸` Similitud con las expresiones aritméticas C
    *   `🔸` El comando interno let
    *   `🔸` Sentencias de control de flujo aritméticas
    *   `🔸` Arrays

### 📑 Tema 07:   [Redirecciones]
* 🔶 |Redirecciones|
    *   `🔸` Los descriptores de fichero
    *   `🔸` El comando exec
    *   `🔸` Here documents
* 🔶 |Entrada y salida de texto|
    *   `🔸` El comando interno echo
    *   `🔸` El comando interno printf
    *   `🔸` El comando interno read
* |Los bloques de comandos|
* |Los comandos comand, builtin y enable|
* |El comando interno eval|

### 📑 Tema 08:   [Manipular texto]
* 🔶 |Herramientas de manipulación de texto|
    *   `🔸` Edición de stream con sed
    *   `🔸` Las instrucciones
    *   `🔸` Instrucciones como argumentos
    *   `🔸` El fichero de instrucciones
    *   `🔸` Suprimir la salida automática
* 🔶 |Generación de informes con awk|
    *   `🔸` Ejecutar awk
    *   `🔸` Instrucciones awk
    *   `🔸` Combinar sed y awk
* 🔶 |Expresiones regulares|
    *   `🔸` Caracteres y metacaracteres
    *   `🔸` Los metacaracteres posicionales
    *   `🔸` Extensión de la expresión regular
    *   `🔸` Agrupar expresiones regulares y alternativas
* 🔶 |Programación con sed|
    *   `🔸` El pattern space y holding space
    *   `🔸` Direccionamiento
    *   `🔸` Agrupar procedimientos
    *   `🔸` Comentarios
    *   `🔸` El procedimiento de sustitución
    *   `🔸` Procedimientos para insertar, añadir y cambiar
    *   `🔸` Imprimir el número de línea
    *   `🔸` Leer y escribir ficheros
* 🔶 |Control de flujo básico|
    *   `🔸` Pattern space multilínea
    *   `🔸` Añadir línea
    *   `🔸` Borrar línea
    *   `🔸` Imprimir línea
    *   `🔸` El bucle multilínea
    *   `🔸` Holding space
    *   `🔸` Invertir la entrada
    *   `🔸` Convertir a mayúsculas
    *   `🔸` Bloques de texto
* 🔶 |Control de flujo avanzado|
    *   `🔸` El procedimiento b
    *   `🔸` El procedimiento t
* 🔶 |Programación con awk|
    *   `🔸` El bucle de proceso
    *   `🔸` Variables del sistema
    *   `🔸` Los campos del registro
    *   `🔸` Los registros
    *   `🔸` Expresiones
    *   `🔸` Formatear la salida
    *   `🔸` Paso de variables como argumentos
    *   `🔸` Sentencias de control de flujo
    *   `🔸` Arrays
    *   `🔸` El operador in
    *   `🔸` Parsear los datos de un array
    *   `🔸` Arrays multidimensionales
    *   `🔸` Variables del sistema que son arrays
* 🔶 |Funciones|
    *   `🔸` Funciones internas
    *   `🔸` Funciones personalizadas
* 🔶 |Redirecciones y pipes|
    *   `🔸` La función getline
    *   `🔸` Escribir en ficheros y pipes
    *   `🔸` La función system()
    *   `🔸` La función close()

### 📑 Tema 09:   [Control de procesos]
* IDs de procesos y números de jobs
* 🔶 |Control de jobs|
   *   `🔸` Foreground y background
   *   `🔸` Suspender y reanudar un job
   *   `🔸` El comando ps
   *   `🔸` El comando top
* 🔶 |Señales|
   *   `🔸` Combinaciones de teclas que envían señales
   *   `🔸` El comando interno kill
* 🔶 |Capturar señales desde un script|
   *   `🔸` El comando interno trap
   *   `🔸` Traps y funciones
   *   `🔸` IDs de proceso
   *   `🔸` Ignorar señales
* |Reatachar sesiones del terminal|
* |Corrutinas|
* |Subshells|
* |La sustitución de procesos|

### 📑 Tema 10:   [Depurar scripts]
* |Opciones de Bash para depuración|
* 🔶 |Fake signals|
    *   `🔸` La señal SIGEXIT
    *   `🔸` La señal SIGERR
    *   `🔸` La señal SIGDEBUG
    *   `🔸` La señal SIGRETURN
* 🔶 |Un depurador Bash|
    *   `🔸`  Estructura del depurador
    *   `🔸`  El driver
    *   `🔸`  El preámbulo
* 🔶 |Funciones del depurador|
    *   `🔸` Avanzar paso apaso
    *   `🔸` El menú de comandos
    *   `🔸` Los breakpoints por número de línea
    *   `🔸` Los breakpoints condicionales
    *   `🔸` Trazar la ejecución
    *   `🔸` Ejemplo de ejecución

---
