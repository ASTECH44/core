Hier ist der wichtigste Teil in der Hausautomation : die Szenarien.
Das wahre Gehirn der Domotiker macht es möglich, mit ihm zu interagieren
die reale Welt auf "intelligente Weise".

Die Seite zur Verwaltung von Szenarien
================================

Gestion
-------

Um darauf zuzugreifen, gehen Sie einfach zu Extras ->
Szenarien. Dort finden Sie auch die Liste der Szenarien für Ihr Jeedom
funktioniert nur, um sie besser zu verwalten :

-   **Ajouter** : Erstellen Sie ein Szenario. Die Vorgehensweise wird beschrieben
    im nächsten Kapitel.

-   **Szenarien deaktivieren** : Deaktiviert alle Szenarien.

-   **Siehe Variablen** : Sehen wir uns auch die Variablen und ihren Wert an
    dass der Ort, an dem sie verwendund werden. Sie können auch
    erstellen Sie eine. Variablen werden in einem Kapitel von beschrieben
    diese Seite.

-   **Übersicht** : Ermöglicht Ihnen einen Überblick über alle
    die Szenarien. Sie können die Werte ändern **actif**,
    **visible**, **Multi-Launch**, **synchroner Modus**, **Log** et
    **Timeline** (Diese Parameter werden im nächsten Kapitel beschrieben.).
    Sie können auch auf die Protokolle für jedes Szenario und zugreifen
    einzeln starten.

-   **Expressionstester** : Ermöglicht das Ausführen eines Tests für a
    Ausdruck Ihrer Wahl und zeigen Sie das Ergebnis.

Meine Szenarien
-------------

In diesem Abschnitt finden Sie die **Liste der Szenarien** dass du
erstellt haben. Sie sind klassifiziert nach **groupes** das hast du
für jeden von ihnen definiert. Jedes Szenario wird mit seinem angezeigt **nom**
und seine **übergeordnetes Objekt**. Die **ausgegraute Szenarien** sind diejenigen, die sind
untauglich.

Stellen Sie die Maus wie auf vielen Jeedom-Seiten links von
Auf dem Bildschirm wird ein Schnellzugriffsmenü angezeigt (von
Ihr Profil können Sie jederzeit sichtbar lassen). Du kannst
dann **chercher** Ihr Szenario, aber auch in **ajouter** eins davon
menu.

Szenario bearbeiten
=====================

Nach dem Klicken auf **Ajouter**, Sie müssen den Namen Ihres wählen
Szenario und Sie werden auf die Seite mit den allgemeinen Einstellungen weitergeleitet.
Oben finden Sie einige nützliche Funktionen zum Verwalten unseres Szenarios
:

-   **ID** : Neben dem Wort **General**, Dies ist die Szenariokennung.

-   **statut** : Aktueller Status Ihres Szenarios.

-   **variables** : Variablen anzeigen.

-   **Expression** : Zeigt den Ausdruckstester an.

-   **Ausführen** : Ermöglicht das manuelle Starten des Szenarios (Denken Sie daran
    vorher nicht sparen!). Die Auslöser sind daher nicht
    nicht berücksichtigt.

-   **Supprimer** : Szenario löschen.

-   **Sauvegarder** : Speichern Sie die vorgenommenen Änderungen.

-   **Template** : Ermöglicht den Zugriff auf und das Anwenden von Vorlagen
    zum Drehbuch vom Markt. (am Ende der Seite erklärt).

-   **Exporter** : Holen Sie sich eine Textversion des Skripts.

-   **Log** : Zeigt die Szenarioprotokolle an.

-   **Dupliquer** : Kopieren Sie das Szenario, um eines zu erstellen
    neu mit einem anderen Namen.

-   **Liens** : Ermöglicht das Anzeigen des Diagramms der verknüpften Elemente
    mit dem Skript.

Registerkarte &quot;Allgemein&quot;
--------------

In der Registerkarte **General**, wir finden die Hauptparameter von
unser Szenario :

-   **Name des Szenarios** : Der Name Ihres Szenarios.

-   **Name, der angezeigt werden soll** : Der Name, der für die Anzeige verwendund wird.

-   **Groupe** : Ermöglicht das Organisieren der Szenarien durch Klassifizieren in
    Gruppen.

-   **Actif** : Aktivieren Sie das Szenario.

-   **Visible** : Wird verwendet, um das Szenario sichtbar zu machen.

-   **übergeordnetes Objekt** : Zuordnung zu einem übergeordneten Objekt.

-   **Timeout Sekunden (0 = unbegrenzt)** : Die maximale Ausführungszeit
    autorisiert

-   **Multi-Launch** : Aktivieren Sie dieses Kontrollkästchen, wenn Sie das möchten
    Das Szenario kann mehrmals gleichzeitig gestartund werden.

-   **Synchroner Modus** : Starten Sie das Szenario im aktuellen Thread anstelle eines dedizierten Threads. Dies erhöht die Startgeschwindigkeit des Szenarios, kann jedoch das System instabil machen.

-   **Log** : Der für das Szenario gewünschte Protokolltyp.

-   **Folgen Sie der Zeitleiste** : Verfolgt das Szenario
    in der Zeitleiste.

-   **Description** : Ermöglicht das Schreiben eines kleinen zu beschreibenden Textes
    Ihr Szenario.

