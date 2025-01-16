Liesmich-Datei für den Hewlett-Packard HP-GL/2 und HP RTL Treiber für AutoCAD 
-----------------------------------------------------------------------------

Produktname:     HP-GL/2 Treiber für AutoCAD
--------------------     Releases 10, 11, 12, 13, 14 (v4.0)

Versionsnummer:  v4.0
-------------------------
Unterstützte Sprache(n): Englisch, Französisch, Italienisch, Deutsch,
----------------------------------- Spanisch, Japanisch, vereinfachtes Chinesisch, 
                                    traditionelles Chinesisch, Koreanisch.

Unterstützte Produkte:     
--------------------------------      
      HP DesignJet Serie (außer dem ursprünglichen DesignJet)
      HP DraftMaster SX/RX/MX
      HP DraftMaster Plus Serie
      HP DraftPro Plus
      HP LaserJet Serie
      HP PaintJet XL 300
      HP 7600 Serie Elektrostatische Plottermodelle


Systemanforderungen:  Die AutoCAD-Version, für welche dieser Treiber
--------------------------------  installiert werden soll, muß bereits auf Ihrem PC
                                  installiert sein. AutoCAD muß vor der Treiber-
                                  installation wenigstens einmal ausgeführt worden sein, 
                                  damit die richtige Konfiguration sichergestellt ist
                                  und die Datei ACAD.CFG (oder ACADNT.CFG oder 
                                  ACAD14.CFG) erstellt wurde.



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Treiberhinweise: (Allgemein für alle Versionen)
------------------------------------------------------------------


Netzwerk-Installation
------------------------------
Beachten Sie die nachstehenden Voraussetzungen zum Installieren dieses
Treibers, wenn Sie AutoCAD von einem Server aus starten:

1.- Der Treiber kann im Server installiert und auf jedem Computer,
    der am Server angeschlossen ist, verwendet werden.

2.- Sie müssen Schreibberechtigung für die Verzeichnisse auf der Festplatte
    des Servers haben. Wenn keine Schreibberechtigung vorliegt, muß die
    Installation vom Systemverwalter oder einem anderen Anwender, der die
    geforderten Zugriffsrechte hat, ausgeführt werden.

3.- AutoCAD darf nicht gestartet sein, während Sie den Treiber installieren.
    Gegebenenfalls bitten Sie Ihre Kolleginnen/Kollegen, deren Arbeit mit
    AutoCAD zu beenden, bevor Sie mit der Installation beginnen.


Dateiübertragungsfehler
----------------------------------
Wenn während der Installation dieses Treibers ein "Allgemeiner 
Dateiübertragungsfehler" auftritt, vergewissern Sie sich, daß Sie für das 
Verzeichnis und alle Unterverzeichnisse, die Sie für die Installation 
ausgewählt haben, über die Schreibberechtigung verfügen.


Wenn Sie Ihren vorhandenen Treiber auf v4.0 erweitern
------------------------------------------------------------------------------
Wenn Ihre AutoCAD-Konfiguration bereits für den Einsatz einer älteren
Treiberversion (v3.3 oder älter) eingerichtet ist, sollten Sie beachten,
daß Sie die Plotterkonfiguration für AutoCAD wiederholen müssen, um die
Version 4.0 verwenden zu können. Außerdem löscht die Installationsprozedur 
Ihre ältere Treiberversion, während die neue Version installiert wird.

An späterer Stelle finden Sie weitere Hinweise zu spezifischen Systemen.


Abbrechen eines Jobs
--------------------------------
Es ist nicht möglich, unter Verwendung des Statusmonitors einen Job
abzubrechen, wenn sich der Job innerhalb von geschachtelten Jobs befindet.
Der Abbruchbefehl wirkt sich jedoch auf die nachfolgende Schachtelung
aus, falls diese Seiten des abzubrechenden Jobs enthält.


Mehrfache AutoCAD-Sitzungen
---------------------------------------------
Obwohl AutoCAD Release 13 und 14 den gleichzeitigen Ablauf mehrerer 
Sitzungen erlauben, kann der Treiber jeweils nur für eine arbeiten 
bzw. verwendet werden.


