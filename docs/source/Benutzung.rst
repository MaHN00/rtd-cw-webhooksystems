Benutzung
=====

.. _Schnellstart:

Schnellstart
------------

Um das Webhook-System verwenden zu können benötigen sie folgende Rechte:

.. code-block:: console

   webhook_system

Erstellen einer Webhook-Aktion
------------------------------

Ziehen Sie zum Erstellen einer Webhookaktion das Symbol aus der
Aktionsleiste in den Kampagnenmanager in eine Kampagne.
Danach öffnet sich das Setup-Dialog, in dem Sie die Einstellungen für die Webhook-Aktion hinterlegen.
Zuerst wählen Sie das System, von dem oder zu dem Sie eine Anfrage senden wollen.
Klicken Sie dazu einfach auf dem Logo des Systems auf `wählen`.

Danach erscheint eine Auswahlbox für die Anmeldedaten. Sollten Sie schon Anmeldedaten
zu dem System hinterlegt haben, können Sie diese an dieser Stelle auswählen. Sollten
noch keine Anmeldedaten hinterlegt sein, wird nur `Bitte wählen` angeboten.
In diesem Fall klicken Sie auf den Pfeil rechts neben der Auswahlbox um Anmeldedaten
für dieses System zu hinterlegen. Mehr dazu unter :doc:`Anlegen von Anmeldedaten`

Nachdem die Anmeldedaten gewählt oder angelegt sind, wählen Sie den eigentlichen Event,
der im anderen System stattfinden soll. Zum Beispiel `Kontakt erstellen` oder `Rechnung erstellen`.

Zu dem gewählten Event, muss nun noch gegebenenfalls Angegeben werden,
welche Daten des Kontaktes gesendet werden sollen. Dazu einfach das Feld aus der
Auswahlbox wählen zum dem Punkt, zu dem es gesendet werden soll.

Darauf hin kann mit einem Klick auf den `Test`-Knopf die bisherige Einstellung
getestet werden. Darunter ist gegebenenfalls die Zuweisung für die Daten, die von dem externen
System zurück kommen. So können diese innerhalb des Kontaktes gespeichert werden.

Nach dieser Einstellung ist es noch möglich zu der Aktion Bedingungen anzugeben
und zuletzt noch zu speichern.



Anlegen von Anmeldedaten
------------------------

Anlegen von Anmeldedaten ist sehr Einfach. Sie werden nur nach den entsprechenden Daten gefragt
und im Anschluss noch nach einem Namen, unter dem Sie diese Daten hinterher auswählen können.
Während des Anlegens der Daten besteht die Möglichkeit diese zu Testen,
auch mit einem Klick auf den `Test`-Knopf. Dies ist auch benötigt, um weiter gehen zu können.
