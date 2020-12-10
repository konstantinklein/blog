+++
title = "Im Bastelkeller"
date = 2020-04-23T22:58:26+02:00
draft = false
tags = ["Hugo","Blog","WordPress"]
categories = ["Blog"]
cover = "/images/brahehus.jpg"
authors = ["kkl"]
+++
Es ist wie früher. Wenn der Mensch nicht (genug) zu tun hat, begibt er sich in den Bastelkeller und ~~schreibt~~ schraubt an seinem Blog herum.

Seinen Ausgangspunkt hatte das Drama [vor einigen Tagen](../baustelle-oder-nicht), als ich anfing, über WordPress im Allgemeinen und dieses kleine Blog im Besonderen nachzudenken. Das Ergebnis sehen Sie hier - vielleicht nicht allzu lange, weil ich vielleicht doch noch einen dicken Fehler finde und schnell wieder auf die alte Version umstellen muss. Was ja mit statischen Seiten wie den von Hugo erzeugten nicht schwer ist - man muss sie nur in einem anderen Verzeichnis ablegen, und da sind sie schon.

Dies ist also weiterhin ein Hugoblog, aber mit neuem Anstrich. Den habe ich mir zusammen mit der aktuellen Ausgabe der Engine heruntergeladen, und was bei WordPress (schon irgendwie verdächtig, dass ich immer wieder drauf zurückkomme, wa?) eine Sache von zwei, drei Mausklicks ist, dauert selbst bei einem Theme, das schon einen sehr ~~fertigen~~ ausgereiften Eindruck macht, Stunden.

### Stunden? Stunden.
Zum einen verwendet das Theme mit dem wunderschön umständlichen Namen [Hugo Future Imperfect Slim](https://themes.gohugo.io/hugo-future-imperfect-slim/) ~~reichlich Google-Fonts, was zwar schick aussieht, aber mit meinem Anspruch, möglichst keine (Nutzer-) Daten nach Google zu schicken, nicht zusammenpasst. Ich habe also versucht, alle Fonts durch allgemein und vor allem auf jedem Endgerät verfügbare zu ersetzen. Das ist mir wahrscheinlich noch nicht durchgehend gelungen, und ich werde noch tagelang in den CSS-Dateien herumfuhrwerken müssen~~ Fonts, die auf den meisten Endgeräten nicht zum Standardangebot zählen dürften. Wie aus den durchgestrichenen Zeilen immer noch deutlich genug hervorgehen dürfte, werden diese Fonts vom Theme per default von Google geladen - was ich nicht gut fand und sie deshalb durch Standardfonts ersetzte. Ein Tipp von [Ralf G. aus K.](https://uninform.at) ließ mich dann wissen:

{{< mastodon status="https://mastodon.social/@leralle/104052503507006895" width="700" height="345">}}

...und mit der Hilfe der verlinkten App [google-webfonts-helper](https://google-webfonts-helper.herokuapp.com/fonts) habe ich das jetzt umgesetzt. Falls es da noch Fehlermeldungen gibt... [Kontakt](../../pages/kontakt) - dankeschön.

Darüber hinaus sollte die Seite schon ein bisschen angepasst werden, auch an die Seitenstruktur, wie sie hier bisher herrschte - nichts aufregendes, aber ich wollte die bisherigen Einträge schon alle dort wiederfinden, wo ich sie suche.

Und als ich schon fast fertig war (oder mir das einbildete), fiel mir auf, dass ich vor zwei Jahren, beim Umstieg auf Hugo, schon einmal lange gebastelt hatte, um aus dem Hugo-eigenen RSS-Feed, der nur Titel und die ersten paar Worte ausgibt, wieder einen Volltext-Feed zu machen. Der erste Versuch, Funktionen aus dem alten Hugo-Setup von 2018 zu kopieren (etwas, das bei der einen oder anderen im Theme nicht enthaltenen Funktion schon geklappt hatte), ging gründlich schief und endete in einem Haufen von Fehlermeldungen. (Hatte das einfach keiner meiner alten Hugo-Version gesagt, oder warum gab es da keine Probleme?)

Der zweite Versuch bestand darin, das zu kopieren, was auch andere mit dem gleichen Problem schon gemacht und netterweise in diversen Hugo-Foren gepostet hatten. Aber auch das klappte irnzwie nicht: Es gab einen Feed, aber keine Inhalte.

### Hugo im Nebel
Weil, wie ich [dann hier herausfand](https://randomgeekery.org/2017/09/15/full-content-hugo-feeds/), neuere Hugo-Versionen eine andere interne Dateistruktur verwenden (an der "sichtbaren" Dateistruktur hatte sich nichts geändert...) und deshalb beim Feedbauen in den Nebel glotzen.

Wie war das nochmal mit *"Never touch a running system"*?

Zu spät. Das System ist betatscht und jetzt erstmal live. Die Hugo-Installation dahinter ist neu und längst nicht mehr so ungeordnet wie das, was ich mir vor zwei Jahren mit *learning by doing* zusammengebaut hatte. Und wenn ich in den nächsten Tagen doch noch Fehler der *dealbreaker*-Klasse finde, sehen diese Seiten ganz rasch wieder aus wie am letzten Montag. *Stay tuned.*
