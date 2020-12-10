+++
title = "Abschreckendes Beispiel"
date = 2018-05-28T18:00:38+02:00
draft = false
tags = ["Blogging","Hugo","WordPress","MarkDown"]
categories = ["Blog"]
cover = "/images/hugofenster.jpg"
authors = ["kkl"]
+++
Nuja, was man eben so in Überschriften hineinschreibt, um Aufmerksamkeit zu erregen...

Eine Erfahrung, die ich schon auf der Suche nach einem Generator für statische (Blog-)Seiten und dann beim Einrichten dieser Seiten mit Hugo gemacht habe: Um nicht mit WordPress weiterzubloggen, muss  der Mensch  entweder ein Nerd oder bekloppt sein - oder, wie im vorliegenden Falle, beides.

Es hat ja Gründe, weshalb WordPress im Rennen der Blogsysteme mit weitem Abstand vorne liegt. Eine Installation mit einem Klick, eine Auswahl des Themes mit nicht viel mehr Klicks, und schon bloggt der Neuling froh vor sich hin. Dass WordPress durchaus nicht immer intuitiv ist und gerade bei der Verwaltung großer Mengen von Content und Seiten schwer zu wünschen übrig lässt, kriegt der bloggende Neuling erst später mit. Immerhin: Schreiben und Kommentare verwalten kann er ganz bequem von einem Browser-Fenster aus.

Hugo dagegen... Das Bild da oben zeigt, mit welchen (und wievielen!) unterschiedlichen offenen Fenstern der Mensch arbeiten muss, wenn er seine Hugoseite füttert. Heute sehen wir hier:

- den iA Writer mit Vorschaubild, in dem ich diesen Text gerade schreibe,
- die Windows-Kommandozeile, in der der Hugo-Vorschauserver läuft (und in der Hugo später den Befehl bekommt, die Änderungen auch tatsächlich in die entsprechenden Dateien zu schreiben),
- Firefox, in dem ich mir live angucken kann, wie sich meine Veränderungen auswirken werden, und schließlich, ganz versteckt im Hintergrund, weil gerade nicht gebraucht
- ein FTP-Programm, mit dem ich <del>den ganzen Schmonzes</del> die aktualisierten Seiten schließlich auf den Server hochlade.

Das muss man mögen - oder mit WordPress bloggen.

Dabei sehen wir hier nur, was nötig ist, ein zumindest vorläufig konfiguriertes Hugo-Blog zu betreuen. Darüber hinaus, dort, wo noch reichlich Bastelarbeit zu leisten ist, sind bei mir noch Fragen offen, die ich in den nächsten Tagen, Wochen und Monaten klären will. Freundliche Menschen, die mir in ihren Mails Hilfe anbieten, befinden sich in großer Gefahr, von mir Fragen gestellt zu bekommen...

#### Kommentare
Auch in dieser Nacht, um 1:33 Uhr, kam der erste Kommentar, den ich zwischen Dusche und Frühstück hier einbaue. Peter F. schreibt:

>> Nerd und/oder bekloppt

> am Anfang sicher... ;)

> Wenn du erst mal alles automatisiert hast, fragst dich wie das früher alles so kompliziert geschafft hast.

> Ich hab keine Ahnung womit man bei Windows 2018  automatisiert... ob man sich das überhaupt antut.

> Vor 1994 hab ich mit 4dos ziemlich viel gemacht, aber das ist m.W.n. mausetot.

> Powershell hab ich nicht so richtig mitbekommen, hab vorher meinen Windows-Hut an den Nagel gehängt.

Ehrlich gesagt: Die Powershell habe ich mir noch nicht näher angeguckt - und werde das evtl. auch gar nicht tun. Inzwischen laufen schließlich verschiedene Linices nativ unter Windows, und eigentlich hätte ich Hugo gar nicht in der Windows-Version installieren müssen, sondern gleich auf die "klassische Weise". Leider will ich diese Seiten eben nicht auf Github hosten (hatte ich auch schon mal getestet), sondern auf einem ganz normalen FTP-Server, und dazu muss ich sie in dem Verzeichnisgestrüpp, das Windows mit den Linux-Installationen anrichtet, erst einmal finden. Habe ich auf später verschoben. Weiter im Kommentartext...

>> Abschreckendes Beispiel

> kultiviert da etwa wer irrationale Angst vor der Kommandozeile? ;)

Klar, ey...

>> den iA Writer mit Vorschaubild, in dem ich diesen Text gerade schreibe,

> öhm. also ich bin in Linux unterwegs, seit 1994. ich schreib meist in Vim. Aber für SQL (Beruf...) hab ich mir den sublimetext gegönnt, und als ich mit Markdown angefangen hab, hab ich Remarkable benutzt.  
> https://remarkableapp.github.io/linux.html

> Den machst vollscreeen, links Markdown tippen, rechts wird das alles instant gerendert, mit allen von Github eingeführeten Zusätzen (github flavoured markdown).

Hier sind wir ganz tief im Becken der persönlichen Vorlieben unterwegs. Sublimetext habe ich ja auch auf dem Rechner, aber den iA Writer habe ich - ausgerechnet - seit meiner Zeit mit einem Android-Telefon, und weil es ihn ursprünglich schon für iOS und jetzt auch für Windows gibt, ist das eben mein Cross-Platform-Markdown-Editor.

Der Kommentar geht noch lange und technisch weiter, aber eine Frage will ich doch beantworten:

> Nutzt dein Hoster wirklich noch FTP??? Schau mal ob er in abnehmender Reihenfolge der Präferenz rsync/scp/sftp/ftps kann.

Nein, natürlich bietet selbst 1&1 inzwischen SFTP an. Sonst sieht es aber auf *shared hosting*-Accounts eher basic aus. Was sich da alles machen lässt, werde ich sicher in den nächsten Tagen und Wochen sehen. Und darüber berichten.
