Hier finden Sie eine Dokumentation zu API-Methoden. 

Hier sind zunächst die Spezifikationen (JSON RPC 2.0) :
<http://www.jsonrpc.org/specification>

Der Zugriff auf die API erfolgt über die URL : *URL\_JEEDOM * / core / api / jeeApi.php

Divers
======

ping
----

Pong zurückgeben, Kommunikation mit Jeedom testen

version
-------

Gibt die Version von Jeedom zurück

datetime
--------

Gibt die Jeedom-Datumszeit in Mikrosekunden zurück

Konfigurations-API
==========

config::byKey
-------------

Gibt einen Konfigurationswert zurück.

Einstellungen :

-   String-Schlüssel : Konfigurationswertschlüssel, der zurückgegeben werden soll

-   String Plugin : (optional), Konfigurationswert-Plugin

-   Zeichenfolge Standard : (optional), Wert, der zurückgegeben werden soll, wenn der Schlüssel nicht vorhanden ist

config::save
------------

Speichert einen Konfigurationswert

Einstellungen :

-   Zeichenfolgenwert : Wert aufzuzeichnen

-   String-Schlüssel : Konfigurationswertschlüssel zum Speichern

-   String Plugin : (optional), Plugin des zu speichernden Konfigurationswerts

JSON-Ereignis-API
==============

event::changes
--------------

Gibt die Liste der Änderungen seit der im Parameter übergebenen Datum / Uhrzeit zurück (muss in Mikrosekunden angegeben werden).. Sie haben in der Antwort auch die aktuelle Datumszeit von Jeedom (die für die nächste Abfrage wiederverwendet werden soll).

Einstellungen :

-   int Datetime

JSON Plugin API
===============

plugin::listPlugin
------------------

Gibt die Liste alleer Plugins zurück

Einstellungen :

-   int activOnly = 0 (gibt nur die Liste der aktivierten Plugins zurück)

-   int orderByCaterogy = 0 (gibt die Liste der Plugins nach Kategorie sortiert zurück)

Objekt-JSON-API
==============

jeeObject::all
-----------

Gibt die Liste alleer Objekte zurück

jeeObject::full
------------

Gibt die Liste alleer Objekte zurück, wobei für jedes Objekt allee Geräte und für jedes Gerät allee Befehle sowie deren Status angegeben werden (für Befehle vom Typ Info).

jeeObject::fullById
----------------

Gibt ein Objekt mit alle seinen Geräten und für jedes Gerät allee seine Befehle und deren Status zurück (für Befehle vom Typ Info).

Einstellungen :

-   int id

jeeObject::byId
------------

Gibt das angegebene Objekt zurück

Einstellungen:

-   int id

jeeObject::fullById
----------------

Gibt ein Objekt, seine Ausrüstung und für jede Ausrüstung allee seine Befehle sowie die Zellenzustände zurück (für Befehle vom Typ Info).

jeeObject::save
------------

Gibt das angegebene Objekt zurück

Einstellungen:

-   int id (leer, wenn es sich um eine Kreation handelt)

-   Zeichenfolgenname

-   int Vater\_id = null

-   int isVisible = 0

-   int position

-   Array-Konfiguration

-   Array-Anzeige

JSON-Zusammenfassungs-API
================

summary::global
---------------

Gibt die insgesamte Zusammenfassung für den im Parameter übergebenen Schlüssel zurück

Einstellungen:

-   String-Schlüssel : (optional), Schlüssel der gewünschten Zusammenfassung. Wenn leer, sendet Jeedom Ihnen die Zusammenfassung alleer Schlüssel

summary::byId
-------------

Gibt die Zusammenfassung für die Objekt-ID zurück

Einstellungen:

-   int id : Objekt-ID

-   String-Schlüssel : (optional), Schlüssel der gewünschten Zusammenfassung. Wenn leer, sendet Jeedom Ihnen die Zusammenfassung alleer Schlüssel

JSON EqLogic API
================

eqLogic::all
------------

Gibt die Liste alleer Geräte zurück

eqLogic::fullById
-----------------

Gibt Geräte und ihre Befehle sowie deren Status zurück (für Befehle vom Typ Info).

