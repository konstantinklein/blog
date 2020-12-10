+++
title = "Malen nach Zahlen"
date = 2018-06-11T17:54:02+02:00
draft = false
tags = ["Technik"]
categories = ["Blog"]
cover = "/images/malen.jpg"
authors = ["kkl"]
+++
Feststellung des Tages: Auch nach ca. 20 Jahren des Bastelns im Netz lerne ich noch Grundsätzliches dazu. Bis zu meiner Begegnung mit dem [Minimo-Theme](https://minimo.netlify.com/), das diese Seiten so schön minimalistisch darstellt, war die Aufgabenstellung für einen Web-Browser aus meiner Sicht klar aufgeteilt:

- Für Struktur und Text einer Website ist HTML zuständig (wie auch immer es erzeugt wird, statisch oder dynamisch),
- das Layout und die Darstellung kontrolliert ein *cascading style sheet* (CSS) - oder auch mehrere,
- multimediale Inhalte, also Grafiken oder Audios oder Videos, werden von dem Ort, wo sie als Datei abgelegt sind, in die Seite eingebunden, und
- für das bisschen lokale Interaktivität ist meistens Javascript zuständig.

*Old school*. Ausgesprochen *old school*, muss ich zugeben.

Nehmen wir mal das Beispiel des netten kleinen Kalender-Icons direkt unter dem Titel dieses Textes, dort, wo das Veröffentlichungsdatum steht. In der WWWelt, wie ich sie bis vor kurzem kannte, ist dieses Icon als GIF-Datei in dem Verzeichnis mit den Bilderns abgelegt und wird wie folgt auf die Seite gepackt:

    <img src="/images/kalender.gif" />

Ins Deutsche übersetzt: Hier kommt ein Bild <code>img</code> hin, und du, Browser, findest es an folgender Stelle: <code>src</code>.

Nun sind die Zeiten, zu denen ich im Quellcode von fremden oder auch den eigenen Seiten herumschnüffelte, eigentlich vorbei. Aus gegebenem Anlass&trade; wollte ich aber wissen, wo Minimo die Icons abgelegt hat - und stellte fest, dass es überhaupt keine Icon-Grafiken gibt und das Kalender-Icon wie alle anderen Icons ganz anders aufgerufen wird:

    <svg class='icon' viewbox='0 0 25 24' stroke-linecap='round' stroke-linejoin='round' stroke-width='2' aria-hidden='true'>  
    <rect x="3" y="4" width="18" height="18" rx="2" ry="2"/>  
    <line x1="16" y1="2" x2="16" y2="6"/>  
    <line x1="8" y1="2" x2="8" y2="6"/>  
    <line x1="3" y1="10" x2="21" y2="10"/>  
    </svg>

Ei guck. Keine Grafikdatei, nirgends. Die ganzen Icons auf diesen Seiten sind keine GIFs, JPGs oder PNGs, sondern Vektorgrafiken: [SVG](https://de.wikipedia.org/wiki/Scalable_Vector_Graphics)s.

### Bildbeschreibung
Die Icons werden *als Text* vom Server ausgeliefert und erst vom Browser Ihres Vertrauens in eine Grafik umgerechnet und so dargestellt. Es wird also im HTML-Text eine Menge mehr Zeichen übertragen, dafür sparen wir uns eine (oder zwei, oder drei, oder viele) weitere Anfrage(n) an den Server, je nachdem, wieviele solche SVGs auf der Seite sind.

Dass es SVGs gibt, wusste ich schon lange; in meiner *old school*-WWWelt wusste ich nur nicht, wozu man sowas  im Alltag eigentlich brauchen kann. Jetzt weiß ich es: Weil z.B. bei einem Icon im Theme (kleiner Fehler) der rechte Rand etwas angefressen wirkte, ändere ich einen einzigen Zahlenwert, und das Icon ist komplett. Und weil ich alle Icons gerne im Rostrot meines Logos sehe, füge ich eine entsprechende Zeile in die .css-Datei ein - und schon sind alle Icons rostrot gestylt. Ui!

Und das ist nur der Anfang. SVG-Grafiken können z.B. aus den Ergebnissen eines Skripts errechnet werden: Webgrafiken, die es bis zum Moment der Darstellung noch gar nicht gegeben hat. Ui!! (Ja, ich weiß: Jede schnöde Balken- oder Tortengrafik im Netz könnte ein SVG sein, aber was habe ich schon mit Balken am Hut? Mit Torten schon eher...)

**Update:** OK, nach etwas Nachgucken auf anderen Seiten weiß ich jetzt, dass SVGs eben *nicht* nur für schnöde Balkengrafiken benutzt werden, sondern auch anderswo für grafische Seitenelemente. Da - z.B. in der Webausgabe von [Twitter](https://twitter.com), unter jedem einzelnen Tweet (aber nicht oben im Seitenkopf - da sind noch klassische Grafiken!) - gibt es auch reichlich SVG-Icons.

Egal, ich freu mich trotzdem über meine Entdeckung. Auch wenn ich inzwischen vermutlich der Einzige, weil Letzte bin.