-   **Szenariomodus** : Das Szenario kann programmiert, ausgelöst oder
    beide gleichzeitig. Sie haben dann die Wahl, die (s) anzugeben.
    Trigger (s) (Vorsicht, die Anzahl der möglichen Trigger pro Szenario ist auf 15 begrenzt) und die Programmierung (en).

> **Tip**
>
> Aufmerksamkeit : Sie können maximal 28 haben
> Trigger / Programmierung für ein Szenario.

Registerkarte &quot;Szenario&quot;
---------------

Hier erstellen Sie Ihr Szenario. Wir müssen anfangen
durch **Fügen Sie einen Block hinzu**, mit dem Knopf rechts. Einmal ein Block
erstellt, können Sie eine weitere hinzufügen **bloc** oder a **action**.

> **Tip**
>
> In Bedingungen und Aktionen ist es besser, einfache Anführungszeichen (&#39;) anstelle von doppelten (&quot;) zu bevorzugen.

### Blöcke

Hier sind die verschiedenen Arten von Blöcken verfügbar :

-   **If / Then / Oder** : Ermöglicht das Ausführen von Aktionen
    unter Bedingung (en).

-   **Action** : Ermöglicht das Starten einfacher Aktionen ohne
    keine Bedingungen.

-   **Boucle** : Ermöglicht das wiederholte Ausführen von Aktionen
    1 bis zu einer definierten Zahl (oder sogar dem Wert eines Sensors oder a
    Zufallszahl…).

-   **Dans** : Startund eine Aktion in X Minute (n) (0 ist a
    möglicher Wert). Die Besonderheit ist, dass die Aktionen gestartund werden
    im Hintergrund, damit sie den Rest des Szenarios nicht blockieren.
    Es ist also ein nicht blockierender Block.

-   **A** : Ermöglicht es Jeedom, die Aktionen des Blocks beich a zu starten
    gegebene Zeit (in der Form hhmm). Dieser Block ist nicht blockierend. Ex :
    0030 für 00:30 oder 0146 für 1h46 und 1050 für 10h50.

-   **Code** : Ermöglicht das direkte Schreiben in PHP-CODE (Anfrage
    etwas Wissen und kann riskant sein, erlaubt aber nicht zu haben
    keine Einschränkungen).

-   **Commentaire** : Ermöglicht das Hinzufügen von Kommentaren zu Ihrem Szenario.

Jeder dieser Blöcke hat seine Optionen für eine bessere Handhabung :

-   Mit dem Kontrollkästchen links können Sie das Kontrollkästchen vollständig deaktivieren
    blockieren, ohne es zu löschen.

-   Mit dem vertikalen Doppelpfeil links können Sie das Ganze verschieben
    Blockieren per Drag &amp; Drop.

-   Mit der Schaltfläche ganz rechts können Sie den gesamten Block löschen.

#### Wenn / Dann / Sonst blockiert, Loop, In und Bis.

> **Note**
>
> Auf Sich / Then / Sonst-Blöcken befinden sich Kreispfeile
> links neben dem Bedingungsfeld aktivieren oder nicht aktivieren
> Wiederholung von Handlungen, wenn die Bewertung des Zustands dasselbe ergibt
> Ergebnis, dass die vorherige Bewertung.

Für die Bedingungen versucht Jeedom sicherzustellen, dass wir können
Schreiben Sie so viel wie möglich in natürlicher Sprache und bleiben Sie dabeich flexibel. drei
Rechts neben diesem Blocktyp stehen Schaltflächen für zur Verfügung
Wählen Sie ein zu testendes Element aus :

-   **Finden Sie eine Bestellung** : Ermöglicht die Suche nach einer Bestellung in
    alle in Jeedom verfügbaren. Sobald die Bestellung gefunden ist,
    Jeedom öffnund ein Fenster und fragt Sie, welchen Test Sie möchten
    darauf ausführen. Wenn Sie möchten **Setzen Sie nichts**,
    Jeedom wird die Bestellung ohne Vergleich hinzufügen. Sie können auch
    wählen **et** oder **ou** Front **Ensuite** zu Kettentests
    auf verschiedenen Geräten.

-   **Suchen Sie ein Szenario** : Suchen wir nach einem Szenario
    zu testen.

-   **Suche nach Ausrüstung** : Gleiches gilt für die Ausrüstung.

> **Tip**
>
> Es gibt eine Liste von Tags, die den Zugriff auf Variablen ermöglichen
> aus dem Skript oder einem anderen oder nach Uhrzeit, Datum, a
> Zufallszahl,…. Weitere Informationen finden Sie in den Kapiteln zu Befehlen und
> Tags.

Sobald die Bedingung erfüllt ist, müssen Sie die Schaltfläche verwenden
"add ", links, um ein neues hinzuzufügen **bloc** oder a
**action** im aktuellen Block.

> **Tip**
>
> Sie dürfen [] NICHT in Bedingungstests verwenden, nur Klammern () sind möglich

#### Blockcode

> **Important**
>
> Bitte beachten Sie, dass Tags in einem Codeblock nicht verfügbar sind.

Bedienelemente (Sensoren und Aktoren):
-   cmd::byString ($ string); : Gibt das entsprechende Befehlsobjekt zurück.
  -   $string : Link zur gewünschten Bestellung : #[Objekt] [Bisusrüstung] [Befehl] # (z : #[Wohnung] [Bislarm] [Bisktiv] #)
-   cmd::BYIdentifikation ($ id); : Gibt das entsprechende Befehlsobjekt zurück.
  -   $id : Bestellnummer
-   $cmd->execCmd($options = null); : Führen Sie den Befehl aus und geben Sie das Ergebnis zurück.
  -   $options : Optionen zur Ausführung des Befehls (möglicherweise Plugin-spezifisch), Basisoption (Befehlssubtyp) :
    -   Nachricht : $option = array('title' => 'titre du Nachricht , 'message' => 'Mon message');
    -   Farbe : $option = array('color' => 'couleur en hexadécimal');
    -   Schieber : $option = array('slider' => 'valeur voulue de 0 à 100');

Log :
-   log::add ( &#39;Dateiname&#39; &#39;Stufe&#39;, &#39;message&#39;);
  -   Dateiname : Name der Protokolldatei.
  -   Ebene : [Debug], [Info], [Fehler], [Ereignis].
  -   Nachricht : Nachricht zum Schreiben in die Protokolle.

Szenario :
-   $scenario->getName(); : Gibt den Namen des aktuellen Szenarios zurück.
-   $scenario->getGroup(); : Gibt die Szenariogruppe zurück.
-   $scenario->getIsActive(); : Gibt den Status des Szenarios zurück.
-   $scenario->setIsActive($active); : Ermöglicht das Aktivieren oder Nicht-Aktivieren des Szenarios.
  -   $active : 1 aktiv, 0 nicht aktiv.
-   $scenario->setOnGoing($onGoing); : Sagen wir, ob das Szenario läuft oder nicht.
  -   $onGoing => 1 en cours , 0 arrêté.
-   $scenario->save(); : Änderungen speichern.
-   $scenario->setData($key, $value); : Daten speichern (Variable).
  -   $key : Werteschlüssel (int oder string).
  -   $value : zu speichernder Wert (int, string, array oder object).
-   $scenario->getData($key); : Daten abrufen (variabel).
  -   $key => Werteschlüssel (int oder string).
-   $scenario->removeData($key); : Daten löschen.
-   $scenario->setLog($message); : Schreiben Sie eine Nachricht in das Szenario-Protokoll.
-   $scenario->persistLog(); : Erzwingen Sie das Schreiben des Protokolls (andernfalls wird es nur am Ende des Szenarios geschrieben). Seien Sie vorsichtig, dies kann das Szenario etwas verlangsamen.

### Aktionen

Zu Blöcken hinzugefügte Aktionen haben mehrere Optionen. In Ordnung :

-   Eine Kiste **parallel** so dass dieser Befehl parallel gestartund wird
    andere Befehle ebenfalls ausgewählt.

-   Eine Kiste **aktiviert** damit dieser Befehl berücksichtigt wird
    Konto im Szenario.

-   Ein **vertikaler Doppelpfeil** um die Aktion zu verschieben. Einfach
    von dort ziehen und ablegen.

-   Eine Schaltfläche zum Löschen der Aktion.

-   Eine Schaltfläche für bestimmte Aktionen, jedes Mal mit dem
    Beschreibung dieser Aktion.

-   Eine Schaltfläche zum Suchen nach einem Aktionsbefehl.

> **Tip**
>
> Abhängig vom ausgewählten Befehl können wir unterschiedliche sehen
> zusätzliche Felder angezeigt.

Mögliche Substitutionen
===========================

Auslöser
----------------

Es gibt bestimmte Auslöser (außer denen von
Befehle) :

-   #start# : ausgelöst beim (Wieder-) Start von Jeedom,

-   #begin_backup# : Ereignis, das zu Beginn einer Sicherung gesendund wurde.

-   #end_backup# : Ereignis, das am Ende einer Sicherung gesendund wird.

-   #BEGIN_UPDATE# : Ereignis, das zu Beginn eines Updates gesendund wurde.

-   #END_UPDATE# : Ereignis, das am Ende eines Updates gesendund wurde.

-   #begin_restore# : Ereignis zu Beginn einer Restaurierung gesendet.

-   #end_restore# : Ereignis am Ende einer Restaurierung gesendet.

-   #user_connect# : Benutzer Login

Sie können auch ein Szenario auslösen, wenn eine Variable auf gesetzt ist
Etikett setzen : #Variable (Variablenname) # oder über die HTTP-API
beschrieben
[hier](https://jeedom.github.io/core/fr_FR/api_http).

Vergleichsoperatoren und Verknüpfungen zwischen Bedingungen
-------------------------------------------------------

Sie können eines der folgenden Symbole für verwenden
Vergleiche in Bedingungen :

-   == : gleich,

-   \.> : streng größer als,

-   \.>= : größer als oder gleich,

-   < : streng weniger als,

-   <= : kleiner als oder gleich,

-   != : anders als, ist nicht gleich,

-   Streichhölzer : enthält (z :
    [Badezimmer] [Hydrometrie] [Zustand] entspricht "/ wund /"),

-   nicht (… passt…) : enthält nicht (z :
    nicht ([Badezimmer] [Hydrometrie] [Zustand] stimmt mit "/ wund /" überein)),

Sie können jeden Vergleich mit Operatoren kombinieren
folgende :

-   &amp;&amp; / ET / und / AND / und : et,

-   \.|| / OR / oder / OR / oder : ou,

-   \.|^ / XOR / xor : oder exklusiv.

Tags
--------

Ein Etikett wird während der Ausführung des Szenarios durch seinen Wert ersetzt. Sie
kann die folgenden Tags verwenden :

> **Tip**
>
> Verwenden Sie die Taste, um die führenden Nullen anzuzeigen
> Date () Funktion. Ansicht
> [hier](http://php.net/manual/fr/function.date.php).

-   #seconde# : Aktuelle Sekunde (ohne führende Nullen, z : 6 für
    08:07:06),

-   #heure# : Aktuelle Zeit im 24h-Format (ohne führende Nullen,
    ex : 8 für 08:07:06 oder 17 für 17:15),

-   #heure12# : Aktuelle Zeit im 12-Stunden-Format (ohne führende Nullen,
    ex : 8 für 08:07:06),

-   #minute# : Aktuelle Minute (ohne führende Nullen, z : 7 für
    08:07:06),

-   #jour# : Aktueller Etikett (ohne führende Nullen, z : 6 für
    2017.06.07),

