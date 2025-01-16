Fichier Lisezmoi du gestionnaire HP-GL/2 et RTL HP pour AutoCAD 
--------------------------------------------------------------------------------------------------

Nom du produit :   Gestionnaire HP-GL/2 pour AutoCAD
-----------------------    Versions 10, 11, 12, 13 et 14 (v4.0)

Num�ro de version : v4.0
----------------------------

Langue(s) prise(s) en charge : anglais, fran�ais, italien, allemand, espagnol,
------------------------------------------- japonais, chinois simplifi�, chinois traditionnel et cor�en.

Produits pris en charge :     
-----------------------------------     
      Traceurs de la s�rie HP DesignJet (� l'exception du traceur DesignJet d'origine)
      Traceurs de la s�rie HP DraftMaster SX/RX/MX
      Traceurs de la s�rie HP DraftMaster Plus
      Traceurs HP DraftPro Plus
      Imprimantes de la s�rie HP LaserJet
      Traceurs HP PaintJet XL 300
      Traceurs �lectrostatiques HP 7600


Caract�ristiques du syst�me : La version d'AutoCAD pour laquelle vous souhaitez
------------------------------------------- installer ce gestionnaire doit d�j� �tre install�e sur votre PC. 
                                            AutoCAD doit avoir �t� ex�cut� au moins une fois avant
                                            d'installer le gestionnaire afin de vous assurer qu'il est
                                            correctement configur� et que le fichier ACAD.CFG (ou
                                            ACADNT.CFG ou ACAD14.CFG) a �t� cr��. 
                      


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


G�n�ralit�s concernant le gestionnaire (pour toutes les versions) :
----------------------------------------------------------------------------------------------


Installation en r�seau   
----------------------
Si vous ex�cutez AutoCAD � partir d'un serveur, gardez � l'esprit les  
points suivants pour installer ce gestionnaire : 
  
1. - Vous pouvez installer le gestionnaire sur le serveur et l'utilisez
     � partir de chaque ordinateur. 
 
2. - Vous devez poss�der des droits d'acc�s en �criture sur les  
    r�pertoires du disque dur du serveur. Dans le cas contraire, vous  
    devrez faire ex�cuter l'installation par l'administrateur syst�me ou  
    par un utilisateur poss�dant les droits d'acc�s appropri�s.  
  
3. - Aucune session AutoCAD ne doit �tre ouverte lorsque vous  
    installez le gestionnaire. Demandez � tous les utilisateurs de fermer  
    leur session AutoCAD pendant la proc�dure d'installation. 


Erreur de transfert de fichier 
----------------------------------------
Si vous recevez une "Erreur g�n�rale de transfert" au cours de l'installation 
de ce gestionnaire, assurez-vous que vous disposez de droits d'acc�s en
�criture sur le r�pertoire et sur tous les sous-r�pertoires dans lesquels le
gestionnaire doit �tre install�. 


Si vous mettez � jour votre gestionnaire pour une version v4.0
----------------------------------------------------------------------------------------
Si AutoCAD est configur� pour utilisez une ancienne version de ce
gestionnaire (v3.3 ou ant�rieure), notez que vous devrez r�p�ter la
processus de configuration du traceur dans AutoCAD de mani�re � ce
qu'il utilise la version 4.0 du gestionnaire. De plus, le processus d'installation
supprimera l'ancienne version du gestionnaire lors de l'installation de la
nouvelle version. 

Pour toute information sur des probl�mes sp�cifiques, voir ci-dessous. 


Annulation d'une t�che
---------------------------------
Il n'est pas possible d'annuler une t�che � l'aide du gestionnaire d'�tat si
la t�che se trouve au sein d'un ensemble de t�ches. Toutefois, l'annulation
sera effective sur l'ensemble suivant s'il comporte des pages de la t�che
annul�e. 


Sessions AutoCAD multiples
------------------------------------------
Bien que AutoCAD versions 13 et 14 permettent l'ex�cution de
plusieurs sessions en simultan�, le gestionnaire ne peut fonctionner
que pour l'une d'entre elles.


