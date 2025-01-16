Liesmich-Datei fr den Hewlett-Packard HP-GL/2 und HP RTL Treiber fr AutoCAD 
-----------------------------------------------------------------------------

Produktname:     HP-GL/2 Treiber fr AutoCAD
------------     Releases 10, 11, 12, 13, 14 (v4.0)

Versionsnummer:  v4.0
--------------
Untersttzte Sprache(n): Englisch, Franz”sisch, Italienisch, Deutsch,
------------------------ Spanisch, Japanisch, vereinfachtes Chinesisch, 
			 traditionelles Chinesisch, Koreanisch.

Untersttzte Produkte:     
----------------------      
      HP DesignJet Serie (auáer dem ursprnglichen DesignJet)
      HP DraftMaster SX/RX/MX
      HP DraftMaster Plus Serie
      HP DraftPro Plus
      HP LaserJet Serie
      HP PaintJet XL 300
      HP 7600 Serie Elektrostatische Plottermodelle


Systemanforderungen:  Die AutoCAD-Version, fr welche dieser Treiber
--------------------  installiert werden soll, muá bereits auf Ihrem PC
		      installiert sein. AutoCAD muá vor der Treiber-
		      installation wenigstens einmal ausgefhrt worden sein, 
		      damit die richtige Konfiguration sichergestellt ist
		      und die Datei ACAD.CFG (oder ACADNT.CFG oder 
		      ACAD14.CFG) erstellt wurde.



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Treiberhinweise: (Allgemein fr alle Versionen)
-----------------------------------------------


Netzwerk-Installation
---------------------
Beachten Sie die nachstehenden Voraussetzungen zum Installieren dieses
Treibers, wenn Sie AutoCAD von einem Server aus starten:

1.- Der Treiber kann im Server installiert und auf jedem Computer,
    der am Server angeschlossen ist, verwendet werden.

2.- Sie mssen Schreibberechtigung fr die Verzeichnisse auf der Festplatte
    des Servers haben. Wenn keine Schreibberechtigung vorliegt, muá die
    Installation vom Systemverwalter oder einem anderen Anwender, der die
    geforderten Zugriffsrechte hat, ausgefhrt werden.

3.- AutoCAD darf nicht gestartet sein, w„hrend Sie den Treiber installieren.
    Gegebenenfalls bitten Sie Ihre Kolleginnen/Kollegen, deren Arbeit mit
    AutoCAD zu beenden, bevor Sie mit der Installation beginnen.


Dateibertragungsfehler
-----------------------
Wenn w„hrend der Installation dieses Treibers ein "Allgemeiner 
Dateibertragungsfehler" auftritt, vergewissern Sie sich, daá Sie fr das 
Verzeichnis und alle Unterverzeichnisse, die Sie fr die Installation 
ausgew„hlt haben, ber die Schreibberechtigung verfgen.


Wenn Sie Ihren vorhandenen Treiber auf v4.0 erweitern
-----------------------------------------------------
Wenn Ihre AutoCAD-Konfiguration bereits fr den Einsatz einer „lteren
Treiberversion (v3.3 oder „lter) eingerichtet ist, sollten Sie beachten,
daá Sie die Plotterkonfiguration fr AutoCAD wiederholen mssen, um die
Version 4.0 verwenden zu k”nnen. Auáerdem l”scht die Installationsprozedur 
Ihre „ltere Treiberversion, w„hrend die neue Version installiert wird.

An sp„terer Stelle finden Sie weitere Hinweise zu spezifischen Systemen.


Abbrechen eines Jobs
--------------------
Es ist nicht m”glich, unter Verwendung des Statusmonitors einen Job
abzubrechen, wenn sich der Job innerhalb von geschachtelten Jobs befindet.
Der Abbruchbefehl wirkt sich jedoch auf die nachfolgende Schachtelung
aus, falls diese Seiten des abzubrechenden Jobs enth„lt.


Mehrfache AutoCAD-Sitzungen
---------------------------
Obwohl AutoCAD Release 13 und 14 den gleichzeitigen Ablauf mehrerer 
Sitzungen erlauben, kann der Treiber jeweils nur fr eine arbeiten 
bzw. verwendet werden.


