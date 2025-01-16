
File Leggimi per il driver Hewlett-Packard HP-GL/2 e HP RTL per AutoCAD 
-----------------------------------------------------------------------------------------------------------

Nome del prodotto:    Driver HP-GL/2 per AutoCAD
---------------------------    Release 10, 11, 12, 13, 14 (v4.0)

Numero di versione: v4.0
----------------------------

Lingue supportate:  inglese, francese, italiano, tedesco, spagnolo, giapponese
--------------------------  cinese semplificato, cinese tradizionale e coreano.

Prodotti supportati:    
---------------------------    
      Serie HP DesignJet (eccetto la stampante DesignJet originale)
      HP DraftMaster SX/RX/MX
      Serie HP DraftMaster Plus
      HP DraftPro Plus
      Serie HP LaserJet
      HP PaintJet XL 300
      Modelli di plotter elettrostatici serie HP 7600


Requisiti di sistema:  La versione di AutoCAD per cui si desidera installare 
-----------------------------  questo driver deve già essere installata sul PC.
                               AutoCAD deve essere stato eseguito almeno una volta
                               prima di installare il driver in modo da essere certi
                               che sia configurato correttamente e che sia stato creato
                               il file ACAD.CFG (o ACADNT.CFG o ACAD14.CFG). 
                      


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Note sul driver: (generiche per tutte le versioni)
------------------------------------------------------------------


Installazione in rete
----------------------------
Se AutoCAD viene eseguito da server, tenere presente quanto segue per
installare questo driver:

1. - Il driver può essere installato sul server ed usato da qualsiasi computer
    ad esso collegato.

2. - Occorre disporre del permesso di scrittura per le directory dell'unità
    disco fisso del server. Se non si dispone di tale permesso, la procedura di
    installazione deve essere eseguita dall'amministratore del sistema o da un
    altro utente provvisto delle apposite autorizzazioni.

3. - Non vi possono essere sessioni AutoCAD attive mentre si installa il
    driver. Pertanto, durante la procedura di installazione, si può dover
    chiedere agli altri utenti di chiudere le loro sessioni AutoCAD.


Errore di trasferimento file 
-------------------------------------
Se si riceve un messaggio che segnala un "errore generale di trasferimento
file" durante l'installazione di questo driver, accertarsi di disporre del permesso
di scrittura per la directory e tutte le sottodirectory selezionate per l'installazione.


Se si sta aggiornando il driver esistente a v4.0
------------------------------------------------------------------
Se AutoCAD è già configurato per usare una versione più vecchia di questo
driver (v3.3 o precedente), si noti che occorrerà ripetere la procedura
di configurazione del plotter in AutoCAD in modo che possa utilizzare la
versione 4.0 del driver. Si tenga presente, inoltre, che con l'installazione
di questa nuova versione verrà rimossa la versione precedente del driver. 

Per ulteriori informazioni relative a sistemi specifici, vedere più avanti.


Annullamento di un lavoro
-------------------------------------
Non è possibile annullare un lavoro con la funzione di controllo dello stato
se il lavoro fa parte di un annidamento di lavori. Tuttavia, l'annullamento
avrà effetto sul successivo annidamento se questo contiene delle pagine del
lavoro annullato. 


Sessioni AutoCAD multiple
---------------------------------------
Sebbene AutoCAD r13 e r14 consentano di avere attive più sessioni
contemporaneamente, il driver può operare solo con una di esse.


Formato minimo dei supporti
-----------------------------------------
Quando si specificano (in PLOT, HPMPLOT o HPRENDER) delle dimensioni utente
inferiori a quelle corrispondenti ad un formato A4 e si utilizza un supporto
in rotoli, il disegno viene stampato con le dimensioni corrette, ma è
possibile che il supporto venga tagliato come per il formato A4.


    -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Note sulle applicazioni AutoCAD:

AutoCAD release 12 per gli utenti di Windows
------------------------------------------------------------------

1. - Accertarsi di aver installato l'ultima versione (C4 o successiva)
    di AutoCAD r12 per Windows. Autodesk fornisce gratuitamente un
    aggiornamento a questa versione per tutti gli utenti di AutoCAD
    per Windows.

2. - Per verificare che il driver HP per AutoCAD sia installato
    correttamente, controllare il contenuto dei seguenti file:

    File 1: ACAD.ADS

        Questo file, che per impostazione predefinita si trova nella
        directory C:\ACADWIN, dovrebbe contenere le seguenti istruzioni:

        acadapp
        C:\ACADWIN\SUPPORT\HPMPLOT.EXE

    File 2: WIN.INI

        Questo file, che per impostazione predefinita si trova nella
        directory C:\WINDOWS, dovrebbe contenere nella sezione: 

        [hpgl2acaddrv]

        la seguente riga:

        config=C:\ACADWIN\

        o il percorso relativo a dove si trova la configurazione AutoCAD.

3. - E' possibile installare il driver HP-GL/2 per un'unica 
    configurazione AutoCAD release 12 per ogni PC.


AutoCAD release 13 per gli utenti di Windows
------------------------------------------------------------------

