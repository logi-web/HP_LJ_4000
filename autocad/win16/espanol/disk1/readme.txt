Archivo Léame para el controlador HP-GL/2 y RTL HP para AutoCAD 
---------------------------------------------------------------

Nombre del producto:   Controlador HP-GL/2 para AutoCAD
------------------------------    Versiones 10, 11, 12, 13, 14 (v4.0)

Numero de versión: v4.0
---------------------------

Idiomas admitidos: inglés, francés, italiano, alemán, español, japonés
--------------------------- chino simplificado, chino tradicional, coreano.

Productos admitidos:     
------------------------------      
      Serie HP DesignJet (excepto el DesignJet original)
      HP DraftMaster SX/RX/MX
      Serie HP DraftMaster Plus 
      HP DraftPro Plus
      Serie HP LaserJet 
      HP PaintJet XL 300
      Modelos de trazadores electrostáticos de la serie HP 7600


Requisitos del sistema:  Es preciso que la versión de AutoCAD para la cual 
---------------------------------   desea instalar este controlador se encuentre ya
                                    instalada en el PC. Deberá ejecutarse AutoCAD al
                                    menos una vez antes de instalar el controlador para
                                    asegurarse de que se ha configurado adecuadamente y
                                    se ha creado el archivo ACAD.CFG (o ACAD14.CFG). 
              

     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notas para el controlador: (general para todas las versiones)
--------------------------------------------------------------------------------------


Instalación de Red
---------------------------
Tenga en cuenta los siguientes requisitos para instalar este controlador 
si ejecuta AutoCAD desde un servidor:

1. El controlador debe estar instalado en cada ordenado local que ejecute 
AutoCAD.

2. Necesita tener permiso de escritura para los directorios del disco duro
del servidor. Si no lo tiene, necesitará que el Administrador del Sistema
u otro usuario con los derechos de acceso apropiados ejecute la instalación.

3. No puede estar ejecutándose ninguna sesión de AutoCAD mientras instala 
el controlador. Puede ser preciso que pida a sus colegas que abandonen 
sus sesiones de AutoCAD durante el proceso de instalación.


Error de transferencia de archivo
----------------------------------------------
Si durante el proceso de instalación de este controlador, recibe un
"Error general de transferencia de archivo", asegúrese de que tiene permisos
de escritura en el directorio y en todos los subdirectorios que ha 
seleccionado, en donde realizar la instalación.


Si va a actualizar su controlador actual a v4.0
------------------------------------------------------------------
Si su configuración de AutoCAD ya está preparada para utilizar una versión
anterior de este controlador (v3.3 o anterior) tenga en cuenta que deberá
repetir el proceso de configuración del trazador en AutoCAD para que pueda
utilizar la versión 4.0. Por otro lado, el proceso de instalación eliminará
la versión antigua del controlador cuando se instale esta nueva versión.

Vea más adelante notas adicionales para los sistemas específicos.


Cancelación de un trabajo
-------------------------------------
No es posible cancelar un trabajo utilizando el Monitor de Estado si el
trabajo se encuentra dentro de un grupo de trabajos. Sin embargo la
cancelación se efectuará en el siguiente grupo si éste contiene páginas
del trabajo cancelado.


Sesiones múltiples de AutoCAD 
----------------------------------------------
Aunque AutoCAD v13 y v14 permite ejecutar simultáneamente varias sesiones,
el controlador solamente puede funcionar para una de ellas.


Tamaño mínimo del papel
-------------------------------------
Cuando se especifica un Tamaño de usuario (en SALTRAZ, HPMPLOT o HPRENDER)
inferior al tamaño A4 y se utiliza papel en rollo, el dibujo se trazará
en el tamaño correcto, pero el papel podría recortarse al tamaño A4.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notas para aplicaciones AutoCAD:

AutoCAD versión 12 para usuarios de Windows.
--------------------------------------------------------------------
1.- Compruebe que haya instalado la versión más reciente (C4 o superior) 
    de AutoCAD v12 para Windows. Autodesk proporciona una actualización
    gratuita a esta versión para todos los usuarios de AutoCAD para Windows.

2.- Para asegurarse de que el controlador HP para AutoCAD está instalado
    correctamente, compruebe el contenido de los siguientes archivos:

    Archivo 1: ACAD.ADS

    Este archivo, que se encuentra por defecto en el directorio
    C:\ACADWIN, debe incluir las siguientes instrucciones:

    acadapp
    C:\ACADWIN\SUPPORT\HPMPLOT.EXE

    Archivo 2: WIN.INI

    Este archivo, que se encuentra por defecto en el directorio
    C:\WINDOWS, debe incluir bajo la sección: 

    [hpgl2acaddrv]

    la siguiente línea:

    config=C:\ACADWIN\

    o donde se haya colocado la configuración.

3.- Solamente puede instalar el controlador HP-GL/2 para una 
    configuración de AutoCAD Versión 12 por PC.


AutoCAD versión 13 para usuarios de Windows
--------------------------------------------------------------------
Esta versión requiere una gran cantidad de memoria. Si aparecen mensajes
de error, se recomienda que añada más memoria al PC.