Medium-Mindestgr”áe
-------------------
Wenn Sie eine benutzerdefinierte Gr”áe (in PLOT, HPMPLOT oder HPRENDER) 
festlegen, die kleiner als A4 ist, und Sie verwenden ein Rollenmedium,
dann wird die Abbildung in der richtigen Gr”áe gedruckt, wobei das Medium
jedoch auf die Gr”áe A4 abgeschnitten werden kann.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


AutoCAD Anwendungshinweise:

AutoCAD Release 12 fr Windows-Anwender
---------------------------------------

1.- Stellen Sie sicher, daá die neueste Version (C4 oder h”her) 
    von AutoCAD r12 fr Windows installiert ist. Autodesk bietet fr 
    alle Anwender von AutoCAD fr Windows eine kostenlose Erweiterung auf
    diese Version an.


2.- Um festzustellen, ob Ihr HP Treiber fr AutoCAD richtig installiert
    ist, sollten Sie den Inhalt einer der folgenden Dateien berprfen:

    Datei 1: ACAD.ADS

	Diese Datei, welche sich standardm„áig im Verzeichnis
	C:\ACADWIN befindet, sollte folgende Anweisung enthalten:

	acadapp
	C:\ACADWIN\SUPPORT\HPMPLOT.EXE


    Datei 2: WIN.INI

	Diese Datei, welche sich standardm„áig im Verzeichnis
	C:\WINDOWS befindet, sollte im Abschnitt: 

	[hpgl2acaddrv]

	die folgende Zeile enthalten:

	config=C:\ACADWIN\

	oder wo immer die AutoCAD-Konfiguration gespeichert ist.


3.- Sie k”nnen den HP-GL/2 Treiber nur fr eine Konfiguration 
    von AutoCAD Release 12 pro PC installieren.


AutoCAD Release 13 fr Windows-Anwender
---------------------------------------

Diese Version ben”tigt eine nicht unbeachtliche Speichergr”áe. 
Falls Fehlermeldungen angezeigt werden, wird eine Vergr”áerung des
Speicherbereichs fr Ihren PC empfohlen.

(Autodesk empfiehlt ein Minimum von 16 MB RAM; beachten Sie jedoch,
daá es sich hier um die Basiskonfiguration handelt.)


AutoCAD Release 14 fr Windows-Anwender
---------------------------------------

Wenn eine Fehlermeldung erscheint, die Sie ber eine fehlende oder
inkonsistente Treiberdatei informiert, k”nnen Sie den Fehler wie folgt 
manuell in der Datei acad14.cfg korrigieren:

1.- Stellen Sie sicher, daá AutoCAD beendet wurde und nicht aktiv ist.

2.- ™ffnen Sie die Datei acad14.cfg in einem beliebigen Texteditor.
    acad14.cfg ist eine ASCII-Datei, so daá Sie in fast jeden Texteditor
    eingelesen werden kann.

3.- Ersetzen Sie jede Stelle, an welcher die Zeichenfolge

      "Hewlett-Packard HP-GL/2 Ger„te, ADI 4.3 - fr Autodesk von HP"

    erscheint durch die Zeichenfolge

      "Hewlett-Packard HP-GL/2 v4.0, ADI 4.3 - von HP".

    Hierdurch wird AutoCAD mitgeteilt, daá der neue Treiber mit den
    verbundenen Ger„ten zu verwenden ist.

4.- Speichern Sie die Datei, und verlassen Sie den Texteditor.

Jetzt sollten Sie AutoCAD starten k”nnen ohne daá die Fehlermeldung 
erscheint.

Sie k”nnen erneut "Konfig" ausfhren und "ndern" und "Rekonfigurieren" 
ausw„hlen, um von Ihnen installierte Ger„te neu zu konfigurieren.
Beachten Sie, daá die HP LaserJets jetzt auch Rasterbilder untersttzen,
so daá Sie Ihre LaserJet 4 Ger„te entweder als "HP LaserJet (11x17, A3)"
oder als "HP LaserJet (Standard)" (mit diesem Treiber verfgbar) neu 
konfigurieren sollten.


Windows fr Workgroups-Anwender
-------------------------------

