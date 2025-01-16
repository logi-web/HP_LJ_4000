Fichier Lisezmoi du gestionnaire HP-GL/2 et RTL HP pour AutoCAD 
--------------------------------------------------------------------------------------------------

Nom du produit :   Gestionnaire HP-GL/2 pour AutoCAD
-----------------------    Versions 10, 11, 12, 13 et 14 (v4.0)

Numéro de version : v4.0
----------------------------

Langue(s) prise(s) en charge : anglais, français, italien, allemand, espagnol,
------------------------------------------- japonais, chinois simplifié, chinois traditionnel et coréen.

Produits pris en charge :     
-----------------------------------     
      Traceurs de la série HP DesignJet (à l'exception du traceur DesignJet d'origine)
      Traceurs de la série HP DraftMaster SX/RX/MX
      Traceurs de la série HP DraftMaster Plus
      Traceurs HP DraftPro Plus
      Imprimantes de la série HP LaserJet
      Traceurs HP PaintJet XL 300
      Traceurs électrostatiques HP 7600


Caractéristiques du système : La version d'AutoCAD pour laquelle vous souhaitez
------------------------------------------- installer ce gestionnaire doit déjà être installée sur votre PC. 
                                            AutoCAD doit avoir été exécuté au moins une fois avant
                                            d'installer le gestionnaire afin de vous assurer qu'il est
                                            correctement configuré et que le fichier ACAD.CFG (ou
                                            ACADNT.CFG ou ACAD14.CFG) a été créé. 
                      


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Généralités concernant le gestionnaire (pour toutes les versions) :
----------------------------------------------------------------------------------------------


Installation en réseau   
----------------------
Si vous exécutez AutoCAD à partir d'un serveur, gardez à l'esprit les  
points suivants pour installer ce gestionnaire : 
  
1. - Vous pouvez installer le gestionnaire sur le serveur et l'utilisez
     à partir de chaque ordinateur. 
 
2. - Vous devez posséder des droits d'accès en écriture sur les  
    répertoires du disque dur du serveur. Dans le cas contraire, vous  
    devrez faire exécuter l'installation par l'administrateur système ou  
    par un utilisateur possédant les droits d'accès appropriés.  
  
3. - Aucune session AutoCAD ne doit être ouverte lorsque vous  
    installez le gestionnaire. Demandez à tous les utilisateurs de fermer  
    leur session AutoCAD pendant la procédure d'installation. 


Erreur de transfert de fichier 
----------------------------------------
Si vous recevez une "Erreur générale de transfert" au cours de l'installation 
de ce gestionnaire, assurez-vous que vous disposez de droits d'accès en
écriture sur le répertoire et sur tous les sous-répertoires dans lesquels le
gestionnaire doit être installé. 


Si vous mettez à jour votre gestionnaire pour une version v4.0
----------------------------------------------------------------------------------------
Si AutoCAD est configuré pour utilisez une ancienne version de ce
gestionnaire (v3.3 ou antérieure), notez que vous devrez répéter la
processus de configuration du traceur dans AutoCAD de manière à ce
qu'il utilise la version 4.0 du gestionnaire. De plus, le processus d'installation
supprimera l'ancienne version du gestionnaire lors de l'installation de la
nouvelle version. 

Pour toute information sur des problèmes spécifiques, voir ci-dessous. 


Annulation d'une tâche
---------------------------------
Il n'est pas possible d'annuler une tâche à l'aide du gestionnaire d'état si
la tâche se trouve au sein d'un ensemble de tâches. Toutefois, l'annulation
sera effective sur l'ensemble suivant s'il comporte des pages de la tâche
annulée. 


Sessions AutoCAD multiples
------------------------------------------
Bien que AutoCAD versions 13 et 14 permettent l'exécution de
plusieurs sessions en simultané, le gestionnaire ne peut fonctionner
que pour l'une d'entre elles.


Format de support minimal
---------------------------------------
Si vous entrez un Format Utilisateur (dans TRACEUR, HPMPLOT ou HPRENDER)
inférieur à A4 et que vous utilisez une alimentation en rouleau, le format du
dessin sera bon mais le support sera peut-être coupé au format A4.


     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Notes d'application AutoCAD :


AutoCAD version 12 pour utilisateurs Windows
-------------------------------------------------------------------

1.- Assurez-vous que vous avez installé la dernière version (C4 ou ultérieure) 
    d'AutoCAD v12 pour Windows. Sinon, Autodesk offre une mise à jour gratuite 
    pour tous les utilisateurs d'AutoCAD pour Windows.


2.- Afin de vous assurer que votre gestionnaire HP pour AutoCAD est
    correctement installé, vérifiez le contenu des fichiers suivants :

    Fichier 1 : ACAD.ADS

    Ce fichier, qui se trouve par défaut dans le répertoire
    C:\ACADWIN, doit comporter les instructions suivantes :

    acadapp
    C:\ACADWIN\SUPPORT\HPMPLOT.EXE

    Fichier 2 : WIN.INI

    Ce fichier, qui se trouve par défaut dans le répertoire
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

