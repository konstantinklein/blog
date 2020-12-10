+++
title = "Sie geben nicht auf"
date = 2018-09-28T08:58:59+02:00
draft = false
tags = ["Werkzeug","Datenschutz"]
categories = ["Blog"]
cover = "/images/secure.jpg"
authors = ["kkl"]
+++
Es liegt wohl daran, dass sie Beamte und/oder sonstige Staatsbedienstete sind, die schließlich dafür bezahlt werden, ~~Dinge zu tun, deren Sinn sich nicht sofort erschließt~~ nicht aufzugeben. Jedenfalls fand ich im (durchaus empfehlenswerten) [Bürger-CERT-Newsletter](https://www.bsi-fuer-buerger.de/BSIFB/DE/Service/Buerger-CERT/Sicher-informiert/Newsletter.html) des [Bundesamtes für Sicherheit in der Informationstechnik](https://bsi.bund.de) diese Woche den Hinweis auf [diesen Artikel](https://www.bsi-fuer-buerger.de/BSIFB/DE/Service/Aktuell/Informationen/Artikel/einfache_email_verschluesselung.html) mit der Jubel-Überschrift:

> Gewusst wie: E-Mail-Verschlüsselung endlich einfach

"Endlich einfach", so, so.

Damit wir uns nicht falsch verstehen: Eine Vereinfachung (oder mehrere) ist, was PGP-Verschlüsselung im Mailverkehr am aller-aller-allerdringendsten braucht. Das ganze Gewese und Gemache mit öffentlichem und privatem Schlüssel, mit dem Austausch des öffentlichen Schlüssels beider Partner, bevor die Verschlüsselung überhaupt losgehen kann, mit der Verwaltung von Schlüsselringen und Schlüsselwiderrufen... was auch immer es ist, *einfach* ist es nicht.

### Vielfältige Versuche
Entsprechend vielfältig sind die Versuche, mit denen Entwickler und private Anbieter wie [GMX](https://gmx.net), [Web.de](https://web.de) und [mailbox.org](https://mailbox.org) die Einrichtung der Verschlüsselung, die Erstellung der Schlüssel und die Verteilung zumindest über hausinterne Schlüsselserver automatisiert haben - bis hin zu dem Stadium, in dem alles so automatisiert ist, dass der Nutzer keine Chance hat, irgendwas zu unternehmen, wenn etwas schief läuft.

Daran versucht sich jetzt auch das [BSI-Projekt: "EasyGPG" - E-Mail Verschlüsselung vereinfacht](https://www.bsi-fuer-buerger.de/DE/Themen/Kryptografie_Kryptotechnologie/Kryptografie/EasyGPG/EasyGPG_node.html). Und das soll so gehen:

> 1. Private und öffentliche Schlüssel werden automatisch erzeugt.
> 2. Öffentliche Schlüssel werden automatisch verteilt.
> 3. Nachrichten werden per Voreinstellung verschlüsselt und signiert.
> 4. Veröffentlichung und Bereitstellung der Software.

Fein. Doch, ich begrüße das auf das allerschärfste&trade;. Ich freue mich sogar, dass meine *tax Euros at work* für sowas eingesetzt werden.

### Aber...
Aber ich fürchte, es wird nichts nützen. Denn einerseits interessiert sich nur ein schandhaft geringer Teil der Netzbevölkerung in meiner Umgebung überhaupt dafür, seine Mails sicherer zu machen. Nur 0,2 Prozent der Menschen in meinem Addressbuch haben einen PGP-Schlüssel (und da reden wir noch nicht von der tatsächlichen Nutzung), weit entfernt von den 13 Prozent der Deutschen, die angeben (in jedem Sinne des Wortes), Mailverschlüsselung zu nutzen.

Andererseits nützen die mir Wichtigsten im Netz durchaus verschlüsselte Kommunikationswege. Sie heißen Messenger, und mein liebster heißt [Signal](https://signal.org). Seit diese Messenger mehr können als nur kurze Textnachrichten, seit sie auch Fotos und Dokumente verschlüsseln und transportieren, sehen die Menschen in meiner Umgebung noch viel weniger die Notwendigkeit für Mail-Verschlüsselung.

### Nachtrag: Schuss in den Ofen
Am Einheiztag (3. Oktober, Tag, an dem ich die Heizperiode 18/19 eröffnet habe, aber das gehört nicht hierher) berichtet heise Security, wie ein *anderer* Versuch, PGP leichter nutzbar zu machen, grandios in die Hose geht: [c't deckt auf: Enigmail verschickt Krypto-Mails im Klartext](https://www.heise.de/security/meldung/c-t-deckt-auf-Enigmail-verschickt-Krypto-Mails-im-Klartext-4180405.html). Betrifft die aktuelle Enigmail-Version für Windows im sog. *Junior Mode*, also dem, der PGP endlich einfach machen soll; Mac- und Linux-User haben das Problem offenbar nicht.
