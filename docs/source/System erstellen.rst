System erstellen
================

Zum Erstellen eines Webhook-Systems, gehe unter den Einstellung zu *Allgemein* > *APIs* > *Webhook-Systems* > *Systeme*.
Dort ist am unteren Ende der Seite der Knopf zum Erstellen eines Systems.

Es öffnet sich ein Wizard, der Sie durch die Einrichtung begleitet.

Einrichtung
-----------

1) Schritt: Authentifizierungsmethode
   Wählen Sie hier, mit welcher Methode Sie den Benutzer an dem externen System authentifizieren.
   Möglich sind ``"none", "basic_auth", "api_key", "oauth_v2", "bearer_token"``.
   
2) Schritt: Authentifizierung einrichten
   Geben Sie auf dieser Seite an, welche Daten vom User erfragt werden müssen
   (Hinweis: einige Daten werden zu den jeweiligen Authentifizierungsmethoden schon abgefragt).
   Setzen Sie bei OAuth2 verbindungen auch die entsprechend weiteren Felder.
   Zuletzt geben Sie eine URL an, gegen die die Anmeldung getestet werden kann. Am besten eine URL, die keine weitere Konfiguration benötigt wie ``/me``.
   Zur Konfiguration, lesen Sie unter :ref:`URL Einstellung` weiter.

3) Schritt: Events
   Auf dieser Seite richten Sie die eigentlichen Prozesse oder Geschäftsvorfälle ein.
   Zum Anlegen eines neuen Events, klicken Sie auf den Knopf mit dem Plus-Symbol.
   
   In dem sich öffnenden Fenster geben Sie oben einen Namen und eine Beschreibung zu dem Event (Geschäftsvorfall) an. Darunter legen Sie fest,
   welche Daten der Benutzer übergeben muss. Danach geben Sie die URL an, an die die HTTP-Anfrage gehen soll.
   Schauen Sie für weitere Informationen unter :ref:`URL Einstellung`.
   Nachdem Sie diese Einstellungen gemacht haben klicken Sie auf ``Test`` daraufhin öffnet sich ein weiterer Wizard,
   in dem Sie die Authentifizierung, Beispieldaten und zuletzt den Event testen können.
   Dies sollten Sie auch machen, um die entsprechenden Rückgabewerte in dem Event zuweisen zu können.
   
4) Schritt: Weitere Einstellungen
   Geben Sie zuletzt einen Namen, Beschreibung, Logo, etc. für das neu erstellte System an.
   Haben Sie das gemacht, klicken Sie zum Speichern auf ``Fertigstellen``
   
   Im Anschluß können Sie das System in einer Aktion verwenden. Lesen Sie dazu mehr unter :doc:`Benutzung`



URL Einstellung
---------------

Die Einstellungen einer URL teilen sich auf in die HTTP-Methode ``GET, POST, PUT, DELETE, etc.``, die eigentliche URL und weitere Optionen.

Die HTTP-Methode ist bei REST-Schnittstellen mit der Funktion, die aufgerufen werden soll, gleich zu setzen.
Bei ``"GET"`` zum Beispiel sollen Daten aus dem Fremdsystem ausgelesen werden. Bei ``"POST"`` entsprechend geschrieben.
Lesen Sie dazu die Dokumentation des anzubindenden Fremdsystems.

Die URL selbst, an die die HTTP-Anfrage gesendet werden soll, tragen Sie in das dafür vorgesehene Text-Feld ein.

Weitere Einstellungen können Sie mit einem klick auf den Pfeil rechts neben den URL-Text-Feld finden.
Dort können Sie URL-Parameter, HTTP-Header oder den Request-Body einstellen. Hierfür steht ihnen aine Tabelle für Key-Value zuweisungen zur Verfügung.
Klicken Sie in der Tabelle unten rechts auf den Knopf mit dem Plus-Symbol, um einen weiteren Eintrag der aktuell ausgewählten Kategorie hinzuzufügen.
In dem linken Text-Feld geben Sie den Namen des Wertes an, so wie er vom Fremdsystem erwartet wird an.
Wenn zum Beispiel das Fremdsystem diesen Datensatz erwartet: ``{"name": "Max", "lastname": "Mustermann"}``, fügen Sie zwei Einträge der Tabelle hinzu und tragen Sie in den linken Text-Feldern jeweils ``name`` und ``lastname`` ein. Auf der rechten Seite können Sie eintsprechend ``Max`` und ``Mustermann`` eintragen.

