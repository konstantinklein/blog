+++
title = "Zeit für Crypto - drei Nachträge"
date = 2019-07-04T20:49:00+02:00
draft = false
tags = ["Crypto","Verschlüsselung","PGP","Messenger"]
categories = ["Blog"]
cover = "/images/secure.jpg"
authors = ["kkl"]
+++
Drei Ergänzungen zu [diesem Text](../zeit-fuer-crypto/), die ich nicht einfach an den Originaltext anhängen möchte, weil sie da niemand liest, der den Originaltext schon kennt.

**1. Probleme mit Firefox**

Da schreibe ich a.a.O. so schön, wie sich mit Mailvelope und GMX, Schritt für Schritt geführt, eine funktionierende PGP-Installation einrichten lässt. Und dann merke ich ein paar Tage später, dass - wenn im Firefox betrieben und aufgerufen - die Installation jedes Mal vergisst, dass es sie gibt, und sich nur durch die Eingabe des GMX-Wiederherstellungscodes wieder daran erinnern mag, wie man mit PGP und Mailvelope GMX-Mail ver- und entschlüsselt. Dieser Wiederherstellungscode ist 26 Zeichen lang, und man kann die wiederholte Eingabe dieser 26 Zeichen durchaus als zusätzliches Sicherheitsmerkmal betrachten. So ist es aber nicht gemeint, und bei der Verwendung eines anderen Browsers (Chrome, z.B.) tritt die Vergesslichkeit auch nicht auf.

Ich habe bei den Machern von Mailvelope Alarm geschlagen, ~~aber noch keine Antwort bekommen~~ aber Thomas Oberndörfer, der Mann hinter Mailvelope, hat mich höflich darauf hingewiesen, dass er nicht wisse, was mit der GMX-Integration in Firefox klemmen könnte, und mich an GMX verwiesen (wahrscheinlich, weil nicht er die Integration entwickelt hat, sondern GMX).

~~Und vielleicht braucht es die auch gar nicht, denn das Verhalten ist ganz neu, ungefähr so neu wie die Firefox-Version vor der aktuellen, [mit der Add-ons schon anderweitig Schwierigkeiten hatten](https://support.mozilla.org/en-US/kb/add-ons-disabled-or-fail-to-install-firefox). Da am 9. Juli, also nächste Woche, Version 68 des Browsers erscheinen soll, halte ich einstweilen meine Füße still - und gebe bei Bedarf eben die 26-Zeichen-Kette *nochmal* ein, die ich inzwischen fast auswendig kann.~~ Inzwischen weiß ich, dass auch die 68er-Version von Firefox das gleiche Verhalten zeigt. Und jetzt grübelt der Support von GMX darüber nach. *Stay tuned!*

**2. Mobil und trotzdem verschlüsselt**

Was ich beim Schreiben des [Originalposts](../zeit-fuer-crypto/) völlig übersehen hatte:  Ich schreibe meine Einträge in dieses Blog an einem Desktop-PC und denke dann auch vor allem über Leben und Arbeiten mit einem PC nach. Deshalb ist alles, was ich [hier](../zeit-fuer-crypto/) geschrieben habe, auch nur an einem PC oder einem Mac zu machen.

Nun sagen mir aber die, die's wissen müssen (oder zumindest von sich behaupten, dass sie's wüssten), dass der Mensch von heute zunehmend bis überwiegend mit seinem Mobilgerät ~~herummacht~~ interagiert. Und da geht der ganze Krypto-Kram entweder gar nicht oder doch sehr anders.

iOS-Geräte sind zwar durchaus in der Lage, ihre Daten intern verschlüsselt zu speichern; mit dem Krypto-Standard PGP und all seinen Varianten kann jedoch (fast) keine iOS-App etwas anfangen. In der Welt der Androiden ist es nur unwesentlich besser; dort gibt es zwar PGP-taugliche Mail-Apps, aber keine davon ist standardmäßig vorinstalliert, und die Bedienungsfreundlichkeit ist, sagen wir: sehr mäßig.

Und da kommt schon wieder der Anbieter GMX ins Spiel, der - entgegen seinem Ruf - in dieser Hinsicht inzwischen einiges ganz richtig macht. Die GMX-Mail-App für Android wie für iOS mag zwar längst nicht so cool aussehen wie die GMail-App oder die von Apple, aber dafür kommt sie tatsächlich mit eingebauter, funktionierender und leicht bedienbarer Verschlüsselung daher. Dafür macht GMX aus mir nicht verständlichen Gründen kaum Werbung (sie werden es doch nicht etwa aus Kostengründen wieder abschaffen wollen?), aber für an verschlüsselter Mail interessierte Nutzer ist das ein Hammerargument. Entschuldigen Sie den unangemessenen Begeisterungsausbruch.

**3. Und eine Lektüreempfehlung**

Im Zusammenhang mit [dem Text über Kryptografie](../zeit-fuer-crypto/) ist mir auch wieder eingefallen, wie ich so um den Jahrtausendwechsel herum selbst angefangen habe, mit Verschlüsselung zu experimentieren. Damals gab es noch keine Browser-Erweiterungen, die sowas einfacher machten, und keine Mailanbieter, die einem das ganze nahezubringen versuchten. Und mir fiel das Buch ein, das 2001 erschien und beschrieb, "wie die Code-Rebellen die Regierung besiegten und die Privatsphäre im Digitalen Zeitalter retteten": ["Crypto" von Steven Levy](https://amzn.to/2RT8V6P) (Amazon-Link), das es jetzt netterweise immer noch gibt. Das Buch hat inzwischen etwas anheimelnd Altmodisches an sich; [NSA](https://de.wikipedia.org/wiki/National_Security_Agency) & Co. kommen zwar als düstere Schlapphüte vor, die die aufrechten Krypto-Helden zu schlagen hatten, aber von den Erkenntnissen der [Snowden](https://de.wikipedia.org/wiki/Edward_Snowden)- und Nach-Snowden-Ära war und ist darin natürlich nichts enthalten. Trotzdem: Ich habe mich erinnert, dass ich aus diesem Buch, das sich eigentlich nicht mit Kryptografie, sondern mit ihren Pionieren beschäftigt, eine Menge gelernt hatte. Und möchte es deshalb, so verstaubt es inzwischen ist, Interessierten ans Herz legen.
