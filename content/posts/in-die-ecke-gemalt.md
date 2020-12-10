+++
title = "In die Ecke gemalt"
date = 2019-01-27T13:39:52+01:00
draft = false
tags = ["Sicherheit","Datenschutz","Passwort","Passwort-Manager"]
categories = ["Blog"]
cover = "/images/ecke.jpg"
authors = ["kkl"]
+++
Im wirklichen Leben&trade; ist mir das natürlich noch nie passiert, dass ich mich mit einem Eimer Farbe selbst in einer Ecke festgemalt hätte - schon allein deshalb, weil ich als Wohnungsmieter die Ecken (s.o.) meist in fertigem Zustand übernehme. Im digitalen Leben dagegen *ist* es mir gerade erst jetzt passiert. Und das kam so...

Seit Anfang des Jahres bin ich mit meinem Hobby "[Sicherheit im Netz](../../tags/datenschutz/)" ja [nicht mehr ganz so allein](../es-tut-sich-was-tut-sich-was/), und Menschen fragen mich völlig freiwillig und von sich aus, was ich ihnen zu diesem Thema empfehlen kann. Dabei geht es aus gegebenem Anlass oft um das [Problem sicherer Passwörter](../beschaeftigung-aber-sicher/), und wie man sie sich merken kann. Die Lösung liegt auf der Hand bzw. im Netz: Passwort-Manager.

### Online...
Nun haben sich Anbieter wie [1Password](https://1password.com/) oder [LastPass](https://lastpass.com) nicht nur in meinen Augen eine saubere Reputation erarbeitet, was die Sicherheit der dort gespeicherten Login-Daten angeht. 1Password und LastPass bekommen die Daten selbst nur verschlüsselt zu sehen; die Entschlüsselung findet auf dem Gerät des Kunden statt. Und das Unbehagen, eigene Login-Daten einer Firma anzuvertrauen (igitt!), ist wirklich nur ein Unbehagen. Schließlich vertraut man ja auch sein Geld - wenn man denn welches hat - einer Firma an. Solche Firmen nennt man "Bank".

Trotzdem habe ich, langjähriger Kunde eines Online-Passwort-Managers, mich in der vergangenen Woche mal mit einer Lösung beschäftigt, bei der ich selbst den Grad an Absicherung bestimmen kann: [KeePass](https://keepass.info/). Und ich habe mich prompt in die Ecke gemalt (s.o.).

### ...und offline
KeePass ist ein *open source*-Passwort-Manager, der nichts anderes macht (und kann), als komplizierte Passwörter zu erzeugen und sicher zu speichern. KeePass legt die Daten in einer kleinen Datenbank ab, gesichert mit einem Passwort (*das* muss man sich allerdings merken, aber das ist bei den Online-Diensten ja auch nicht anders) und noch ein paar anderen Möglichkeiten, gerne auch zwei oder mehr gleichzeitig. Diese Datenbank legt der Mensch dann dort ab, wo er sie gut aufgehoben glaubt.

Und genau das ist das Problem. Am sichersten aufgehoben ist eine solche Datenbank... nein, nicht etwa auf dem heimischen Rechner, und schon gleich nicht auf dem Handy, das man in einem schwachen Moment auf'm Klo vergisst, sondern auf einem zusätzlich verschlüsselten USB-Stick, den man Tag und Nacht auf seinem Herzen trägt.

Macht natürlich niemand, das. Bringt ja auch nichts, denn um an die Daten in der Datenbank heranzukommen, braucht man ja doch wieder einen Rechner. Oder einen Ort in der Cloud *plus* einen Rechner...

Wie ich [an einem anderen Ort](https://www.dw.com/de/kommentar-das-märchen-vom-schutzlosen-user/a-46959302) schon geschrieben habe, kann man Daten selbstverständlich in der Cloud ablegen. Aber alles, was über Familien- und vor allem Katzenfotos hinausgeht, sollte bei allem sinnlosen Vertrauen in den Cloudanbieter verschlüsselt sein.

Nun bringt ein Passwort-Manager nicht viel, wenn er nicht überall dort zur Verfügung steht, wo man ihn braucht - also zuhause ebenso wie auf den angeblich so genannten mobilen Endgeräten. Also war meine Lösung: KeePass-Datenbank in die eine Cloud, Keyfile (die zweite Absicherung) in eine andere, beide Clouds natürlich verschlüsselt und zusätzlich mit 2FA gesichert, und das Passwort für beides zusammen in mein geplagtes Hirn.

Jo. Hätte ich auch lassen können. Denn der Sinn eines Passwort-Managers ist ja, immer auf dem neuesten Stand zu sein, wenn man z.B. [gerade sein Passwort geändert hat](../beschaeftigung-aber-sicher/). Das geht aber nur dann einigermaßen bequem, wenn der jeweilige Client auf PC oder Mobilquatsche auch ständigen Zugriff auf die Datenbank in der Cloud hat - den Zugriff, den ich mit der Verschlüsselung erfolgreich verhindert habe. Weshalb ich mit dieser  sehr weitgehend abgesicherten Lösung sichergestellt hatte, dass ich mit KeePass eigentlich nur an einem ausgewachsenen PC arbeiten kann; auf den Mobildingsen geht es nur nach Sprüngen durch drei Feuerreifen und dem Murmeln düsterer Beschwörungen. Also eigentlich gar nicht.

Das alte Problem: Sicherheit vs. Bequemlichkeit. Und irgendwo zwischen dem USB-Stick auf dem eigenen Herzen und dem Password-Speicher des eigenen Browsers (Hoppla! Über den haben wir noch gar nicht nachgedacht.) landen wir, die wir nicht alle Accounts mit "12345678" absichern wollen, letzendlich doch bei einem Passwortmanager im Netz.