(Autodesk recomienda un mínimo de 16Mb de RAM, pero tenga en cuenta 
que ésta es la configuración básica) 


AutoCAD versión 14 para usuarios de Windows
--------------------------------------------------------------------

Si recibe un mensaje de error acerca de la falta o inconsistencia de un
archivo del controlador, puede arreglar manualmente el archivo acad14.cfg 
de la siguiente manera:

1.- Asegúrese de que ha salido de AutoCAD y que no se está ejecutando.

2.- Abra el archivo acad14.cfg en un editor de texto de su elección.
    acad14.cfg es un archivo ASCII, por tanto se puede leer con la mayoría
    de los editores de texto.

3.- Sustituya cada ocurrencia de la cadena

      "Dispositivos Hewlett-Packard HP-GL/2, ADI 4.3 - para Autodesk por HP"

    por la cadena

      "Hewlett-Packard HP-GL/2 v4.0, ADI 4.3 - por HP".

    Esto indicará a AutoCAD que utilice el controlador nuevo con los
    dispositivos asociados.

4.- Guarde el archivo y salga del editor de texto.

Ahora podrá iniciar AutoCAD sin recibir el mensaje de error.

Puede desear ejecutar de nuevo "configurar" y seleccionar "modificar" y
"reconfigurar" para reconfigurar cualquier dispositivo que tenga instalado.
Observe que ahora las HP LaserJets admiten imágenes de trama, por tanto
debería volver a configurar sus dispositivos LaserJet 4 como "HP LaserJet
(11x17, A3)" o "HP LaserJet (Estándar)", que están disponibles con este 
controlador.


Usuarios de Windows para Trabajo en Grupo
-----------------------------------------------------------------
Los usuarios de Windows para Trabajo en Grupo deberán asegurarse de que 
tienen las versiones más recientes de los archivos del sistema operativo.


Usuarios de Windows NT
------------------------------------
1.- Si ha configurado impresoras para que utilicen un puerto LPTx específico 
    e intenta imprimir desde AutoCAD utilizando este mismo puerto, recibirá 
    un mensaje de error informando de que AutoCAD no puede configurar dicho 
    puerto. Esto se debe a que AutoCAD intenta acceder al hardware 
    directamente. Para evitar este problema no debe haber ninguna impresora 
    configurada para utilizar el mismo puerto LPTx que desea utilizar desde 
    AutoCAD.

2.- ¿Cómo realiza trazados desde AutoCAD 13 en Windows NT?, ¿en un trazador 
    conectado a un servidor?

    a) Vaya al indicador de comando del DOS y escriba:

       net use LPTx "nombre del trazador de red"/persistent: yes

    b) Configure su trazador en AutoCAD en la forma habitual. Cuando se le 
       pida un número de puerto COM/LPT, coloque un punto (.) para indicar 
       ninguno.

    c) Mientras configura el trazador, acceda a los parámetros del sistema y 
       cambie el nombre de archivo de trazado por defecto a
       c:\<ruta local>\LPTx.

4.- Si falla el instalador al detectar instalaciones anteriores de AutoCAD...

    Si está en Windows NT 4.0 y ha instalado AutoCAD bajo una cuenta con
    privilegios de administrador, también deberá instalar este controlador
    bajo una cuenta con privilegios de administrador.  Si no lo hace, el
    instalador puede fallar al detectar la ubicación de la instalación de
    AutoCAD.  También puede resolver este problema introduciendo la 
    ubicación exacta del directorio de la instalación de AutoCAD cuando así
    se lo solicite el instalador. 


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notas para el controlador: (solamente para las versiones asiáticas)
------------------------------------------------------------------------------------------------

Esta sección describe el entorno en el que se admite la versión localizada 
del controlador AutoCAD para los países asiáticos.


China
--------
La versión inglesa de AutoCAD para DOS (v10, v11, v12 y v13), junto con
la capa ACE y el controlador AutoCAD versión inglesa de HP para DOS.

La versión inglesa de AutoCAD para Windows (v12 y v13), junto con la capa
ACE y el controlador AutoCAD versión china de HP para Windows. 


Taiwan
----------
La versión inglesa de AutoCAD para DOS (v10 y v11), junto con 
el controlador AutoCAD versión inglesa de HP para DOS.

La versión taiwanesa de AutoCAD para DOS (v12 y v13), junto con el 
controlador AutoCAD versión taiwanesa de HP para DOS.

La versión inglesa de AutoCAD para Windows v12, junto con el controlador
AutoCAD versión inglesa de HP para Windows.

Versión taiwanesa de AutoCAD para Windows v13, junto con el controlador 
AutoCAD versión taiwanesa de HP para Windows.


Corea
--------
La versión inglesa de AutoCAD para DOS (v10 y v11), junto con el 
controlador AutoCAD versión inglesa de HP para DOS.

Versión coreana de AutoCAD para DOS (v12 y v13), junto con el 
controlador AutoCAD versión coreana de HP para DOS.

La versión inglesa de AutoCAD para Windows v12, junto con el controlador
AutoCAD versión inglesa de HP para Windows.

Versión coreana de AutoCAD para Windows v13, junto con el controlador
AutoCAD versión coreana de HP para Windows.