Medium-Mindestgröße
--------------------------------
Wenn Sie eine benutzerdefinierte Größe (in PLOT, HPMPLOT oder HPRENDER) 
festlegen, die kleiner als A4 ist, und Sie verwenden ein Rollenmedium,
dann wird die Abbildung in der richtigen Größe gedruckt, wobei das Medium
jedoch auf die Größe A4 abgeschnitten werden kann.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


AutoCAD Anwendungshinweise:

AutoCAD Release 12 für Windows-Anwender
-----------------------------------------------------------------

1.- Stellen Sie sicher, daß die neueste Version (C4 oder höher) 
    von AutoCAD r12 für Windows installiert ist. Autodesk bietet für 
    alle Anwender von AutoCAD für Windows eine kostenlose Erweiterung auf
    diese Version an.


2.- Um festzustellen, ob Ihr HP Treiber für AutoCAD richtig installiert
    ist, sollten Sie den Inhalt einer der folgenden Dateien überprüfen:

    Datei 1: ACAD.ADS

        Diese Datei, welche sich standardmäßig im Verzeichnis
        C:\ACADWIN befindet, sollte folgende Anweisung enthalten:

        acadapp
        C:\ACADWIN\SUPPORT\HPMPLOT.EXE


    Datei 2: WIN.INI

        Diese Datei, welche sich standardmäßig im Verzeichnis
        C:\WINDOWS befindet, sollte im Abschnitt: 

        [hpgl2acaddrv]

        die folgende Zeile enthalten:

        config=C:\ACADWIN\

        oder wo immer die AutoCAD-Konfiguration gespeichert ist.


3.- Sie können den HP-GL/2 Treiber nur für eine Konfiguration 
    von AutoCAD Release 12 pro PC installieren.


AutoCAD Release 13 für Windows-Anwender
-----------------------------------------------------------------

Diese Version benötigt eine nicht unbeachtliche Speichergröße. 
Falls Fehlermeldungen angezeigt werden, wird eine Vergrößerung des
Speicherbereichs für Ihren PC empfohlen.

(Autodesk empfiehlt ein Minimum von 16 MB RAM; beachten Sie jedoch,
daß es sich hier um die Basiskonfiguration handelt.)


AutoCAD Release 14 für Windows-Anwender
-----------------------------------------------------------------

Wenn eine Fehlermeldung erscheint, die Sie über eine fehlende oder
inkonsistente Treiberdatei informiert, können Sie den Fehler wie folgt 
manuell in der Datei acad14.cfg korrigieren:

1.- Stellen Sie sicher, daß AutoCAD beendet wurde und nicht aktiv ist.

2.- Öffnen Sie die Datei acad14.cfg in einem beliebigen Texteditor.
    acad14.cfg ist eine ASCII-Datei, so daß Sie in fast jeden Texteditor
    eingelesen werden kann.

3.- Ersetzen Sie jede Stelle, an welcher die Zeichenfolge

      "Hewlett-Packard HP-GL/2 Geräte, ADI 4.3 - für Autodesk von HP"

    erscheint durch die Zeichenfolge

      "Hewlett-Packard HP-GL/2 v4.0, ADI 4.3 - von HP".

    Hierdurch wird AutoCAD mitgeteilt, daß der neue Treiber mit den
    verbundenen Geräten zu verwenden ist.

4.- Speichern Sie die Datei, und verlassen Sie den Texteditor.

Jetzt sollten Sie AutoCAD starten können ohne daß die Fehlermeldung 
erscheint.

Sie können erneut "Konfig" ausführen und "Ändern" und "Rekonfigurieren" 
auswählen, um von Ihnen installierte Geräte neu zu konfigurieren.
Beachten Sie, daß die HP LaserJets jetzt auch Rasterbilder unterstützen,
so daß Sie Ihre LaserJet 4 Geräte entweder als "HP LaserJet (11x17, A3)"
oder als "HP LaserJet (Standard)" (mit diesem Treiber verfügbar) neu 
konfigurieren sollten.


Windows für Workgroups-Anwender
---------------------------------------------------