-   #mois# : Aktueller Monat (ohne führende Nullen, z : 7 für
    2017.06.07),

-   #annee# : Laufendes Jahr,

-   #time# : Aktuelle Stunde und Minute (z : 1715 für 17.15 Uhr),

-   #timestamp# : Anzahl der Sekunden seit dem 1. Januar 1970,

-   #date# : Etikett und Monat. Achtung, die erste Zahl ist der Monat.
    (zB : 1215 für den 15. Dezember),

-   #semaine# : Wochennummer (z : 51),

-   #sjour# : Name des Wochentags (z : Samedi),

-   #njour# : Tagesnummer von 0 (Sonntag) bis 6 (Samstag),

-   #smois# : Name des Monats (z : Janvier),

-   #IP# : Jeedom&#39;s interne IP,

-   #hostname# : Name der Jeedom-Maschine,

-   #trigger# : Möglicherweise der Name des Befehls, der das Szenario gestartund hat: &quot;API&quot;, wenn der Start von der API gestartund wurde, &quot;Zeitplan&quot;, wenn er durch Programmierung gestartund wurde, &quot;Benutzer&quot;, wenn er manuell gestartund wurde

Sie haben auch die folgenden zusätzlichen Tags, wenn Ihr Skript gewesen ist
ausgelöst durch eine Interaktion :