Format de support minimal
---------------------------------------
Si vous entrez un Format Utilisateur (dans TRACEUR, HPMPLOT ou HPRENDER)
inf�rieur � A4 et que vous utilisez une alimentation en rouleau, le format du
dessin sera bon mais le support sera peut-�tre coup� au format A4.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notes d'application AutoCAD :


AutoCAD version 12 pour utilisateurs Windows
-------------------------------------------------------------------

1.- Assurez-vous que vous avez install� la derni�re version (C4 ou ult�rieure) 
    d'AutoCAD v12 pour Windows. Sinon, Autodesk offre une mise � jour gratuite 
    pour tous les utilisateurs d'AutoCAD pour Windows.


2.- Afin de vous assurer que votre gestionnaire HP pour AutoCAD est
    correctement install�, v�rifiez le contenu des fichiers suivants :

    Fichier 1 : ACAD.ADS

    Ce fichier, qui se trouve par d�faut dans le r�pertoire
    C:\ACADWIN, doit comporter les instructions suivantes :

    acadapp
    C:\ACADWIN\SUPPORT\HPMPLOT.EXE

    Fichier 2 : WIN.INI

    Ce fichier, qui se trouve par d�faut dans le r�pertoire
    C:\WINDOWS, doit comporter sous la section :

    [hpgl2acaddrv]

    la ligne suivante :

    config=C:\ACADWIN\

    ou quelque autre ligne indiquant l'emplacement de la
    configuration d'AutoCAD.


3.- Vous ne pouvez installer le gestionnaire HP-GL/2 que pour 
    une configuration de la version 12 d'AutoCAD par PC.


AutoCAD version 13 pour utilisateurs Windows
-------------------------------------------------------------------

Cette version exige un espace m�moire important. Si des messages
d'erreur apparaissent, il est conseill� d'ajouter de la m�moire � votre PC.

(Autodesk recommande un minimum de 16 Mo de RAM, mais gardez �
l'esprit qu'il s'agit de la configuration de base) 


AutoCAD version 14 pour utilisateurs Windows
-------------------------------------------------------------------

Si vous recevez un message d'erreur signalant l'absence d'un fichier
du gestionnaire ou un probl�me avec ce gestionnaire, vous pouvez modifier
le fichier acad14.cfg manuellement en proc�dant de la mani�re suivante :

1.- Assurez-vous qu'AutoCAD est bien pr�sent et qu'aucune session n'est ouverte. 

2.- Ouvrez le fichier acad14.cfg dans l'�diteur de texte de votre choix.
    Acad14.cfg est un fichier ASCII qui peut donc �tre �dit� dans presque
    tous les �diteurs de texte. 

3.- Remplacez toutes les occurrences de la cha�ne. 

      "Hewlett-Packard HP-GL/2, ADI 4.3 - pour Autodesk par HP"

    par la cha�ne

      "Hewlett-Packard HP-GL/2 v4.0, ADI 4.3 - par HP".

    Ceci indique � AutoCAD d'utiliser le nouveau gestionnaire ainsi que
    les p�riph�riques qui lui sont associ�s. 

3.- Sauvegardez le fichier et quittez l'�diteur de texte. 

Vous devriez maintenant �tre en mesure d'ex�cuter AutoCAD 
sans message d'erreur. 

Si vous souhaitez de nouveau ex�cuter "config", s�lectionner
"modifier" et "reconfigurer" pour reconfigurer un p�riph�rique que vous
avez install�, notez que les imprimantes g�rent d�sormais les images
tram�es. Vous devriez donc reconfigurer vos imprimantes LaserJet 4 en
"HP LaserJet (11x17, A3)" ou en "HP LaserJet (Standard)" disponibles
avec votre gestionnaire. 


Utilisateurs de Windows pour Workgroups.
-------------------------------------------------------------

Il est conseill� aux utilisateurs Windows pour Workgroups de v�rifier
qu'ils disposent des fichiers de syst�me d'exploitation les plus r�cents.

   
Utilisateurs Windows NT   
-----------------------------------
1. Si vous avez configur� des imprimantes sur un port LPTx   
    sp�cifique et que vous tentez d'imprimer depuis AutoCAD en   
    utilisant le m�me port, vous obtiendrez un message d'erreur vous   
    signalant qu'AutoCAD ne peut pas configurer ce port. Ceci   
    s'explique par le fait qu'AutoCAD tente d'acc�der directement au   
    mat�riel. Pour ne pas rencontrer ce probl�me, ne configurez aucune   
    imprimante sur le m�me port LPTx qu'AutoCAD.   
   
2. Proc�dure pour imprimer depuis AutoCAD 13 dans Windows NT   
    sur un traceur connect� � un serveur   
   
    a) Au niveau de l'invite de commande du DOS, tapez :   
   
