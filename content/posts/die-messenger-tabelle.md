+++
title = "Die Messenger-Tabelle"
date = 2018-06-09T10:47:15+02:00
draft = false
tags = ["Werkzeug","Datenschutz","Messenger"]
categories = ["Blog"]
cover = "/images/secure.jpg"
authors = ["kkl"]
+++
Aus gegebenem Anlass&trade; habe ich eine Übersicht aktueller Messenger (lies: *nicht* [AIM](http://www.dailymail.co.uk/sciencetech/article-5183887/The-end-internet-era-AOL-kills-AIM.html), [ICQ](http://www.spiegel.de/netzwelt/web/icq-messenger-dienst-is-wieder-da-a-1083839.html), [Yahoo! Messenger](https://thenextweb.com/apps/2018/06/08/yahoo-messenger-dead-squirrel/) und andere Todeskandidaten) zusammengestellt - vor allem unter den Gesichtspunkten Verschlüsselung und Datenschutz. Alle aufgeführten Messenger bieten *end-to-end*-Verschlüsselung an; der Telegram-Messenger allerdings nur optional und auf der Basis von einzelnen Chats.

Dies ist, wenn man so will, eine Fortsetzung der Mail-Tabelle, in der ich in einer früheren Ausgabe meines Blogs verschiedene Mailanbieter, ebenfalls unter den o.a. Gesichtspunkten, zusammengefasst habe. Gleichzeitig ist es aber *keine* Fortsetzung der Mail-Tabelle. Der grundsätzliche Unterschied: E-Mail bzw. die darunter liegenden Standards sind ein universelles Protokoll, und auch wenn ich einen *top secure*-Mailanbieter wähle, kann ich immer noch mit Tante.Adelheid@mail.ru mailen. In der Welt der Messenger müssen sich beide Seiten, Tante Adelheid und ich, für den gleichen Messenger entscheiden - was es in einer WhatsApp-dominierten Welt schwierig macht, einen *wirklich* sicheren Messenger zu nutzen.

Hier also die Tabelle (Stand: 21.07.2020 - Fehler bitte [per Mail an mich](../../pages/kontakt)):

|Produkt, Anbieter|ID|Krypto|Datenschutz|Sonstiges|
|---|---|---|---|---|
|[WhatsApp](https://whatsapp.com), Facebook</td>|Tel-Nr.|end-to-end|Zugriff auf Kontakte, lädt Kontakte hoch|Austausch mit Facebook unklar|
|[Signal](https://signal.org), Open Whisper Systems|Tel-Nr.|end-to-end, [PFS](https://de.wikipedia.org/wiki/Perfect_Forward_Secrecy), [Abstreitbarkeit](https://de.wikipedia.org/wiki/Glaubhafte_Abstreitbarkeit), indiv. Authentifizierung|Zugriff auf Kontakte optional, sollte unterbunden werden|von Edward Snowden empfohlen&trade;|
|[Telegram](https://telegram.org)|Tel-Nr.|end-to-end, muss pro Chat aktiviert werden|Zugriff auf Kontakte sollte unterbunden werden|Klartext-Inhalte dauerhaft beim Anbieter gespeichert|
|[Threema](https://threema.ch/de/)|Threema-ID|end-to-end, PFS, indiv. Authentifizierung|[keine Probleme bekannt]|Clients kostenpflichtig|
|[Wire](https://wire.com/de/)|Wire-ID, Mail-Adresse|end-to-end|[keine Probleme bekannt]|
|[Hoccer](https://hoccer.com)|Hoccer-ID|end-to-end|[keine Probleme bekannt]|geringe Nutzerbasis?|
|[ginlo](https://www.ginlo.net/de/)|ginlo-ID, Tel-Nr|end-to-end|sollte Ende 2019 eingestellt werden, wird von einem der Gründer vorerst weiterbetrieben|unsichere Zukunft?|

Aus Datenschutz- wie aus Gesichtspunkten der Nutzerfreundlichkeit ist die verwendete ID unterschiedlich problematisch. Wird die Telefonnummer (keine frei gewählte ID, sondern vom Provider vergeben und dort abfragbar!) als ID verwendet und dem Betreiber mitgeteilt, kann dieser jeden User, der ihm das Hochladen des eigenen Adressbuches gestattet, wissen lassen, dass man selbst auch Benutzer des jeweiligen Produktes ist. Gleiches gilt für Mail-Adressen in Kombination mit dem Hochladen von Adressbüchern.

Wer dagegen das Hochladen sämtlicher Kontakte verweigert (was man nach der DSGVO machen sollte, wenn man nicht alle Kontakte um Erlaubnis fragen will), muss jeden einzelnen Menschen in seiner digitalen Umgebung fragen, welchen Messenger er oder sie unter welcher ID benutzt. Umständlich, aber datensauber.

Ich bin über folgende Messenger erreichbar:

- Signal (ID: meine Tel.-Nr., ätsch)
- ginlo  (ID: 62XN5BZP)
- Threema (ID: [JCVUCNWU](https://threema.id/JCVUCNWU))

WhatsApp ist, wie alle anderen Facebook-Produkte, aus meiner digitalen Welt verbannt. Und Hoccer... Also ich kenne niemand, der das nutzt.

#### Kommentare
Nur eine Stunde nach der Veröffentlichung dieses Textes meldet sich der stetige Kommentierer Peter und weist auf [Confide](https://getconfide.com) hin, den Lieblingsmessenger der US-Republikaner (wahrscheinlich, weil für sie, Angehörige der *Generation Mission Impossible*, Nachrichten, die sich nach dem Lesen selbst zerstören, das Höchste der Verschlüsselungsgefühle sind) - aber auch darauf, [warum man Confide nicht benutzen sollte](https://www.cyberscoop.com/confide-app-security-audit-donald-trump-white-house/), z.B. [weil Marketing echte Verschlüsselung nicht ersetzen kann](https://www.cyberscoop.com/confide-favorite-app-trumps-white-house-triumph-marketing-substance/).

Und um 15:51 kommentierte [Robert](http://hackerb.it):

> Uff! Messenger benutze ich schon seit Monaten nicht mehr. Im Grunde vertraue ich keinem Messenger und bin bisher auch ohne ganz gut zurecht gekommen.
>
> P.s. PGP muss ich auch wieder neu einrichten. Danke für das erinnern.

Nun... Das mit dem Vertrauen gilt aber auch, solange man nicht ausgewiesener Kryptografie-Experte ist, für PGP. Zwar sehe ich da - im Gegensatz zu einem Krypto-Messenger - den Kryptotext; dass der aber schwer bis nicht zu knacken ist, muss ich genauso glauben wie bei z.B. Signal oder Threema. Beide sind durch unabhängige Audits gegangen, die Signal-Verschlüsselung ist darüber hinaus *open source*, und beide gelten als sicher.

Was die Verschlüsselung angeht, gilt sogar WhatsApp als sicher, weil es das gleiche Protokoll benutzt wie Signal; hier ist nur das Datensammelverhalten drumherum hochproblematisch.

*Aktualisiert am 21.07.2020*
