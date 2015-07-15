Stud.IP Video Conference Plugin
===============================

[![Build Status](https://travis-ci.org/virtUOS/studip-bigbluebutton.svg?branch=master)](https://travis-ci.org/virtUOS/studip-bigbluebutton)

Ein Stud.IP-Plugin um BigBlueButton aus einer Veranstaltung heraus starten zu k�nnen.
Teilnehmer/innen des Kurses k�nnen der Konferenz beitreten.

Einrichtung
-----------

Ist die Hochschule Mitglied der DFN und soll f�r das Plugin "Meetings" (Videokonferenzen)
Adobe Connect �ber die DFN genutzt werden, m�sste die Hochschule bei der DFN
per E-Mail (hotline@vc.dfn.de) anfragen, um eine Hochschul-Kennung zu erhalten.
Die DFN ben�tigt hierf�r eine spezielle Funktionsemailadresse und die IP-Adresse
des Stud.IP-Servers der Hochschule.

Konfiguration
-------------

Als Benutzer mit root-Berechtigung m�ssen in der Konfiguration die folgenden
Optionen konfiguriert werden:

Option            | Erkl�rung
----------------- | ------------------------------------------------------------------------------
`VC_DRIVER`       | zu verwendender Treiber (muss auf *dfnvc* oder *bigbluebutton* gesetzt werden)
`DFN_VC_URL`      | API-Endpoint des DFN (wird vom DFN mitgeteilt)
`DFN_VC_LOGIN`    | die Funktionsemailadresse
`DFN_VC_PASSWORD` | Passwort (wird vom DFN mitgeteilt)
`BBB_URL`         | API-Endpoint des BigBlueButton-Servers
`BBB_SALT`        | Passwort des API-Endpoints