Einstellungen:

-   int id

eqLogic::byId
-------------

Gibt das angegebene Gerät zurück

Einstellungen:

-   int id

eqLogic::byType
---------------

Gibt allee Geräte zurück, die zum angegebenen Typ gehören (Plugin).

Einstellungen:

-   Zeichenfolgentyp

eqLogic::byObjectId
-------------------

Gibt allee Geräte zurück, die zum angegebenen Objekt gehören

Einstellungen:

-   int object\_id

eqLogic::byTypeAndId
--------------------

Gibt eine Gerätetabelle gemäß den Parametern zurück. 

Die Rückgabe erfolgt vom Formulararray (&#39;eqType1&#39; ⇒array (&#39;id&#39;⇒…,&#39; cmds &#39;⇒)
Array (….)), &#39;eqType2&#39; ⇒array (&#39;id&#39;⇒…,&#39; cmds &#39;⇒ Array (….))….,id1 ⇒
Array (&#39;id&#39;⇒…,&#39; cmds &#39;⇒ Array (….)), id2 ⇒ Array (&#39; id&#39;⇒…, &#39;cmds&#39; ⇒
array(…​.))..)

Einstellungen:

-   string \ [\] eqType = Tabelle der erforderlichen Gerätetypen

-   int \ [\] id = Tabelle der gewünschten benutzerdefinierten Geräte-IDs

eqLogic::save
-------------

Gibt das registrierte / erstellte Gerät zurück

Einstellungen:

-   int id (leer, wenn es sich um eine Kreation handelt)

-   Zeichenfolge eqType\_name (Skripttyp, virtuelle Ausrüstung usw.)

-   Zeichenfolgenname

-   Zeichenfolge Protokollische ID = ''

-   int object\_id = null

-   int eqReal\_id = null

-   int isVisible = 0

-   int isEnable = 0

-   Array-Konfiguration

-   int timeout

-   Array-Kategorie

JSON Cmd API
============

cmd::all
--------

Gibt die Liste alleer Befehle zurück

cmd::byId
---------

Gibt den angegebenen Befehl zurück

Einstellungen:

-   int id

cmd::byEqLogicId
----------------

Gibt allee Bestellungen zurück, die zum angegebenen Gerät gehören

Einstellungen:

-   int eqLogic\_id

cmd::execCmd
------------

Führen Sie den angegebenen Befehl aus

Einstellungen:

-   int id : Befehls-ID oder ID-Array, wenn Sie mehrere Befehle gleichzeitig ausführen möchten
    
-   \ [Optionen \] Liste der Befehlsoptionen (abhängig vom Typ und Subtyp des Befehls)

cmd::getStatistique
-------------------

Gibt Statistiken zur Bestellung zurück (funktioniert nur bei Informationen und historischen Bestellungen)

Einstellungen:

-   int id

-   Zeichenfolge startTime : Startdatum der Statistikberechnung

-   Zeichenfolge endTime : Enddatum der Statistikberechnung

cmd::getTendance
----------------

Gibt den Trend der Bestellung zurück (funktioniert nur bei Informationen und historischen Bestellungen)

Einstellungen:

-   int id

-   Zeichenfolge startTime : Startdatum der Trendberechnung

-   Zeichenfolge endTime : Enddatum der Trendberechnung

cmd::getHistory
---------------

Gibt den Bestellverlauf zurück (funktioniert nur bei Informationen und historischen Aufträgen)

Einstellungen:

-   int id

-   Zeichenfolge startTime : Startdatum der Geschichte

-   Zeichenfolge endTime : Enddatum der Geschichte

cmd::save
---------

Gibt das angegebene Objekt zurück

Einstellungen:

-   int id (leer, wenn es sich um eine Kreation handelt)

-   Zeichenfolgenname

-   Zeichenfolge Protokollische ID

-   Zeichenfolge eqType

-   Zeichenfolgenreihenfolge

-   Zeichenfolgentyp

-   String-Subtyp

-   int eqLogic\_id

-   int isHistorized = 0

-   String-Einheit = ''

-   Array-Konfiguration

-   Array-Vorlage

-   Array-Anzeige

-   Array HTML

-   int value = null

