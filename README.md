

>[!WARNING]
>-EN ELABORACION ESTE REPOSITORIO AUN NO ESTA TERMINADO-<br>
>El dosier de [Manual de procedimientos], nunca esta terminado del todo, se revisa y amplia periodicamente.   
># Ultima revisión: 16-09-2026
 

<br>

---

*   **📚 Nombre del Dossier:** [Despliegue de Sistemas Linux] (introducción)
*   **🐧 Sistema Operativo Base:** Linux Mint 22.2
*   **✍️ Autor:** Santiago Garcia Santiago            
*   **✅ Estado:** Completado / Técnico



*|Descripción:<br>
*|Dosier técnico con procedimientos detallados para la preparación, instalación y mantenimiento de <br>
*|sistemas GNU Linux de ámbito domestico. Contiene información detallada desde el particionado, <br>
*|procedimientos críticos (reparación de [GRUB] y drivers Nvidia conflictivos) hasta el gaming funcional.<br>


---


<br>

<a href="https://github.com/SantiagoGarciaSantiagoTECSRM/dosieres-tecnicos-elaboracion-propia/blob/main/README.md">[📂 Indice Repositorio]</a> | [indice_contenidos](#dosier_05)  


<table style="margin: 0 auto; width: 50%; border-collapse: collapse; align:center;"">
  <tr>
    <th style="border: 1px solid black; padding: 8px;">  &emsp; &emsp;&emsp; &emsp; &emsp; &emsp; &emsp;  &emsp; &emsp; &emsp; &emsp;&emsp;|Despliegue de Sistemas Linux - Distros domesticas | &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp;  &emsp;  &emsp; &emsp; &emsp; </th> 
  </tr>
  <tr>
    <td style="border: 1px solid black; padding: 8px;">
     <a href="https://github.com/SantiagoGarciaSantiagoTECSRM/dosieres-tecnicos-elaboracion-propia/blob/despliegue-sistemas-linux/%5Bpost%5DDespliegue_linux_idx_repositorio.pdf">[post]Despliegue_linux_idx_repositorio.pdf</a>
 
  </tr>
  
</table>
<hr>
<br>


<a name="dosier_05">Indice contenidos:</a> &emsp; (Enlace de descarga al comienzo de este documento)


## 🔍 Índice del Contenido

### 📑 01 -  Uso de laboratorio virtual   **[Opcional]**   

*  `⚙️` |Virtualización de máquinas Linux| 
*  `⚙️` |Asignación de memoria RAM| 
*  `⚙️` |Asignación de Procesador| 
*  `⚙️` |Creación de discos complementarios|  
*  `⚙️` |Virtualización de máquinas Linux|
 

### 📑 02 - Preparación previa a migración
 
* |Tipo de mantenimiento en base a la distribución| 
* |Rutinas de mantenimiento en sistemas Linux| 
* |Cambios en escala almacenamiento en referencia a Windows|  
* |Conversión de unidades de almacenamiento| 
* |Tabla de equivalencias GB – TB a Mb|

### 📑 03 - Sistemas de archivo en Linux
 
* |Sistemas de archivo en Linux|   **[Diferencias]** 
* |Ofimática y uso doméstico|  
* |Características destacables|  **[ext4] [Extensión recomendada]**               
* |Servidores y alto volumen de trabajo|  
* |Sistemas virtualizados y servidores|                
* |Trabajo con grandes archivos|               
* |Brtfs|                 
* |Fat32 – Ntfs - exFat|   
              
🔶 |Sistema de arranque|     **[Legacy – MBR – GPT - UEFI]**  
*  `🔸` Partición de arranque  
*  `🔸` Equipos antiguos sin UEFI **(Anteriores al 2005)** 
*  `🔸` Equipos UEFI  **(2005 en adelante)**

🔶 |Métodos de partición| 03-01
*  `🔸` Métodos de partición  
*  `🔸` Partición clásica  
*  `🔸` Partición agrupada LVM   
*  `🔸` Ventajas del particionado clásico   
*  `🔸` Desventajas del particionado clásico 

🔶 |Métodos de trabajo en Linux|  **[Particionado clásico]** 
*  `🔸` Método 01:    -Manual-  **[Particionado Genérico]** 
*  `🔸` Método 02:    -Automático  **[Particionado Genérico]** 
*  `🔸` Partición de intercambio o **[Swap]**  
*  `🔸` Sí se dispone de un disco mecánico  
*  `🔸` Sí no se dispone de discos mecánicos  
*  `🔸` Tabla particionado moderno    [Resumen]  

* |Partición de intercambio| o [Swap]      [Discos mecánicos] 
* |Tamaño de la partición| [Swap]  [Discos HDD] 
* |Creación alternativa| de [Swap]     [Discos solidos] 
* |Volcado a archivo| [Swap]  [Swap-file] 

🔶 |Procedimiento|   **[Swap-file]**   
*  `🔸` Creación del archivo de swap                  [01-06] 
*  `🔸` Verificación del archivo swap                 [02-06]  
*  `🔸` Configuración de permisos en el archivo swap  [03-06]  
*  `🔸` Creación del swap y la asignación al archivo  [04-06] 
*  `🔸` Activación del swap en el sistema             [05-06] 
*  `🔸` Anclaje del archivo swap a [fstab ]           [06-06]  

🔶  |Virtualización de Swap|  [Zram]    **[Opcional]**
*  `🔸` Virtualización de Swap [Comprobación de instalación previa]  [01-05] 
*  `🔸` Virtualización de Swap [Instalación de app zram]             [02-05] 
*  `🔸` Virtualización de Swap [Configuración de app zram]           [03-05]  
*  `🔸` Virtualización de Swap [Activación de zram]                  [04-05]  
*  `🔸` Virtualización de Swap [Comprobación de estado zram]         [05-05]  
*  `🔸` Virtualización de Swap [Resumen instalación y activación]  

🔶 |Resumen tabla particionado Moderno|   03-02             
*  `🔸` |Preparaciones previas a la migración|   [Tabla resumen] 
*  `🔸` |Preservando la salud de las unidades de almacenamiento|


### 📑 04  Preparación previa a migración
* |Escenario 01|  [Configuración clásica HDD]     
* |Escenario 02|  [Configuración clásica – Var 01 HDD]   
* |Escenario 03|  [Configuración Clásica HDD x 1   HDD x 1]  
* |Escenario 04|  [Configuración Moderna HDD x 1   SSD x 1]
* |Escenario 05|  [Configuración Moderna HDD x 1   SSD x 2]

<hr>
Escenario optimo: [Escenario 04, ssd: particion EFI + root, HDD:/home]
<hr>

### 📑 05  Laboratorio practico 
 
* |Proceso de instalación|              [Escenario 01 - Manual] 
* |Particiones mínimas requeridas|      [Escenario 01 - Manual] 
* |Tras crear las particiones|          [Escenario 01 - Manual] 
* |Proceso de instalación|              [Escenario 05 - Manual] 
* |Información de la instalación|       [Escenario 05 - Manual] 
* |Proceso de instalación|              [Escenario 05 – Automático]
  
<hr>
Actualizaciones mayores del sistema:              [Cambiar de versión] 
<hr>

* |Proceso de instalación|              [Escenario 06 – Actualización versión]  
* |Actualizaciones de sistema|          [Escenario 06 – Actualización versión]  
* |Actualización “sucia”|               [Escenario 06 – Actualización versión] 
* |Mantener| [/home]                    [Escenario 06 – Actualización versión]  
* |Actualización “limpia”|              [Escenario 06 – Actualización versión] 
* |No actualizar|                       [Escenario 06 – Actualización versión] 

🔶 |Manteniendo| [/home]  [Escenario 06 – Actualización versión] 
*  `🔸` Identificación de los discos y sus particiones       [01-05]  
*  `🔸` Carga del disco de la nueva distro                   [02-05] 
*  `🔸` Configuración del disco de arranque                  [03-05] 
*  `🔸` Configuración del disco de carga                     [04-05] 
*  `🔸` Configuración del disco de carga aux                  [05-05]


### 📑 06  Procedimientos post-Migracion Linux

* |Identificación de la base del kernel de nuestra Fork|

🔶 |Instalación de software|                       06-01
*  `🔸` Instalación de aplicaciones en Linux Mint 
*  `🔸` Paquetes de software en Linux [Tradicionales] 
*  `🔸` Paquetes Debian y sus Forks   
*  `🔸` Instalación automatizada   
*  `🔸` Instalación de binarios para terminal   
*  `🔸` Reubicación manual del binario 
*  `🔸` Uso del compresor [.gz] [tutorial]   
*  `🔸` Uso del compresor [.tar.xz] [tutorial]   
*  `🔸` Instalación manual, paquetes comprimidos

🔶 |Operativa con repositorios| 06-02
*  `🔸` Actualizar índice de contenidos en repositorio                            
*  `🔸` Mostrar las actualizaciones de software disponibles desde repositorio     
*  `🔸` Buscar una aplicación concreta en el repositorio                          
*  `🔸` Mostrar información completa de una aplicación en repositorio            
*  `🔸` Instalar una aplicación desde el repositorio  
*  `🔸` Desinstalar paquete/aplicación y sus opciones de configuración  
*  `🔸` Desinstalar paquete/aplicación manteniendo sus opciones de configuración 
*  `🔸` Limpiar dependencias que ya no se utilizan en el sistema 
*  `🔸` Localizar ubicación del ejecutable de un paquete/aplicación  
*  `🔸` Localizar todos los paquetes y datos de una aplicación en el sistema 
*  `🔸` Ubicaciones comunes del software en sistemas Linux  
*  `🔸` Resumen, métodos de instalación 

🔶 Instalación de aplicaciones [Sand Boxing] en Linux Mint   06-03 
*  `🔸` Aplicaciones convencionales en Linux  
*  `🔸` Aplicaciones Sand Boxing en Linux  
*  `🔸` Instalación de aplicaciones Sand Boxing  
*  `🔸` Aplicaciones Sand Boxing  [Appimage]  
*  `🔸` Anclar en programas un Appimage  
*  `🔸` Repositorios de Appimage  
*  `🔸` Actualizar aplicaciones Appimage   
*  `🔸` Aplicaciones Sand Boxing  [Flatpak]  
*  `🔸` Actualizar aplicación Flatpack   
*  `🔸` Actualizar aplicación concreta de Flatpack 
*  `🔸` Mostrar todas las aplicaciones Flatpack instaladas 
*  `🔸` Ubicaciones de instalación    
*  `🔸` Flatseal 
*  `🔸` Aplicaciones Sand Boxing  [Snap]  
*  `🔸` Instalación del Daemon snap en el sistema  
*  `🔸` Instalación de la tienda snap en el sistema 
*  `🔸` Valoraciones finales  

### 📑 06 Procedimientos críticos
 
* |Instalación manual, drivers privativos grafica Nvidia [.run]|   [Nvidia serie 10xx e inferiores] 
* |Instalación manual, drivers privativos grafica Nvidia [.run]|   [Nvidia serie 20xx y superiores]

♦️ |Configuración de seguridad|  [GRUB]  07-01 
*  `❗` Cifrado de seguridad del   [GRUB] [Modo estricto]  
*  `❗` Cifrado de seguridad del   [GRUB] [Modo permisivo]  
*  `❗` Configuración de seguridad [GRUB] 

♦️ |Recuperación critica del [GRUB]|          07-02

* |Recuperación critica del [GRUB]|  Bug teclado en modo consola [GRUB]

### 📑 08  Reparación del [GRUB] 

* |Recuperación critica del [GRUB]|
   
♦️|Tipo de daños en| [GRUB]   

*  `‼️`Procedimiento reparación [GRUB] [Daños_menores] 
*  `‼️`Resumen operativo Daños menores [GRUB] 
*  `‼️`Procedimiento reparación [GRUB] [Daños_mayores] 
*  `‼️`Resumen operativo Daños mayores [GRUB]  
*  `‼️`Procedimiento reparación [GRUB] [Todo tipo de daños]


### 📑 09  Gaming en Linux     [Conceptos básicos]

🔶 |Distribuciones específicas para Gaming en Linux|  09-01 
*  `🔸` Limitaciones del Gaming en Linux  
*  `🔸` Distribuciones específicas para Gaming en Linux 
*  `🔸` Cachy OS   
*  `🔸` Bazzite   
*  `🔸` Nobara   
*  `🔸` Linux mint   
*  `🔸` ¿Como ejecuta Linux los juegos?             [Conceptos básicos] 
*  `🔸` [Steam] vs Lutris vs Heroic Luncher   

🔶 |Capas de compatibilidad:    [01 / 02]|             09-02
*  `🔸` Wine – Wine Hq   
*  `🔸` ¿Qué son las diferentes siglas y versiones de Wine?  
*  `🔸` ¿El usuario tiene que configurar manualmente Wine?  
*  `🔸` Complemento de Wine:     Bottles-Wine   [Opcional] 
*  `🔸` ¿Es imprescindible la instalación de Bottles?

🔶 |Capas de compatibilidad:    [02 / 02]|            09-03
*  `🔸` Proton  
*  `🔸` ¿Proton es WineHq?   
*  `🔸` ¿Proton se puede ejecutar con independencia de [Steam]? 
*  `🔸` ¿Cuántas versiones de Proton existen?  
*  `🔸` ¿El usuario tiene que descargar e instalar Proton?  
*  `🔸` Complemento de Proton:   Proton +  
*  `🔸` ¿Qué es Proton +?  
*  `🔸` ¿Proton+ solo sirve para el luncher [Steam]?  
*  `🔸` ¿Dónde se instalan las versiones de Proton?  
*  `🔸` Complemento de Proton:   Proton GE   
*  `🔸` ¿Qué es Proton GE?   
*  `🔸` ¿Es necesario instalar Proton GE?   
*  `🔸` Complemento de Proton:     Protontricks 

🔶 |¿Qué es Protontricks?|  
*  `🔸` ¿Cómo emplear [Protontricks]?                    [01/06] 
*  `🔸` ¿Cómo encontrar el App ID del juego?             [02/06]  
*  `🔸` Ejecutar y localizar el juego                    [03/06]  
*  `🔸` Seleccionar el mod a instalar                    [04/06] 
*  `🔸` Seleccionar tipo de componente para el prefijo   [05/06] 
*  `🔸` Instalar los componentes                         [06/06] 


🔶 |Complemento de Wine/Proton:   Winetricks|  
*  `🔸` ¿Qué es Winetricks?  
*  `🔸` ¿Cuándo hay que manejar Winetricks?  
*  `🔸` ¿Cómo funciona Winetricks?
*  
🔶 |Launcher:  [Lutris]|

*  `🔸` ¿Qué es Lutris?   
*  `🔸` ¿Es necesario Lutris para jugar en Linux?  
*  `🔸` ¿Qué ventajas nos ofrece Lutris?   
*  `🔸` ¿Cuál es la instalación optima de Lutris?

🔶 |Funcionamiento de las capas de compatibilidad|   09-04 
*  `🔸` Funcionamiento real de las capas de compatibilidad 
*  `🔸` Diferencias entre los intérpretes   
*  `🔸` Tecnologías GPU compatibles con capas compatibilidad Linux 
*  `🔸` ¿El usuario tiene que instalar estos interpretes? 
*  `🔸` ¿Qué software Linux trae de serie estos interpretes?  
*  `🔸` Resumen de instaladores  
*  `🔸` Gestores de librerías y complementos de instalación  
*  `🔸` Guía de instalación   [jugador Casual] 
*  `🔸` Guía de instalación   [jugador Gamer ]  
*  `🔸` Concepto de [Prefijo] en capas de compatibilidad  
*  `🔸` ¿El software o juego se instalan en el mismo directorio que el prefijo?


### 📑 10   |Capa de compatibilidad Wine|     [Configuración Wine]

🔶 |Instalación de Wine|     10-01 
*  `🔸` Descarga e instalación de Wine  
*  `🔸` Primera ejecución de Wine  [Creación del prefijo default] 
*  `🔸` Activación de Wine  [Desde terminal] 
*  `🔸` Donde se instala el prefijo “default” Wine

🔶 |Winetricks|              10-02 
*  `🔸` Instalación de Winetricks     
*  `🔸` Opciones de Winetricks   
*  `🔸` Resumen Winetricks

🔶 |Instalación de una aplicación en Wine|   [01/05]  10-03 
*  `🔸` Creación del prefijo personalizado    
*  `🔸` ¿Arquitectura de 32 o 64 bits?     
*  `🔸` ¿Bajo qué sistema Windows creamos la estructura del prefijo?    
*  `🔸` Modificación/configuración de un prefijo tras su creación   
*  `🔸` Instalación de dependencias/librerías en el prefijo   
*  `🔸` Instalación de fuentes básicas de Windows    
*  `🔸` Modificación resolución PPP del [Prefijo]    
*  `🔸` ¿Por qué hemos instalado estas librerías en particular?   
*  `🔸` ¿Se pueden realizar instalaciones sin tener que informarse de librerías o dependencias?   

🔶  |Ubicación por defecto de los prefijos en Wine|    
*  `🔸` Creación de un prefijo personalizado por terminal          **[Opcional]**    
*  `🔸` Creación de un prefijo personalizado por terminal          **[Crear]**    
*  `🔸` Creación de un prefijo personalizado por terminal          **[Utilizar]**    
*  `🔸` Creación de un prefijo personalizado por terminal          **[Instalar librerías]**    
*  `🔸` Creación de un prefijo personalizado por terminal          **[Ejemplo script install librerías]**

🔶  |Creación de un prefijo [Proton] mediante [Steam]|     [Opcional]   
*  `🔸`¿En qué casos tendríamos que importar prefijos steam?   
*  `🔸`Procedimiento [Preparación]               [01-06]   
*  `🔸`Procedimiento [Copiar ruta juego]         [02-06]   
*  `🔸`Procedimiento [Iniciar creación]          [03-06]
*  `🔸`Procedimiento [Introducir path cliente]   [04-06]  
*  `🔸`Procedimiento [Introducir ruta prefijo]   [05-06]
*  `🔸`Procedimiento [Introducir ruta juego]     [06-06]

🔶 |Instalación de una aplicación en Wine| [02/05]     10-05
*  `🔸` Ejecución del instalador   
*  `🔸` ¿Cómo crear la imagen del software original?  
*  `🔸` ¿Cómo emplear la imagen del software original?   
*  `🔸` Ejecución de instalador [Microsoft Office 2007]  
*  `🔸`Instalación del complemento para crear/grabar [PDF]

🔶 |Instalación de una aplicación en Wine| [03/05]      10-06 
*  `🔸` Ejecución de la aplicación [Word 2007]  
*  `🔸` Ejecución de la aplicación [Word 2007]   [Configuración]  
*  `🔸` Instalar fuentes adicionales al prefijo  [Opcional]   
*  `🔸` ¿Por qué las fuentes se copian-pegan en un directorio del prefijo?

🔶 Instalación de una aplicación en Wine [04/05]      10-07 
*  `🔸` Desinstalación de aplicación en Wine   
*  `🔸` Aplicación instalada desde [Wine][prefijo] default [01]  
*  `🔸` Aplicación instalada desde [Wine][prefijo] personalizado [02]   
*  `🔸` Software instalado en la raíz del prefijo  
*  `🔸` Software instalado fuera de la raíz del prefijo   
*  `🔸` No funciona el desinstalador de la aplicación ¿Cómo desinstalamos le software?

🔶 Instalación de una aplicación en Wine [05/05]      10-08
*  `🔸` Borrado de la cache de lanzadores 

### 📑 11 |Capa de compatibilidad  Lutris|        [Configuración Lutris]

* |Configuración de [Lutris]|   
* |Configuración del directorio de instalación de juegos por defecto|  
* |Instalación de [ejecutores] de [Lutris]|
* |ProtonUp-Qt|   
* |Proton +|   
* |Listado de versiones Wine/ejecutores en [Lutris]|   
* |Otras opciones de configuración en [Lutris]|  
* |¿Se puede emplear [Lutris] como gestor de Launchers comerciales?|   
* |¿Cómo funciona el enlace/instalación de aplicaciones en [Lutris]?|  
* |¿Se puede modificar el prefijo de instalación [Lutris] desde [winetricks]?|

🔶 |Instalación de una aplicación en Lutris|   11-01 
*  `🔸` Definir el tipo de instalación                   [01/08]  
*  `🔸` Definir datos del software                       [02/08]  
*  `🔸` Confirmar directorio de instalación              [03/08]   
*  `🔸` Ejecutar y configurar instalador                 [04/08]  
*  `🔸` Definir ubicación de instalación                 [05/08]  
*  `🔸` Configurar el [ejecutor] del juego               [06/08]  
*  `🔸` ¿Es un juego antiguo?   
*  `🔸` ¿Por qué sigue sin ejecutarse?   
*  `🔸` Ejecutando el juego                              [07/08]  
*  `🔸` Desinstalar juego                                [08/08]

<hr>
<br>