Cette version exige un espace mémoire important. Si des messages
d'erreur apparaissent, il est conseillé d'ajouter de la mémoire à votre PC.

(Autodesk recommande un minimum de 16 Mo de RAM, mais gardez à
l'esprit qu'il s'agit de la configuration de base) 


AutoCAD version 14 pour utilisateurs Windows
-------------------------------------------------------------------

Si vous recevez un message d'erreur signalant l'absence d'un fichier
du gestionnaire ou un problème avec ce gestionnaire, vous pouvez modifier
le fichier acad14.cfg manuellement en procédant de la manière suivante :

1.- Assurez-vous qu'AutoCAD est bien présent et qu'aucune session n'est ouverte. 

2.- Ouvrez le fichier acad14.cfg dans l'éditeur de texte de votre choix.
    Acad14.cfg est un fichier ASCII qui peut donc être édité dans presque
    tous les éditeurs de texte. 

3.- Remplacez toutes les occurrences de la chaîne. 

      "Hewlett-Packard HP-GL/2, ADI 4.3 - pour Autodesk par HP"

    par la chaîne

      "Hewlett-Packard HP-GL/2 v4.0, ADI 4.3 - par HP".

    Ceci indique à AutoCAD d'utiliser le nouveau gestionnaire ainsi que
    les périphériques qui lui sont associés. 

3.- Sauvegardez le fichier et quittez l'éditeur de texte. 

Vous devriez maintenant être en mesure d'exécuter AutoCAD 
sans message d'erreur. 

Si vous souhaitez de nouveau exécuter "config", sélectionner
"modifier" et "reconfigurer" pour reconfigurer un périphérique que vous
avez installé, notez que les imprimantes gèrent désormais les images
tramées. Vous devriez donc reconfigurer vos imprimantes LaserJet 4 en
"HP LaserJet (11x17, A3)" ou en "HP LaserJet (Standard)" disponibles
avec votre gestionnaire. 


Utilisateurs de Windows pour Workgroups.
-------------------------------------------------------------

Il est conseillé aux utilisateurs Windows pour Workgroups de vérifier
qu'ils disposent des fichiers de système d'exploitation les plus récents.

   
Utilisateurs Windows NT   
-----------------------------------
1. Si vous avez configuré des imprimantes sur un port LPTx   
    spécifique et que vous tentez d'imprimer depuis AutoCAD en   
    utilisant le même port, vous obtiendrez un message d'erreur vous   
    signalant qu'AutoCAD ne peut pas configurer ce port. Ceci   
    s'explique par le fait qu'AutoCAD tente d'accéder directement au   
    matériel. Pour ne pas rencontrer ce problème, ne configurez aucune   
    imprimante sur le même port LPTx qu'AutoCAD.   
   
2. Procédure pour imprimer depuis AutoCAD 13 dans Windows NT   
    sur un traceur connecté à un serveur   
   
    a) Au niveau de l'invite de commande du DOS, tapez :   
   
net use LPTx "nom_du_traceur_reseau" /persistent:yes   
   
    b) Configurez votre traceur dans AutoCAD en suivant la procédure   
        normale. Lorsque le système vous demande un numéro de port   
        COM/LPT, entrez un point (.) pour n'indiquer aucun port.   
   
    c) Lorsque vous configurez le traceur, passez dans la section des   
        paramètres du système et remplacez le nom du fichier de traçage   
        par défaut par c:\<chemin_local>\LPTx.   

4.- Si l'installateur n'a pas détecté une version antérieure d'AutoCAD...

    Si vous travaillez sous Windows NT 4.0 et que vous avez installé AutoCAD
    sur un compte avec des privilèges réservés à l'administrateur, vous devriez
    également installer ce gestionnaire sur un compte à privilège administrateur.
    Sinon, l'installateur ne pourra localiser AutoCAD. Vous pouvez également 
   résoudre ce problème en entrant la localisation exacte du répertoire de
   l'installation AutoCAD lorsque l'installateur vous y invite. 



     -o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o--o-


Remarques sur le gestionnaire (uniquement pour les versions asiatiques) :
----------------------------------------------------------------------------------------------------------

Cette section décrit l'environnement dans lequel la version localisée du 
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


Corée
---------
Version anglaise d'AutoCAD pour DOS (v10 et v11), conjointement avec le
gestionnaire AutoCAD anglais HP pour DOS.

Version coréenne d'AutoCAD pour DOS (v12 et v13), conjointement avec le
gestionnaire AutoCAD coréen HP pour DOS.

Version anglaise d'AutoCAD pour Windows v12, conjointement avec le
gestionnaire AutoCAD anglais HP pour Windows.

Version coréenne d'AutoCAD pour Windows v13, conjointement avec le
gestionnaire AutoCAD coréen HP pour Windows.