-   int isVisible = 1

-   Array-Alarm

cmd::event
-------------------

Ermöglicht das Senden eines Werts an eine Bestellung

Einstellungen:

-   int id

-   Zeichenfolgenwert : Wert

-   Zeichenfolge Datetime : (optional) Wert Datetime

JSON-Szenario-API
=================

scenario::all
-------------

Gibt die Liste alleer Szenarien zurück

scenario::byId
--------------

Gibt das angegebene Szenario zurück

Einstellungen:

-   int id

scenario::export
----------------

Gibt den Export des Szenarios sowie den * menschlichen Namen * des Szenarios zurück

Einstellungen:

-   int id

scenario::import
----------------

Ermöglicht das Importieren eines Szenarios.

Einstellungen:

-   int id : ID des Szenarios, in das Importiert werden soll (leer, wenn erstellt)

-   Zeichenfolge humanName : *menschlicher Name * des Szenarios (leer bei Erstellung)

-   Array-Import : Szenario (aus dem Feld Exportszenario::export)

scenario::changeState
---------------------

Ändert den Status des angegebenen Szenarios.

Einstellungen:

-   int id

-   Zeichenfolgenstatus: \ [Run, Stop, aktivieren, deaktivieren \]

JSON-Protokoll-API
============

log::get
--------

Ermöglicht das Abrufen eines Protokolls

Einstellungen:

-   Zeichenfolgenprotokoll : Name des abzurufenden Protokolls 

-   String-Start : Zeilennummer, auf der mit dem Lesen begonnen werden soll

-   Zeichenfolge nbLine : Anzahl der wiederherzustellenden Zeilen 

log::add
--------

Ermöglicht das Schreiben in ein Protokoll

Einstellungen:

-   Zeichenfolgenprotokoll : Name des abzurufenden Protokolls 

-   Zeichenfolgentyp : Protokolltyp (Debug, Info, Warnung, Fehler)

-   Zeichenfolge Nachricht : SMS zu schreiben

-   Zeichenfolge Protokollische ID : Protokollische ID der generierten Nachricht


log::list
---------

Holen Sie sich die Jeedom-Protokollliste

Einstellungen:

-   String-Filter : (optional) Filter nach dem Namen der abzurufenden Protokolle 

log::empty
----------

Leeren Sie ein Protokoll

Einstellungen:

-   Zeichenfolgenprotokoll : Name des zu leeren Protokolls

log::remove
-----------

Ermöglicht das Löschen eines Protokolls

Einstellungen:

-   Zeichenfolgenprotokoll : Protokollname zum Löschen

JSON-Datenspeicher-API (Variable)
=============================

datastore::byTypeLinkIdKey
--------------------------

Ruft den Wert einer im Datenspeicher gespeicherten Variablen ab

Einstellungen:

-   Zeichenfolgentyp : Art des gespeicherten Werts (für Szenarien ist es Szenario)
    
-   id linkId : -1 für das insgesamte (Wert für die Standardszenarien oder die Szenario-ID)
    
-   String-Schlüssel : Wertname

datastore::save
---------------

Speichert den Wert einer Variablen im Datenspeicher

Einstellungen:

-   Zeichenfolgentyp : Art des gespeicherten Werts (für Szenarien
    es ist Szenario)

-   id linkId : -1 für insgesamt (Wert für Standardszenarien,
    oder die Szenario-ID)

-   String-Schlüssel : Wertname

-   gemischter Wert : Wert aufzuzeichnen

JSON-Nachrichten-API
================

message::all
------------

Gibt die Liste alleer Nachrichten zurück

message::add
--------

Ermöglicht das Schreiben in ein Protokoll

Einstellungen:

-   Zeichenfolgentyp : Protokolltyp (Debug, Info, Warnung, Fehler)

-   Zeichenfolge Nachricht : Nachricht

-   String-Aktion : Aktion

-   Zeichenfolge Protokollische ID : Protokollische ID

message::removeAll
------------------

Löschen Sie allee Nachrichten

JSON-Interaktions-API
====================

interact::tryToReply
--------------------

Versuchen Sie, eine Anfrage mit einer Interaktion abzugleichen, führen Sie die Aktion aus und antworten Sie entsprechend