Questa versione richiede una considerevole quantità di memoria. Se
compaiono dei messaggi di errore, si consiglia di aggiungere altra
memoria al PC.

Autodesk consiglia un minimo di 16 MB di RAM, ma si tenga presente
che questo è solo per la configurazione base.


AutoCAD release 14 per gli utenti di Windows
------------------------------------------------------------------

Se si riceve un messaggio di errore relativo ad un file del driver mancante
o inadeguato, è possibile correggere manualmente il file acad14.cfg
facendo quanto segue:

1. - Accertarsi di essere usciti da AutoCAD e che AutoCAD non sia attivo.

2. - Aprire il file acad14.cfg con un qualsiasi editor di testo. Il file acad14.cfg è
    un file ASCII e quindi può essere aperto con quasi tutti gli editor di testo.

3. - Sostituire ovunque la stringa:

      "Hewlett-Packard periferiche HP-GL/2, ADI 4.3 - per Autodesk da HP"

    con la stringa:

      "Hewlett-Packard, dispositivi HP-GL/2 v4.0, ADI 4.3 - della HP".

    Così facendo AutoCAD userà il nuovo driver con i dispositivi
    associati.

4. - Salvare il file e chiudere l'editor di testo.

A questo punto, si dovrebbe essere in grado di avviare AutoCAD senza
ricevere il messaggio di errore.

Se si desidera eseguire di nuovo "configura" e selezionare "modifica"
e "riconfigura" per riconfigurare i dispositivi installati, si noti che ora
i dispositivi HP LaserJet supportano immagini raster e quindi si
devono riconfigurare i dispositivi LaserJet 4 come "HP LaserJet
(11x17, A3)" o come "HP LaserJet (Standard)", cosa possibile con
questo driver.


Utenti di Windows per Workgroup
------------------------------------------------

Accertarsi di avere le ultime versioni dei file del sistema operativo.


Utenti di Windows NT 
-------------------------------
1. - Se le stampanti sono state configurate per utilizzare una determinata
    porta LPTx e si tenta di stampare da AutoCAD utilizzando quella stessa porta,
    comparirà un messaggio di errore indicante che AutoCAD non è in grado di
    impostare la porta. Ciò dipende dal fatto che AutoCAD tenta di accedere
    direttamente all'hardware. Per evitare questo tipo di problemi, non vi devono
    essere stampanti configurate per l'uso della porta LPTx che si intende utilizzare
    da AutoCAD.

2. - Come stampare da AutoCAD 13 in Windows NT su un plotter collegato ad un
server?

    a) Andare al prompt di DOS e digitare:

	net use LPTx "nome plotter in rete"/persistent:yes

    b) Configurare il plotter in AutoCAD come di consueto. Quando viene richiesto
       di specificare il numero di una porta COM/LPT, immettere un punto (.) e non
       indicare così alcuna porta.

    c) Mentre si configura il plotter, accedere ai parametri di sistema e
       modificare il nome del file di plot predefinito specificando
       c:\<percorso locale>\LPTx.

3. - Se il programma di installazione non riesce a rilevare un'installazione
    precedente di AutoCAD...

    Se si sta usando Windows NT 4.0 e si è installato AutoCAD sotto un
    conto con privilegi di amministratore, è necessario installare anche
    questo driver sotto un conto con privilegi di amministratore. Se non
    lo si fa, il programma di installazione potrebbe non riuscire a rilevare
    l'ubicazione dell'installazione di AutoCAD. E' possibile ovviare a questo
    problema anche immettendo l'esatta ubicazione della directory in cui è
    installato AutoCAD quando richiesto dal programma di installazione.



    -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Note sul driver: (solo per le versioni asiatiche)
-----------------------------------------------------------------

In questa sezione viene descritto l'ambiente in cui la versione
localizzata del driver AutoCAD è supportata nei Paesi asiatici.


Cina
------
Versione inglese di AutoCAD per DOS (r10, r11, r12 e r13) insieme 
al layer ACE ed al driver AutoCAD inglese HP per DOS.

Versione inglese di AutoCAD per Windows (r12 e r13) insieme al 
layer ACE ed al driver AutoCAD cinese HP per Windows. 


Taiwan
----------
Versione inglese di AutoCAD per DOS (r10 e r11) insieme al 
driver AutoCAD inglese HP per DOS.

Versione taiwanese di AutoCAD per DOS (r12 e r13) insieme al 
driver AutoCAD taiwanese HP per DOS.

Versione inglese di AutoCAD per Windows r12 insieme al driver
AutoCAD inglese HP per Windows.

Versione taiwanese di AutoCAD per Windows r13 insieme al driver
AutoCAD taiwanese HP per Windows.


Corea
--------
Versione inglese di AutoCAD per DOS (r10 e r11) insieme al driver
AutoCAD inglese HP per DOS.

Versione coreana di AutoCAD per DOS (r12 e r13) insieme al driver
AutoCAD coreano HP per DOS.

Versione inglese di AutoCAD per Windows r12 insieme al driver
AutoCAD inglese HP per Windows.

Versione coreana di AutoCAD per Windows r13 insieme al driver
AutoCAD coreano HP per Windows.