-   #query# : Interaktion, die das Szenario ausgelöst hat,

-   #profil# : Profil des Benutzers, der das Szenario gestartund hat
    (kann leer sein).

> **Important**
>
> Wenn ein Szenario durch eine Interaktion ausgelöst wird, ist dies der Fall
> muss unbedingt im schnellen Modus laufen.

Berechnungsfunktionen
-----------------------

Für das Gerät stehen verschiedene Funktionen zur Verfügung :

-   Durchschnitt (Reihenfolge, Zeitraum) und Durchschnitt zwischen (Reihenfolge, Start, Ende)
    : Geben Sie den Durchschnitt der Bestellung über den Zeitraum an
    (Zeitraum = [Monat, Tag, Stunde, Minute] oder [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    zwischen den 2 erforderlichen Klemmen (in der Form Ymd H.:i:s oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   min (Reihenfolge, Periode) und minBetween (Reihenfolge, Start, Ende) :
    Geben Sie die Mindestbestellmenge über den Zeitraum an
    (Zeitraum = [Monat, Tag, Stunde, Minute] oder [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    zwischen den 2 erforderlichen Klemmen (in der Form Ymd H.:i:s oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   max (Reihenfolge, Periode) und maxBetween (Reihenfolge, Start, Ende) :
    Geben Sie das Maximum der Bestellung über den Zeitraum an
    (Zeitraum = [Monat, Tag, Stunde, Minute] oder [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    zwischen den 2 erforderlichen Klemmen (in der Form Ymd H.:i:s oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   Dauer (Reihenfolge, Wert, Zeitraum) und
    durationbetween (Sollwert, Start, Ende) : Geben Sie die Dauer in an
    Minuten, in denen das Gerät den auf dem
    Periode (Periode = [Monat, Tag, Stunde, Minute] oder [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    zwischen den 2 erforderlichen Klemmen (in der Form Ymd H.:i:s oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   Statistiken (Reihenfolge, Berechnung, Zeitraum) und
    statisticsBetween (Kontrolle, Berechnung, Beginn, Ende) : Geben Sie das Ergebnis
    verschiedene statistische Berechnungen (Summe, Anzahl, Standard,
    Varianz, Durchschnitt, Min, Max) über den Zeitraum
    (Zeitraum = [Monat, Tag, Stunde, Minute] oder [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    zwischen den 2 erforderlichen Klemmen (in der Form Ymd H.:i:s oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   Trend (Befehl, Zeitraum, threshold) : Gibt den Trend von
    Bestellung über den Zeitraum (Zeitraum = [Monat, Tag, Stunde, Minute] oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   stateDuration (Kontrolle) : Gibt die Dauer in Sekunden an
    seit der letzten Wertänderung. Gibt -1 zurück, wenn keine vorhanden ist
    Verlauf existiert nicht oder wenn der Wert nicht in der Geschichte existiert.
    Gibt -2 zurück, wenn die Bestellung nicht protokolliert wird.

-   lastChangeStateDuration (Sollwert) : Geben Sie die Dauer in an
    Sekunden seit der letzten Zustandsänderung auf den übergebenen Wert
    als Parameter. Gibt -1 zurück, wenn keine vorhanden ist
    Verlauf existiert nicht oder wenn der Wert nicht in der Geschichte existiert.
    Gibt -2 zurück, wenn die Bestellung nicht protokolliert wird

-   lastStateDuration (Sollwert) : Gibt die Dauer in Sekunden an
    währenddessen hat das Gerät kürzlich den gewählten Wert gehabt.
    Gibt -1 zurück, wenn kein Verlauf vorhanden ist oder wenn der Wert nicht im Verlauf vorhanden ist.
    Gibt -2 zurück, wenn die Bestellung nicht protokolliert wird

-   stateChanges (order, [value], period) und
    stateChangesBetween (Befehl, [Wert], Start, Ende) : Gib das
    Anzahl der Statusänderungen (auf einen bestimmten Wert, falls angegeben,
    oder insgesamt anders) über den Zeitraum (Zeitraum = [Monat, Tag, Stunde, Minute] oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) ou
    zwischen den 2 erforderlichen Klemmen (in der Form Ymd H.:i:s oder
    [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   lastBetween (command, Beginn, Ende) : Gibt den letzten Wert zurück
    registriert für das Gerät zwischen den 2 erforderlichen Terminals (unter der
    bilden Ymd H.:i:s oder [Bisusdruck
    PHP](http://php.net/manual/fr/datetime.formats.relative.php)) :

-   Variable (Variable, Standard) : Holen Sie sich den Wert von a
    Variable oder der gewünschte Standardwert :

-   Szenario (Szenario) : Gibt den Status des Szenarios zurück. 1 in Bearbeitung, 0
    wenn gestoppt und -1 wenn deaktiviert, -2 wenn das Szenario nicht existiert und -3
    wenn der Zustand nicht konsistent ist. Um den &quot;menschlichen&quot; Namen des Szenarios zu erhalten, können Sie die entsprechende Schaltfläche rechts neben der Szenariosuche verwenden.

-   lastScenarioExecution (Szenario) : Gibt die Dauer in Sekunden an
    seit dem letzten Start des Szenarios :

-   collectDate (cmd [size]) : Gibt das Datum der letzten Daten zurück
    für den als Parameter angegebenen Befehl der 2. optionale Parameter
    ermöglicht die Angabe des Rückgabeformats (Details
    [hier](http://php.net/manual/fr/function.date.php)). Eine Rückkehr von -1
    bedeutet, dass die Bestellung nicht gefunden werden kann und -2, dass die Bestellung nicht gefunden wird
    kein Infotyp

-   valueDate (cmd [size]) : Gibt das Datum der letzten Daten zurück
    für den als Parameter angegebenen Befehl der 2. optionale Parameter
    ermöglicht die Angabe des Rückgabeformats (Details
    [hier](http://php.net/manual/fr/function.date.php)). Eine Rückkehr von -1
    bedeutet, dass die Bestellung nicht gefunden werden kann und -2, dass die Bestellung nicht gefunden wird
    kein Infotyp

-   eqEnable (Ausrüstung) : Gibt den Status des Geräts zurück. -2 wenn
    Das Gerät kann nicht gefunden werden, 1 wenn das Gerät aktiv ist und 0 wenn es nicht aktiv ist
    ist inaktiv

-   Wert (cmd) : Gibt den Wert einer Bestellung zurück, wenn er nicht automatisch von Jeedom angegeben wird (Groß- und Kleinschreibung, wenn der Name der Bestellung in einer Variablen gespeichert wird).    

-   Etikett (Montag [Standard]) : Wird verwendet, um den Wert eines Tags oder abzurufen
    die Standardeinstellung, wenn sie nicht vorhanden ist :

-   (Art, Kontrolle) : Wird verwendet, um den Namen des Befehls abzurufen,
    Ausrüstung oder Gegenstand. Typ ist entweder cmd, eqLogic oder wert
    Objekt.

-   lastCommunication (Ausrüstung, [size]) : Gibt das Datum der letzten Kommunikation zurück
    für die als Parameter angegebene Ausrüstung der 2. optionale Parameter
    ermöglicht die Angabe des Rückgabeformats (Details
    [hier](http://php.net/manual/fr/function.date.php)). Eine Rückkehr von -1
    bedeutet, dass das Gerät nicht gefunden werden kann

-   color_gradient (couleur_debut, couleur_fin, valuer_min, valeur_max, value) : Gibt eine Farbe zurück, die in Bezug auf den Wert im Bereich color_Start / color_end berechnund wurde. Der Wert muss zwischen min_value und max_value liegen

Die Perioden und Intervalle dieser Funktionen können auch
Verwenden Sie mit [Bisusdrücken
PHP](http://php.net/manual/fr/datetime.formats.relative.php) comme par
Beispiel :

-   Jetzt : maintenant

-   Heute : 00:00 heute (ermöglicht zum Beispiel zu erhalten
    Ergebnisse des Tages zwischen &#39;Heute&#39; und &#39;Jetzt&#39;)

-   Letzten Montag : letzten Montag um 00:00

-   Vor 5 Tagen : Vor 5 Tagen

-   Gestern mittag : gestern mittag

-   Usw..

Hier finden Sie praktische Beispiele zum Verständnis der von zurückgegebenen Werte
diese verschiedenen Funktionen :

| Sockel mit Werten :           | 000 (für 10 Minuten) 11 (für 1 Stunde) 000 (für 10 Minuten)    |
|--------------------------------------|--------------------------------------|
| Durchschnitt (Mitnahmen, Periode)             | Gibt den Durchschnitt von 0 und 1 zurück (can  |
|                                      | durch Umfragen beeinflusst werden)      |
| Durchschnitt zwischen (\.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Gibt die durchschnittliche Bestellung zwischen dem 1. Januar 2015 und dem 15. Januar 2015 zurück                         |
| min (outlet, Periode)                 | Gibt 0 zurück : Der Stecker wurde während des Zeitraums gelöscht              |
| minBetween (\.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Gibt die Mindestbestellmenge zwischen dem 1. Januar 2015 und dem 15. Januar 2015 zurück                         |
| max (Entscheidung, Periode)                 | Rückgabe 1 : Der Stecker war in der Zeit gut beleuchtund              |
| maxBetween (\.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#, 2015-01-01 00:00:00,2015-01-15 00:00:00) | Gibt das Maximum der Bestellung zwischen dem 1. Januar 2015 und dem 15. Januar 2015 zurück                         |
| Dauer (Stecker, 1 Periode)          | Gibt 60 zurück : Der Stecker war in diesem Zeitraum 60 Minuten lang eingeschaltund (beich 1)                              |
| durationBetween (\.# [Salon] [Take] [State] \.#, 0, letzter Montag, jetzt)   | Gibt die Dauer in Minuten zurück, in der die Steckdose seit dem letzten Montag ausgeschaltund war.                |
| Statistiken (Fang, Anzahl, Zeitraum)    | Rückgabe 8 : In diesem Zeitraum gab es 8 Eskalationen               |
| Trend (Stecker, Periode 0.1)        | Gibt -1 zurück : Abwärtstrend    |
| stateDuration (Stecker)               | Gibt 600 zurück : Der Stecker befindund sich seit 600 Sekunden (10 Minuten) in seinem aktuellen Zustand.                             |
| lastChangeStateDuration (Fang, 0)   | Gibt 600 zurück : Die Steckdose ist vor 600 Sekunden (10 Minuten) zum letzten Mal ausgefallen (auf 0 geändert)     |
| lastChangeStateDuration (Fang, 1)   | Gibt 4200 zurück : Die Steckdose wurde vor 4200 Sekunden (1h10) zum letzten Mal eingeschaltund (auf 1 umschalten).                               |
| lastStateDuration (Fang, 0)         | Gibt 600 zurück : Die Steckdose war 600 Sekunden (10 Minuten) ausgeschaltet.     |
| lastStateDuration (Fang, 1)         | Gibt 3600 zurück : Die Steckdose wurde zuletzt für 3600 Sekunden (1 Stunde) eingeschaltet.           |
| stateChanges (Fang, Periode)        | Rückgabe 3 : Der Stecker hat während des Zeitraums dreimal den Zustand geändert            |
| stateChanges (Fang, 0, Periode)      | Rückgabe 2 : Die Steckdose ist während des Zeitraums zweimal erloschen (auf 0)                              |
| stateChanges (Fang, 1 Punkt)      | Rückgabe 1 : Der Stecker leuchtund während des Zeitraums einmal (auf 1 ändern)                              |
| lastBetween (\.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#, gestern, heute) | Gibt die zuletzt gestern aufgezeichnete Temperatur zurück.                    |
| Variable (Plopp, 10)                  | Gibt den Wert der Variablen plop oder 10 zurück, wenn sie leer ist oder nicht existiert                         |
| Szenario (\.# [Badezimmer] [Licht] [Bisuto] \.#) | Gibt 1 in Bearbeitung zurück, 0, wenn gestoppt, und -1, wenn deaktiviert, -2, wenn das Szenario nicht existiert, und -3, wenn der Status nicht konsistent ist                         |
| lastScenarioExecution (\.# [Badezimmer] [Licht] [Bisuto] \.#)   | Gibt 300 zurück, wenn das Szenario vor 5 Minuten zum letzten Mal gestartund wurde                                  |
| collectDate (\.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#)     | Rückgabe 2015-01-01 17:45:12          |
| valueDate (\.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#) | Rückgabe 2015-01-01 17:50:12          |
| eqEnable (\.# [Nein] [Basilika] \.#)       | Gibt -2 zurück, wenn das Gerät nicht gefunden wird, 1, wenn das Gerät aktiv ist, und 0, wenn es inaktiv ist          |
| Etikett (Montag toto)                   | Gibt den Wert von "montag" zurück, falls vorhanden, andernfalls wird der Wert "toto" zurückgegeben"                               |
| Name (eqLogic, \.# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] \.#)     | Gibt Hydrometrie zurück                  |

Mathematische Funktionen
---------------------------

Eine generische Funktions-Toolbox kann ebenfalls verwendund werden
Konvertierungen oder Berechnungen durchführen :

-   rand (1.10) : Geben Sie eine Zufallszahl von 1 bis 10 an.

-   randtext (text1, text2, Text ... ..) : Gibt einen von zurück
    Texte zufällig (Text durch einen trennen;). Es gibt keine
    Begrenzen Sie die Anzahl der Texte.

-   randomColor (min, max) : Gibt eine zufällige Farbe zwischen 2
    Klemmen (0 =&gt; rot, 50 =&gt; grün, 100 =&gt; blau).

-   Trigger (Kontrolle) : Wird verwendet, um den Auslöser für das Szenario herauszufinden
    oder um zu wissen, ob es die Reihenfolge ist, die als Parameter aufgegeben wurde
    löste das Szenario aus.

-   triggerValue (Kontrolle) : Wird verwendet, um den Wert von herauszufinden
    Szenario-Trigger.

-   round (value [dezimal]) : Runde oben [dezimal]
    Anzahl der Dezimalstellen nach dem Dezimalpunkt.

-   ungerade (Wert) : Lässt Sie wissen, ob eine Zahl ungerade ist oder nicht.
    Gibt 1 zurück, wenn sonst ungerade 0.

-   Median (command1, command2 ....BefehlN) : Gibt den Median zurück
    Werte.

-   time_op (Zeit, Wert) : Ermöglicht es Ihnen, Vorgänge pünktlich auszuführen,
    mit Zeit = Zeit (z : 1530) und value = Wert zum Hinzufügen oder Hinzufügen
    in Minuten subtrahieren.

-   `time_between (Zeit, Start, Ende)` : Ermöglicht das Testen, ob eine Zeit ist
    zwischen zweich Werten mit &quot;Zeit = Zeit&quot; (z : 1530), "Start = Zeit", "Ende = Zeit".
    Start- und Endwerte können sich über Mitternacht erstrecken.

-   `time_diff (date1, date1 [, format])` : Wird verwendet, um den Unterschied zwischen zweich Daten zu ermitteln (die Daten müssen das Format JJJJ / MM / TT HH haben:MM:SS).
    Standardmäßig (wenn Sie nichts für das Format angeben) gibt die Methode die Gesamtzahl der Tage zurück. Sie können es in Sekunden (s), Minuten (m), Stunden (h) fragen.. Beispiel in Sekunden `time_diff (2018-02-02 14:55:00,2018-02-25 14:55:00,s)`

-   `formatTime (Zeit)` : Formatiert die Rückgabe einer Kette
    `# Zeit #`.

-   Boden (Zeit / 60) : Konvertiert von Sekunden in Minuten oder
    Minuten bis Stunden (Boden (Zeit / 3600) für Sekunden
    in Stunden)

Und praktische Beispiele :


| Funktionsbeispiel                  | Zurückgegebenes Ergebnis                    |
|--------------------------------------|--------------------------------------|
| randText (es ist # [Wohnzimmer] [Bisuge] [Temperatur] #; Die Temperatur ist # [Wohnzimmer] [Bisuge] [Temperatur] #; Derzeit haben wir # [Wohnzimmer] [Bisuge] [Temperatur] #) | Die Funktion gibt beich jeder Ausführung zufällig einen dieser Texte zurück.                           |
| randomColor (40,60)                 | Gibt eine zufällige Farbe nahe Grün zurück.   
| Auslöser (# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] #)   | 1 wenn es gut ist \.# \. [Badezimmer \.] \. [Hydrometrie \.] \. [Luftfeuchtigkeit \.] \.#, was das Szenario ansonsten gestartund hat 0  |
| triggerValue (# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] #) | 80, wenn die Hydrometrie von \.# \. [Badezimmer \.] \. [Hydrometrie \.] \. [Luftfeuchtigkeit \.] \.# 80% beträgt.                         |
| rund (# [Badezimmer] [Hydrometrie] [Luftfeuchtigkeit] # / 10) | Gibt 9 zurück, wenn der Feuchtigkeitsprozentsatz und 85                     |
| ungerade (3)                             | Rückgabe 1                            |
| Median (15,25,20)                   | Rückgabe 20                           |
| time_op (# Zeit #, -90)               | Wenn es 16:50 Uhr ist, kehren Sie zurück : 1 650-1 130 = 1520                          |
| FormatZeit (1650)                   | Rückgabe 16:50 Uhr                        |
| Stock (130/60)                      | Gibt 2 zurück (Minuten beich 130 s oder Stunden beich 130 m)                      |

Spezifische Bestellungen
=========================

Zusätzlich zu den Befehlen für die Hausautomation haben Sie Zugriff auf die folgenden Aktionen :

-   **Pause** (Sleep) : Pause von x Sekunde (n).

-   **variable** (Variabel) : Erstellung / Änderung einer Variablen oder eines Wertes
    einer Variablen.

-   **Variable entfernen** (Delete_variable) : Ermöglicht das Löschen einer Variablen

-   **Szenario** (Szenario) : Ermöglicht die Steuerung von Szenarien. Der Tag-Teil
    ermöglicht das Senden von Tags an das Szenario, z : montag = 2 (seich dort vorsichtig
    Verwenden Sie nur Buchstaben von a bis z. Keine Großbuchstaben, nein
    Akzente und keine Sonderzeichen). Wir bekommen den Etikett in der
    Zielszenario mit der Tag-Funktion (montag). Mit dem Befehl &quot;SI zurücksetzen&quot; können Sie den Status von &quot;SI&quot; zurücksetzen (dieser Status wird verwendet, um die Aktionen eines &quot;SI&quot; nicht zu wiederholen, wenn Sie ihn zum zweiten Mal in Folge übergeben).

-   **Stop** (Stop) : Stoppen Sie das Szenario.

-   **Attendre** (WAIT) : Warten Sie, bis die Bedingung gültig ist
    (maximal 2h), Timeout ist in Sekunde (n).

-   **Gehe zum Design** (Gotodesign) : Ändern Sie das auf allen angezeigte Design
    Browser nach gewünschtem Design.

-   **Fügen Sie ein Protokoll hinzu** (Log) : Ermöglicht das Hinzufügen einer Nachricht zu den Protokollen.

-   **Nachricht erstellen** (Message) : Fügen Sie eine Nachricht in der Mitte hinzu
    von Nachrichten.

-   **Geräte ausblenden / deaktivieren** (Ausstattung) : Ermöglicht
    Ändern Sie die Eigenschaften eines Geräts
    sichtbar / unsichtbar, aktiv / inaktiv.

-   **Stellen Sie eine Anfrage** (Ask) : Ermöglicht es Ihnen, Jeedom zu bitten, zu fragen
    eine Frage an den Benutzer. Die Antwort wird in a gespeichert
    Variable, dann testen Sie einfach ihren Wert. Für den Moment,
    Nur SMS und Slack Plugins sind kompatibel. Seich vorsichtig, das
    Funktion blockiert. Solange es keine Antwort gibt oder die
    Timeout wird nicht erreicht, das Szenario wartet.

-   **Stoppen Sie Jeedom** (Jeedom_poweroff) : Bitten Sie Jeedom, herunterzufahren.

-   **Starten Sie Jeedom neu** (Jeedom_reboot) : Bitten Sie Jeedom, neu zu starten.

-   **Geben Sie einen Text / Daten zurück** (Scenario_return) : Gibt einen Text oder einen Wert zurück
    für eine Interaktion zum Beispiel.

-   **Symbol** (Symbol) : Ermöglicht das Ändern des Darstellungssymbols des Szenarios.

-   **Alerte** (Alert) : Ermöglicht das Anzeigen einer kleinen Warnmeldung für alle
    Browser mit geöffneter Jeedom-Seite. Du kannst
    Wählen Sie 4 Alarmstufen.

-   **Pop-up** (Popup) : Ermöglicht die Anzeige eines Popups, das unbedingt angezeigt werden muss
    Validiert in allen Browsern, in denen eine Jeedom-Seite geöffnund ist.

-   **Rapport** (Bericht) : Exportieren Sie eine Ansicht im Format (PDF, PNG, JPEG)
    oder SVG) und senden Sie es über einen Befehl vom Typ Nachricht.
    Bitte beachten Sie, dass Ihr Internetzugang in nicht signiertem HTTPS erfolgt
    Funktionalität wird nicht funktionieren. Signiertes HTTP oder HTTPS ist erforderlich.

-   **Programmierten IN / A-Block löschen** (Remove_inat) : Ermöglicht das Löschen der
    Programmierung aller Blöcke IN und Bis des Szenarios.

-   **Ereignis** (Ereignis) : Ermöglicht das willkürliche Übertragen eines Werts in einen Befehl vom Typ Information

-   **Tag** (Tag) : Ermöglicht das Hinzufügen / Ändern eines Tags (das Etikett ist nur während der aktuellen Ausführung des Szenarios vorhanden, im Gegensatz zu den Variablen, die das Ende des Szenarios überleben).

Szenariovorlage
====================

Mit dieser Funktion können Sie ein Szenario in eine Vorlage für umwandeln
Wenden Sie es beispielsweise auf ein anderes Jeedom an oder teilen Sie es auf dem
Markt. Von dort aus können Sie auch ein Szenario wiederherstellen
vom Markt.

![scenario15](../images/scenario15.JPG)

Sie sehen dann dieses Fenster :

![scenario16](../images/scenario16.JPG)

Von dort haben Sie die Möglichkeit :

-   Senden Sie vorher eine Vorlage an Jeedom (JSON-Datei)
    zurückgewonnen),

-   Konsultieren Sie die Liste der auf dem Markt verfügbaren Szenarien,

-   Erstellen Sie eine Vorlage aus dem aktuellen Szenario (vergessen Sie nicht
    einen Namen geben),

-   Um die Vorlagen zu konsultieren, die derzeit auf Ihrem Jeedom vorhanden sind.

Durch Klicken auf eine Vorlage erhalten Sie :

![scenario17](../images/scenario17.JPG)

Oben kannst du :

-   **Partager** : Teilen Sie die Vorlage auf dem Markt,

-   **Supprimer** : Vorlage löschen,

-   **Download** : Stellen Sie die Vorlage als JSON-Dateich wieder her
    um es zum Beispiel an ein anderes Jeedom zurückzusenden.

Unten haben Sie den Teil, auf den Sie Ihre Vorlage anwenden können
aktuelles Szenario.

Da von einem Jeedom zum anderen oder von einer Installation zur anderen,
Die Befehle können unterschiedlich sein, Jeedom fragt Sie die
Entsprechung von Aufträgen zwischen den beich der Erstellung Anwesenden
der Vorlage und die zu Hause anwesenden. Sie müssen nur die ausfüllen
Match Orders gelten dann.

Hinzufügung der PHP-Funktion
====================

> **IMPORTANT**
>
> Das Hinzufügen der PHP-Funktion ist fortgeschrittenen Benutzern vorbehalten. Der kleinste Fehler kann Ihr Jeedom zum Absturz bringen

## Einrichten

Gehen Sie zur Jeedom-Konfiguration, dann zu OS / DB und starten Sie den Datei-Editor.

Gehen Sie in den Datenordner und dann in PHP und klicken Sie auf die Dateich user.function.class.php.

In dieser Klasse müssen Sie Ihre Funktionen hinzufügen. Dort finden Sie ein Beispiel für eine Grundfunktion.

> **IMPORTANT**
>
> Wenn Sie ein Problem haben, können Sie jederzeit zur Originaldateich zurückkehren und den Inhalt von user.function.class.sample kopieren.PHP in user.function.class.php