Windows fr Workgroups-Anwender sollten berprfen, ob Sie die neuesten
Versionen der zum Betriebssystem geh”renden Dateien vorliegen haben.


Windows NT-Anwender
-------------------
1.- Wenn Sie Drucker konfiguriert haben, die einen speziellen LPTx-Anschluá
    verwenden, und Sie aus AutoCAD an den gleichen Anschluá drucken, kann
    eine Fehlermeldung mit dem Hinweis erscheinen, daá AutoCAD diesen 
    Anschluá nicht einrichten kann. Dies kommt daher, daá AutoCAD direkt
    auf die Hardware zuzugreifen versucht. Um dieses Problem zu vermeiden,
    sollte fr keinen Drucker der gleiche LPTx-Anschluá konfiguriert sein,
    an welchen die Druckausgabe aus AutoCAD erfolgen soll.

2.- Wie kann aus AutoCAD 13 unter Windows NT auf einem Plotter geplottet 
    werden, der an einem Server angeschlossen ist?

    a) Wechseln Sie zur DOS-Eingabeaufforderung, und geben Sie folgenden
       Befehl ein:

	net use LPTx "Netzwerk-Plottername" /persistent:yes

    b) Konfigurieren Sie Ihren Plotter in AutoCAD auf die bliche Weise.
       Wenn Sie zur Eingabe einer COM/LPT-Anschluánummer aufgefordert
       werden, geben Sie einen Punkt (.) fr "keine" an.

    c) W„hrend der Konfiguration des Plotters rufen Sie die
       Systemparameter auf, und „ndern Sie den Namen fr die 
       Standard-Plotdatei auf "c:\<lokaler Pfad>\LPTx".

3.- Wenn das Installationsprogramm keine „ltere AutoCAD-Installation erkennt...

    Wenn Sie mit Windows NT 4.0 arbeiten und AutoCAD unter einem Account
    mit Zugriffsrechten eines Systemverwalters installiert haben, sollten
    Sie auch diesen Treiber unter einem Account mit Zugriffsrechten eines
    Systemverwalters installieren. Wenn Sie dies nicht beachten, kann das
    Installationsprogramm m”glicherweise nicht das Verzeichnis der
    AutoCAD-Installation erkennen. Sie k”nnen dieses Problem umgehen, indem
    Sie das genaue Verzeichnis der AutoCAD-Installation eingeben, wenn Sie
    hierzu vom Installationsprogramm aufgefordert werden.



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Treiberhinweise: (nur fr asiatische Versionen)
-----------------------------------------------
Diese Abschnitte beschreiben die Umgebung, in welcher die lokalisierte
Version des AutoCAD-Treibers in asiatischen L„ndern untersttzt wird.


China
-----
Englische Version von AutoCAD fr DOS (r10, r11, r12 und r13), zusammen
mit dem ACE-Layer und dem englischen HP AutoCAD-Treiber fr DOS.

Englische Version von AutoCAD fr Windows (r12 und r13), zusammen mit dem
ACE-Layer und dem chinesischen HP AutoCAD-Treiber fr Windows. 


Taiwan
------
Englische Version von AutoCAD fr DOS (r10 und r11), zusammen
mit dem englischen HP AutoCAD-Treiber fr DOS.

Taiwanesische Version von AutoCAD fr DOS (r12 und r13), zusammen
mit dem taiwanesischen HP AutoCAD-Treiber fr DOS.

Englische Version von AutoCAD fr Windows r12, zusammen mit dem
englischen HP AutoCAD-Treiber fr Windows.

Taiwanesische Version von AutoCAD fr Windows r13, zusammen mit dem
taiwanesischen HP AutoCAD-Treiber fr Windows.


Korea
-----
Englische Version von AutoCAD fr DOS (r10 und r11), zusammen mit 
dem englischen HP AutoCAD-Treiber fr DOS.

Koreanische Version von AutoCAD fr DOS (r12 und r13), zusammen mit 
dem koreanischen HP AutoCAD-Treiber fr DOS.

Englische Version von AutoCAD fr Windows r12, zusammen mit dem
englischen HP AutoCAD-Treiber fr Windows.

Koreanische Version von AutoCAD fr Windows r13, zusammen mit dem
koreanischen HP AutoCAD-Treiber fr Windows.