Einstellungen:

-   Abfrage (Anforderungsphrase)

-   int reply\_cmd = NULL : Befehls-ID, die zum Antworten verwendet werden soll,
    Wenn nicht angegeben, gibt Jeedom die Antwort an Sie im JSON zurück

interactQuery::all
------------------

Gibt die vollständige Liste alleer Interaktionen zurück

JSON-System-API
===============

jeedom::halt
------------

Stoppen Sie Jeedom

jeedom::reboot
--------------

Starten Sie Jeedom neu

jeedom::isOk
------------

Lässt Sie wissen, ob der insgesamte Zustand von Jeedom in Ordnung ist

jeedom::update
--------------

Starten wir ein Jeedom-Update

jeedom::backup
--------------

Ermöglicht das Starten eines Backups von Jeedom

jeedom::getUsbMapping
---------------------

Liste der USB-Anschlüsse und Namen der daran angeschlossenen USB-Sticks

JSON Plugin API
===============

plugin::install
---------------

Installation / Update eines bestimmten Plugins

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::remove
--------------

Löschen eines bestimmten Plugins

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::dependancyInfo
----------------------

Gibt Informationen zum Plugin-Abhängigkeitsstatus zurück

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::dependancyInstall
-------------------------

Erzwingen Sie die Installation von Plugin-Abhängigkeiten

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::deamonInfo
------------------

Gibt Informationen zum Status des Plugin-Daemons zurück

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::deamonStart
-------------------

Zwinge den Dämon zu starten

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::deamonStop
------------------

Dämonenstopp erzwingen

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

plugin::deamonChangeAutoMode
----------------------------

Ändern Sie den Verwaltungsmodus des Dämons

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)
-   int-Modus : 1 für automatisch, 0 für manuell

JSON-Update-API
===============

update::all
-----------

Zurück zur Liste alleer installierenierten Komponenten, ihrer Versionen und der zugehörigen Informationen

update::checkUpdate
-------------------

Ermöglicht die Suche nach Updates

update::update
--------------

Ermöglicht das Aktualisieren von Jeedom und alleen Plugins

update::doUpdate
--------------

Einstellungen:

-   int Plugin\_id (optional) : Plugin ID
-   Zeichenfolge Protokollische ID (optional) : Plugin Name (logischer Name)

JSON-Netzwerk-API
================

network::restartDns
-------------------

Erzwingen Sie den (Neustart) des Jeedom DNS

network::stopDns
----------------

Erzwingt das Anhalten des DNS Jeedom

network::dnsRun
---------------

Gibt den Jeedom DNS-Status zurück

JSON-API-Beispiele
=================

Hier ist ein Beispiel für die Verwendung der API. Für das folgende Beispiel
Ich benutze [diese PHP-Klasse](https://github.com/jeedom/core/blob/release/core/class/jsonrpcClient.class.php)
Dies vereinfacht die Verwendung der API.

Abrufen der Objektliste :

`` `{.php}
$jsonrpc = new jsonrpcClient('#URL_JEEDOM#/core/api/jeeApi.php', #API_KEY#);
if ($ jsonrpc-&gt; sendrequest ( ‚jeeObject::alle &#39;, array ())){
    print_r ($ jsonrpc-&gt; bekommenResult ());
}else{
    echo $ jsonrpc-&gt; bekommenError ();
}
`` ''

Ausführung eines Auftrags (mit der Option eines Titels und einer Nachricht)

`` `{.php}
$jsonrpc = new jsonrpcClient('#URL_JEEDOM#/core/api/jeeApi.php', #API_KEY#);
if ($ jsonrpc-&gt; sendrequest ( ‚cmd::ExecCmd &#39;, Array (&#39; id &#39;=> # cmd_id #,&#39; options &#39;=> array (&#39; title &#39;=>&#39; Cuckoo &#39;,&#39; Nachricht &#39;=>&#39; It works &#39;))){
    Echo &#39;OK&#39;;
}else{
    echo $ jsonrpc-&gt; bekommenError ();
}
`` ''

Die API kann natürlich auch mit anderen Sprachen verwendet werden (nur ein Beitrag auf einer Seite).
