+++
title = "Zeit für Crypto!"
date = 2019-06-11T21:34:31+02:00
draft = false
tags = ["Crypto","Verschlüsselung","PGP","Messenger"]
categories = ["Blog"]
cover = "/images/secure.jpg"
authors = ["kkl"]
+++
Oh Mann! Der Minister des Inneren, für Bau und Heimat will also, dass Anbieter von Messenger-Diensten auf Zuruf die Inhalte von verschickten Nachrichten [im Klartext an staatliche Stellen übergeben](https://www.heise.de/newsticker/meldung/Angriff-auf-WhatsApp-Co-Seehofer-will-Messenger-zur-Entschluesselung-zwingen-4431634.html) - ein Vorschlag, der derzeit ohne den Komplettumbau der betroffenen Messenger und ihrer Geschäftsmodelle nicht umsetzbar ist (uff!) und trotzdem, gelinde gesagt, [auf Kritik stößt](https://www.spiegel.de/netzwelt/netzpolitik/whatsapp-und-co-warum-messenger-in-deutschland-nicht-entschluesselt-werden-duerfen-a-1269196.html) und schließlich dazu führen wird, dass [der Minister Post bekommt](https://docs.google.com/document/d/17F-OxKJtR8DM9O8jiEfUhxDGguBnJoZ2-lvp9614CyM/edit).

Nun wäre das nicht der erste Vorschlag aus dem Hause Seehofer, der irgendwann im Nirwana versackt (oder was Vorschläge im Nirwana eben so tun), und die Argumente sprechen ja wirklich gegen ihn (den Vorschlag, aber auch den Minister). Trotzdem komme ich ins Grübeln - schließlich verlassen wir uns beim Gebrauch [sicherer Messenger](../die-messenger-tabelle/) nahezu blind darauf, dass seit dem letzten Audit keine *backdoor* eingebaut wurde. Bleibt den meisten von uns ja auch nichts anderes übrig.

### Selbst ist der Verschlüssler

...und seine Gefährtin, die Verschlüsslerin, natürlich auch. Und deshalb - und weil die Suchbegriffe PGP und Verschlüsselung in der letzten Zeit wieder öfter in den Logs dieser Seiten auftauchen - weise ich im Jahr 2019 mal wieder darauf hin, dass es neben der fertig montierten und deshalb gerne genutzten sicheren Kommunikation via Messenger auch noch die gute (wenn man von der *usability* absieht) alte Verschlüsselung nach dem PGP-Prinzip gibt. Was sich aber seit meinem letzten Versuch, Sie dafür zumindest zu interessieren, geändert hat: Inzwischen gibt es Anbieter, die einem die Einrichtung und den Gebrauch von PGP-Verschlüsselung im Mailverkehr zumindest etwas leichter machen. Darum soll es in diesem Text gehen.

### Grundwissen, so kurz wie möglich

Sorry, daran führt kein Weg vorbei. Für die Ver- und Entschlüsselung von Daten nach dem [OpenPGP](https://de.wikipedia.org/wiki/OpenPGP)-Prinzip braucht der Mensch zwei so genannte Schlüssel, die zusammengehören. Das sind Textdateien, die so aussehen wie die [auf dieser Seite](../../pages/pgp-key). Der eine Schlüssel ist privat und **darf keinem Unbefugten in die Pfoten fallen**. Der andere ist öffentlich, und jeder **darf, soll und muss ihn sehen und kopieren** können. PGP-Verschlüsselung funktioniert nun so, dass das PGP-Programm den Inhalt der Nachricht mit dem öffentlichen Schlüssel des Empfängers (und dem des Absenders, damit der die Nachricht später nochmal lesen kann) verschlüsselt. Der so verschlüsselte Inhalt kann aber mit dem gleichen (öffentlichen) Schlüssel nicht mehr entschlüsselt werden (weshalb auch völlig egal ist, wer diesen Schlüssel hat), sondern *nur mit dem privaten Schlüssel* des Empfängers (bzw. Absenders) und der dazugehörigen Passphrase. Warum das so ist, darüber kann man viele dicke Bücher lesen. Muss man aber nicht.

Wer also seine Mail mit PGP verschlüsseln will, braucht mindestens drei Schlüssel in seinem Schlüsselbund (das heißt wirklich so): das eigene Schlüsselpaar aus öffentlichem und privatem Schlüssel sowie den öffentlichen Schlüssel des Empfängers der Nachricht. Diese Schlüssel werden von der PGP-Anwendung auf dem eigenen Rechner (oder dem eigenen Mobilgerät) verwaltet. Wenn man sie erst mal hat, muss man sich darum nicht mehr kümmern.

### Puhhh...

Ja, das ist kompliziert. Und der User kann sich die Einrichtung auch beliebig kompliziert machen - muss aber nicht sein. Die sicherste Lösung ist natürlich eine handgeklöppelte PGP-Installation nach Großmutter-Art. Aber gerade für Webmail (GMail, Yahoo!, GMX, T-Online, web.de, *you name it*) gibt es inzwischen eine Reihe von Lösungen, die einen annehmbaren Kompromiss zwischen Komfort und Sicherheit darstellen - und einem die Ersteinrichtung so schmerzfrei wie möglich machen. Um diese Lösungen geht es hier und heute.

Für die allermeisten Webmail-Anbieter gibt es für die Browser Chrome und Firefox das Add-on [Mailvelope](https://www.mailvelope.com/de). Das setzt PGP mit JavaScript im Browser um, was Puristen aufjaulen lässt. Aber hier geht es um den schon angesprochenen Kompromiss zwischen Komfort und Sicherheit, und Mailvelope wird von denen, die es wissen sollten, bei allem Komfort auf der sicheren Seite angesiedelt.

Anbieter wie [posteo](https://posteo.de), aber auch (ausgerechnet!) die in dieser Hinsicht gerne unterschätzten Mailbetriebe [GMX](https://gmx.net) und [web.de](https://web.de) arbeiten mit Mailvelope zusammen und haben Wege entwickelt, mit denen die Installation von Mailvelope, die Einrichtung des eigenen Schlüsselbundes und die Veröffentlichung des eigenen öffentlichen Schlüssels zum gefälligen Gebrauch durch andere so einfach wie möglich gemacht werden. Der Neuling wird an die Hand genommen, und am Ende von etwa zehn Minuten Klicken und Tippen steht eine funktionsfähige PGP-Installation. Die mobilen Mailclients von GMX für iOS und Android können übrigens auch ver- und entschlüsseln - etwas, das in der Welt des mobilen Mailens durchaus nicht selbstverständlich und oft nur sehr schwierig umzusetzen ist.

[mailbox.org](https://mailbox.org), der andere unter den Berliner Kleinanbietern mit besonderem Fokus auf Sicherheit, bietet zusätzlich einen zweiten Weg zu PGP-Mail an. mailbox.org-Kunden können einerseits ebenfalls Mailvelope nutzen (wie die Kunden *aller* Webmail-Angebote, die nur auf den Komfort bei der Einrichtung verzichten müssen, den die bisher Genannten anbieten), andererseits auch den sogenannten "Guard"; dabei wird das Schlüsselpaar ebenfalls im heimischen Browser erzeugt, dann aber crypto-gesichert auf den Servern von mailbox.org gespeichert. Hier jaulen die Puristen noch lauter, denn aus der angestrebten *end-to-end*-Verschlüsselung wird auf diese Weise eine, die schon bei mailbox.org endet. Mit diesem Nachteil erkauft man sich jedoch den Vorteil, verschlüsselte Mail in *jedem* Browser lesen zu können, nicht nur in dem auf der eigenen Maschine mit der eigenen Mailvelope-Installation. Das Argument der mailbox.org-Leute für den Gebrauch eines privaten Schlüssels auf ihrem Server ist übrigens, dass sie auf ihre Server wahrscheinlich besser aufpassen als unerfahrene Nutzer auf ihren PC oder ihr Handy. Daran könnte sogar was sein...

### Und nu?

Ist erst einmal alles eingerichtet, braucht der Mensch den öffentlichen Schlüssel eines jeden Mailpartners, mit dem er verschlüsselt mailen will. An diese öffentlichen Schlüssel kommt man ran, wenn sie [wie meiner](../../pages/pgp-key) auf einer Website gepostet sind. Natürlich kann man sie sich vorab auch einfach per Mail zuschicken - es ist ja nur Text. Die Lösungen von posteo, mailbox.org, GMX und web.de legen die öffentlichen Schlüssel ihrer Nutzer aber auf Wunsch auch auf Schlüsselservern ab, wobei die von posteo und mailbox.org öffentlich zugänglich sind. Mailt man also jemand an, von dem man selbst den Schlüssel nicht hat, kann es sein, dass der Anbieter über einen Schlüsselserver erfährt, dass es für den Empfänger einen Schlüssel gibt, und sich von selbst mit dem Angebot meldet, den Schlüssel zu importieren. Mailvelope selbst betreibt auch [einen öffentlich zugänglichen Schlüsselserver](https://keys.mailvelope.com/).

Wenn man dann erst den öffentlichen Schlüssel des Partners in seinen Schlüsselbund importiert hat, lässt sich auf Mausklick verschlüsselt mailen. Hurra!

### Sonderfall GMail

GMail-Nutzer können natürlich auch Mailvelope benutzen. Für sie gibt es aber einen weiteren Verschlüsselungsanbieter: [FlowCrypt](https://flowcrypt.com/) dessen Addon (ebenfalls für Chrome und Firefox) sich nicht, wie Mailvelope, über die Weboberfläche legt, sondern sich in die Maschinerie der GMail-Oberfläche einnistet (und deshalb auch mehr Rechte verlangt als Mailvelope). Was das Addon da treibt, kann ich nicht sagen; bei einem kurzen Probelauf habe ich aber festgestellt, dass FlowCrypt den Prozess von Einrichtung und Schlüsselverwaltung *noch einen Tick einfacher* macht als die Lösungen von posteo, GMX und web.de.

**Nachtrag:** Es gibt eine [ausführliche Kritik von FlowCrypt](https://prgomez.com/flowcrypt-review/) von PR Gomez (danke an Stammleser Peter für den Hinweis!).

### Ohgottohgott!

Ja. Das ist bei aller Vereinfachung immer noch scheißkompliziert. Ich habe deshalb die Leser dieser Seiten in den letzten Jahren mit dem Thema verschont - bis heute. Denn vielleicht ist es doch nicht so schlecht, über Verschlüsselung Bescheid zu wissen und ein wenig Erfahrung damit gesammelt zu haben für den Tag, an dem man seinem Messenger nicht mehr so richtig trauen will.

Noch ein Wort für die Fachleute da draußen: Ja, ich habe das eine oder andere in diesem Text einfacher dargestellt, als es ist. Damit das Thema zugänglich bleibt und nicht alle bei "Drei!" schreiend auf die Bäume klettern.

**Nachtrag:** Mir sind noch ein paar zusätzliche Absätze eingefallen, die [ich hier aufgeschrieben](../zeit-fuer-crypto-drei-nachtraege/) habe.
