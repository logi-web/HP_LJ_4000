Archivo L‚ame para el controlador HP-GL/2 y RTL HP para AutoCAD 
---------------------------------------------------------------

Nombre del producto:   Controlador HP-GL/2 para AutoCAD
--------------------   Versiones 10, 11, 12, 13, 14 (v4.0)

Numero de versi¢n: v4.0
------------------

Idiomas admitidos: ingl‚s, franc‚s, italiano, alem n, espa¤ol, japon‚s
------------------ chino simplificado, chino tradicional, coreano.

Productos admitidos:     
--------------------      
      Serie HP DesignJet (excepto el DesignJet original)
      HP DraftMaster SX/RX/MX
      Serie HP DraftMaster Plus 
      HP DraftPro Plus
      Serie HP LaserJet 
      HP PaintJet XL 300
      Modelos de trazadores electrost ticos de la serie HP 7600


Requisitos del sistema:  Es preciso que la versi¢n de AutoCAD para la cual 
-----------------------  desea instalar este controlador se encuentre ya
                         instalada en el PC. Deber  ejecutarse AutoCAD al
                         menos una vez antes de instalar el controlador para
                         asegurarse de que se ha configurado adecuadamente y
                         se ha creado el archivo ACAD.CFG (o ACAD14.CFG). 
              

     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notas para el controlador: (general para todas las versiones)
-----------------------------------------------------------------------


Instalaci¢n de Red
------------------
Tenga en cuenta los siguientes requisitos para instalar este controlador 
si ejecuta AutoCAD desde un servidor:

1. El controlador debe estar instalado en cada ordenado local que ejecute 
AutoCAD.

2. Necesita tener permiso de escritura para los directorios del disco duro
del servidor. Si no lo tiene, necesitar  que el Administrador del Sistema
u otro usuario con los derechos de acceso apropiados ejecute la instalaci¢n.

3. No puede estar ejecut ndose ninguna sesi¢n de AutoCAD mientras instala 
el controlador. Puede ser preciso que pida a sus colegas que abandonen 
sus sesiones de AutoCAD durante el proceso de instalaci¢n.


Error de transferencia de archivo
---------------------------------
Si durante el proceso de instalaci¢n de este controlador, recibe un
"Error general de transferencia de archivo", aseg£rese de que tiene permisos
de escritura en el directorio y en todos los subdirectorios que ha 
seleccionado, en donde realizar la instalaci¢n.


Si va a actualizar su controlador actual a v4.0
-----------------------------------------------
Si su configuraci¢n de AutoCAD ya est  preparada para utilizar una versi¢n
anterior de este controlador (v3.3 o anterior) tenga en cuenta que deber 
repetir el proceso de configuraci¢n del trazador en AutoCAD para que pueda
utilizar la versi¢n 4.0. Por otro lado, el proceso de instalaci¢n eliminar 
la versi¢n antigua del controlador cuando se instale esta nueva versi¢n.

Vea m s adelante notas adicionales para los sistemas espec¡ficos.


Cancelaci¢n de un trabajo
-------------------------
No es posible cancelar un trabajo utilizando el Monitor de Estado si el
trabajo se encuentra dentro de un grupo de trabajos. Sin embargo la
cancelaci¢n se efectuar  en el siguiente grupo si ‚ste contiene p ginas
del trabajo cancelado.


Sesiones m£ltiples de AutoCAD 
-----------------------------
Aunque AutoCAD v13 y v14 permite ejecutar simult neamente varias sesiones,
el controlador solamente puede funcionar para una de ellas.


Tama¤o m¡nimo del papel
-----------------------
Cuando se especifica un Tama¤o de usuario (en SALTRAZ, HPMPLOT o HPRENDER)
inferior al tama¤o A4 y se utiliza papel en rollo, el dibujo se trazar 
en el tama¤o correcto, pero el papel podr¡a recortarse al tama¤o A4.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notas para aplicaciones AutoCAD:

AutoCAD versi¢n 12 para usuarios de Windows.
--------------------------------------------
1.- Compruebe que haya instalado la versi¢n m s reciente (C4 o superior) 
    de AutoCAD v12 para Windows. Autodesk proporciona una actualizaci¢n
    gratuita a esta versi¢n para todos los usuarios de AutoCAD para Windows.

2.- Para asegurarse de que el controlador HP para AutoCAD est  instalado
    correctamente, compruebe el contenido de los siguientes archivos:

    Archivo 1: ACAD.ADS

    Este archivo, que se encuentra por defecto en el directorio
    C:\ACADWIN, debe incluir las siguientes instrucciones:

    acadapp
    C:\ACADWIN\SUPPORT\HPMPLOT.EXE

    Archivo 2: WIN.INI

    Este archivo, que se encuentra por defecto en el directorio
    C:\WINDOWS, debe incluir bajo la secci¢n: 

    [hpgl2acaddrv]

    la siguiente l¡nea:

    config=C:\ACADWIN\

    o donde se haya colocado la configuraci¢n.

3.- Solamente puede instalar el controlador HP-GL/2 para una 
    configuraci¢n de AutoCAD Versi¢n 12 por PC.


AutoCAD versi¢n 13 para usuarios de Windows
-------------------------------------------
Esta versi¢n requiere una gran cantidad de memoria. Si aparecen mensajes
de error, se recomienda que a¤ada m s memoria al PC.