net use LPTx "nom_du_traceur_reseau" /persistent:yes   
   
    b) Configurez votre traceur dans AutoCAD en suivant la proc�dure   
        normale. Lorsque le syst�me vous demande un num�ro de port   
        COM/LPT, entrez un point (.) pour n'indiquer aucun port.   
   
    c) Lorsque vous configurez le traceur, passez dans la section des   
        param�tres du syst�me et remplacez le nom du fichier de tra�age   
        par d�faut par c:\<chemin_local>\LPTx.   

4.- Si l'installateur n'a pas d�tect� une version ant�rieure d'AutoCAD...

    Si vous travaillez sous Windows NT 4.0 et que vous avez install� AutoCAD
    sur un compte avec des privil�ges r�serv�s � l'administrateur, vous devriez
    �galement installer ce gestionnaire sur un compte � privil�ge administrateur.
    Sinon, l'installateur ne pourra localiser AutoCAD. Vous pouvez �galement 
   r�soudre ce probl�me en entrant la localisation exacte du r�pertoire de
   l'installation AutoCAD lorsque l'installateur vous y invite. 



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Remarques sur le gestionnaire (uniquement pour les versions asiatiques) :
----------------------------------------------------------------------------------------------------------

Cette section d�crit l'environnement dans lequel la version localis�e du 
gestionnaire AutoCAD est prise en charge dans les pays asiatiques.


Chine
--------
Version anglaise d'AutoCAD pour DOS (v10, v11, v12 et v13), conjointement 
avec la couche ACE et le gestionnaire AutoCAD anglais HP pour DOS.

Version anglaise d'AutoCAD pour Windows (v12 et v13), conjointement 
avec la couche ACE et le gestionnaire AutoCAD chinois HP pour Windows.


Taiwan
----------
Version anglaise d'AutoCAD pour DOS (v10 et v11), conjointement avec le
gestionnaire AutoCAD anglais HP pour DOS.

Version taiwanaise d'AutoCAD pour DOS (v12 et v13), conjointement avec le
gestionnaire AutoCAD taiwanais HP pour DOS.

Version anglaise d'AutoCAD pour Windows v12, conjointement avec le
gestionnaire AutoCAD anglais HP pour Windows.

Version taiwanaise d'AutoCAD pour Windows v13, conjointement avec le
gestionnaire AutoCAD taiwanais HP pour Windows.


Cor�e
---------
Version anglaise d'AutoCAD pour DOS (v10 et v11), conjointement avec le
gestionnaire AutoCAD anglais HP pour DOS.

Version cor�enne d'AutoCAD pour DOS (v12 et v13), conjointement avec le
gestionnaire AutoCAD cor�en HP pour DOS.

Version anglaise d'AutoCAD pour Windows v12, conjointement avec le
gestionnaire AutoCAD anglais HP pour Windows.

Version cor�enne d'AutoCAD pour Windows v13, conjointement avec le
gestionnaire AutoCAD cor�en HP pour Windows.