Windows für Workgroups-Anwender sollten überprüfen, ob Sie die neuesten
Versionen der zum Betriebssystem gehörenden Dateien vorliegen haben.


Windows NT-Anwender
---------------------------------
1.- Wenn Sie Drucker konfiguriert haben, die einen speziellen LPTx-Anschluß
    verwenden, und Sie aus AutoCAD an den gleichen Anschluß drucken, kann
    eine Fehlermeldung mit dem Hinweis erscheinen, daß AutoCAD diesen 
    Anschluß nicht einrichten kann. Dies kommt daher, daß AutoCAD direkt
    auf die Hardware zuzugreifen versucht. Um dieses Problem zu vermeiden,
    sollte für keinen Drucker der gleiche LPTx-Anschluß konfiguriert sein,
    an welchen die Druckausgabe aus AutoCAD erfolgen soll.

2.- Wie kann aus AutoCAD 13 unter Windows NT auf einem Plotter geplottet 
    werden, der an einem Server angeschlossen ist?

    a) Wechseln Sie zur DOS-Eingabeaufforderung, und geben Sie folgenden
       Befehl ein:

	net use LPTx "Netzwerk-Plottername" /persistent:yes

    b) Konfigurieren Sie Ihren Plotter in AutoCAD auf die übliche Weise.
       Wenn Sie zur Eingabe einer COM/LPT-Anschlußnummer aufgefordert
       werden, geben Sie einen Punkt (.) für "keine" an.

    c) Während der Konfiguration des Plotters rufen Sie die
       Systemparameter auf, und ändern Sie den Namen für die 
       Standard-Plotdatei auf "c:\<lokaler Pfad>\LPTx".

3.- Wenn das Installationsprogramm keine ältere AutoCAD-Installation erkennt...

    Wenn Sie mit Windows NT 4.0 arbeiten und AutoCAD unter einem Account
    mit Zugriffsrechten eines Systemverwalters installiert haben, sollten
    Sie auch diesen Treiber unter einem Account mit Zugriffsrechten eines
    Systemverwalters installieren. Wenn Sie dies nicht beachten, kann das
    Installationsprogramm möglicherweise nicht das Verzeichnis der
    AutoCAD-Installation erkennen. Sie können dieses Problem umgehen, indem
    Sie das genaue Verzeichnis der AutoCAD-Installation eingeben, wenn Sie
    hierzu vom Installationsprogramm aufgefordert werden.



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Treiberhinweise: (nur für asiatische Versionen)
------------------------------------------------------------------
Diese Abschnitte beschreiben die Umgebung, in welcher die lokalisierte
Version des AutoCAD-Treibers in asiatischen Ländern unterstützt wird.


China
--------
Englische Version von AutoCAD für DOS (r10, r11, r12 und r13), zusammen
mit dem ACE-Layer und dem englischen HP AutoCAD-Treiber für DOS.

Englische Version von AutoCAD für Windows (r12 und r13), zusammen mit dem
ACE-Layer und dem chinesischen HP AutoCAD-Treiber für Windows. 


Taiwan
----------
Englische Version von AutoCAD für DOS (r10 und r11), zusammen
mit dem englischen HP AutoCAD-Treiber für DOS.

Taiwanesische Version von AutoCAD für DOS (r12 und r13), zusammen
mit dem taiwanesischen HP AutoCAD-Treiber für DOS.

Englische Version von AutoCAD für Windows r12, zusammen mit dem
englischen HP AutoCAD-Treiber für Windows.

Taiwanesische Version von AutoCAD für Windows r13, zusammen mit dem
taiwanesischen HP AutoCAD-Treiber für Windows.


Korea
--------
Englische Version von AutoCAD für DOS (r10 und r11), zusammen mit 
dem englischen HP AutoCAD-Treiber für DOS.

Koreanische Version von AutoCAD für DOS (r12 und r13), zusammen mit 
dem koreanischen HP AutoCAD-Treiber für DOS.

Englische Version von AutoCAD für Windows r12, zusammen mit dem
englischen HP AutoCAD-Treiber für Windows.

Koreanische Version von AutoCAD für Windows r13, zusammen mit dem
koreanischen HP AutoCAD-Treiber für Windows.