(Autodesk recomienda un m¡nimo de 16Mb de RAM, pero tenga en cuenta 
que ‚sta es la configuraci¢n b sica) 


AutoCAD versi¢n 14 para usuarios de Windows
-------------------------------------------

Si recibe un mensaje de error acerca de la falta o inconsistencia de un
archivo del controlador, puede arreglar manualmente el archivo acad14.cfg 
de la siguiente manera:

1.- Aseg£rese de que ha salido de AutoCAD y que no se est  ejecutando.

2.- Abra el archivo acad14.cfg en un editor de texto de su elecci¢n.
    acad14.cfg es un archivo ASCII, por tanto se puede leer con la mayor¡a
    de los editores de texto.

3.- Sustituya cada ocurrencia de la cadena

      "Dispositivos Hewlett-Packard HP-GL/2, ADI 4.3 - para Autodesk por HP"

    por la cadena

      "Hewlett-Packard HP-GL/2 v4.0, ADI 4.3 - por HP".

    Esto indicar  a AutoCAD que utilice el controlador nuevo con los
    dispositivos asociados.

4.- Guarde el archivo y salga del editor de texto.

Ahora podr  iniciar AutoCAD sin recibir el mensaje de error.

Puede desear ejecutar de nuevo "configurar" y seleccionar "modificar" y
"reconfigurar" para reconfigurar cualquier dispositivo que tenga instalado.
Observe que ahora las HP LaserJets admiten im genes de trama, por tanto
deber¡a volver a configurar sus dispositivos LaserJet 4 como "HP LaserJet
(11x17, A3)" o "HP LaserJet (Est ndar)", que est n disponibles con este 
controlador.


Usuarios de Windows para Trabajo en Grupo
-----------------------------------------
Los usuarios de Windows para Trabajo en Grupo deber n asegurarse de que 
tienen las versiones m s recientes de los archivos del sistema operativo.


Usuarios de Windows NT
----------------------
1.- Si ha configurado impresoras para que utilicen un puerto LPTx espec¡fico 
    e intenta imprimir desde AutoCAD utilizando este mismo puerto, recibir  
    un mensaje de error informando de que AutoCAD no puede configurar dicho 
    puerto. Esto se debe a que AutoCAD intenta acceder al hardware 
    directamente. Para evitar este problema no debe haber ninguna impresora 
    configurada para utilizar el mismo puerto LPTx que desea utilizar desde 
    AutoCAD.

2.- ¨C¢mo realiza trazados desde AutoCAD 13 en Windows NT?, ¨en un trazador 
    conectado a un servidor?

    a) Vaya al indicador de comando del DOS y escriba:

       net use LPTx "nombre del trazador de red"/persistent: yes

    b) Configure su trazador en AutoCAD en la forma habitual. Cuando se le 
       pida un n£mero de puerto COM/LPT, coloque un punto (.) para indicar 
       ninguno.

    c) Mientras configura el trazador, acceda a los par metros del sistema y 
       cambie el nombre de archivo de trazado por defecto a
       c:\<ruta local>\LPTx.

4.- Si falla el instalador al detectar instalaciones anteriores de AutoCAD...

    Si est  en Windows NT 4.0 y ha instalado AutoCAD bajo una cuenta con
    privilegios de administrador, tambi‚n deber  instalar este controlador
    bajo una cuenta con privilegios de administrador.  Si no lo hace, el
    instalador puede fallar al detectar la ubicaci¢n de la instalaci¢n de
    AutoCAD.  Tambi‚n puede resolver este problema introduciendo la 
    ubicaci¢n exacta del directorio de la instalaci¢n de AutoCAD cuando as¡
    se lo solicite el instalador. 


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notas para el controlador: (solamente para las versiones asi ticas)
-------------------------------------------------------------------

Esta secci¢n describe el entorno en el que se admite la versi¢n localizada 
del controlador AutoCAD para los pa¡ses asi ticos.


China
-----
La versi¢n inglesa de AutoCAD para DOS (v10, v11, v12 y v13), junto con
la capa ACE y el controlador AutoCAD versi¢n inglesa de HP para DOS.

La versi¢n inglesa de AutoCAD para Windows (v12 y v13), junto con la capa
ACE y el controlador AutoCAD versi¢n china de HP para Windows. 


Taiwan
------
La versi¢n inglesa de AutoCAD para DOS (v10 y v11), junto con 
el controlador AutoCAD versi¢n inglesa de HP para DOS.

La versi¢n taiwanesa de AutoCAD para DOS (v12 y v13), junto con el 
controlador AutoCAD versi¢n taiwanesa de HP para DOS.

La versi¢n inglesa de AutoCAD para Windows v12, junto con el controlador
AutoCAD versi¢n inglesa de HP para Windows.

Versi¢n taiwanesa de AutoCAD para Windows v13, junto con el controlador 
AutoCAD versi¢n taiwanesa de HP para Windows.


Corea
-----
La versi¢n inglesa de AutoCAD para DOS (v10 y v11), junto con el 
controlador AutoCAD versi¢n inglesa de HP para DOS.

Versi¢n coreana de AutoCAD para DOS (v12 y v13), junto con el 
controlador AutoCAD versi¢n coreana de HP para DOS.

La versi¢n inglesa de AutoCAD para Windows v12, junto con el controlador
AutoCAD versi¢n inglesa de HP para Windows.

Versi¢n coreana de AutoCAD para Windows v13, junto con el controlador
AutoCAD versi¢n coreana de HP para Windows.
