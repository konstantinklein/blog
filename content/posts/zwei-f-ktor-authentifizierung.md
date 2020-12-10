+++
title = "Zwei-F*ktor-Authentifizierung"
date = 2019-12-15T17:09:43+01:00
draft = false
tags = ["E-Mail","Passwort","2FA","Sicherheit","Gesetz"]
categories = ["Blog"]
cover = "/images/privacy.jpg"
authors = ["kkl"]
+++
Weiß der Himmel, wie mir gestern morgen ausgerechnet ein FAZ-Artikel in die Timeline gespült wurde. Jedenfalls, es geschah, und ich las [Bundesregierung will an E-Mail-Passwörter](https://www.faz.net/aktuell/wirtschaft/digitec/hassrede-bundesregierung-will-an-e-mail-passwoerter-16535665.html):

> In ihrem Entwurf für ein Gesetz gegen Rechtsextremismus und Hassrede hat die Bundesregierung sich auch auf einen neuen Behördenanspruch auf Passwörter zu Onlinediensten geeinigt. Das geht aus einem am Freitag vorgestellten Referentenentwurf des Bundesjustizministeriums hervor. Künftig können demnach Behörden unter bestimmten Voraussetzungen von Diensten wie Google oder Facebook verlangen, Passwörter zu Kundenkonten zu erlangen.

Zunächst führte ich - ungerecht, wie ich am Samstagmorgen sein kann - das auf ein, sagen wir: Missverständnis seitens des FAZ-Autoren zurück. Passwörter abfragen - pfff! Was soll das denn bringen, wo doch inzwischen sogar Tante Ernas Onlineshop Passwörter nur noch verschlüsselt speichert?

Dann aber kamen auch aus anderen Quellen Artikel in meine Timeline, und ich verstand, dass das, sagen wir: Missverständnis nicht an einem Schreibtisch der FAZ entstanden war: [Justizministerium: WhatsApp, Gmail & Co. sollen Passwörter herausgeben müssen](https://www.heise.de/newsticker/meldung/Justizministerium-WhatsApp-Gmail-Co-sollen-Passwoerter-herausgeben-muessen-4615602.html).

### In einem Wort: Unfug

Sagen wir mal so: In einem von der Piratenpartei geführten Justizministerium wäre das nicht passiert. Viel anderer Unfug, ja, sicher, aber das nicht.

Nochmal: Auch in einem Land, das in Punkto Digitalisierung noch dazulernen kann, sollte sich herumgesprochen haben, dass jeder halbwegs seriöse Diensteanbieter Passwörter *verschlüsselt* speichert; bei den mir bekannten Lösungen bekommt er das Passwort nie unverschlüsselt zu Gesicht, und wenn der User beim Login sein Passwort eingibt, wird es bereits (*Update, s.u.:* transport-)verschlüsselt übertragen, auf dem Server dann verschlüsselt und mit dem gespeicherten Hash verglichen - und dann (so soll es jedenfalls sein) vergessen.

Das gespeicherte verschlüsselte Passwort nützt aber keinem etwas, weil es bei der Eingabe durch Doofe nochmal verschlüsselt wird und mit dem gespeicherten Wert wieder nicht übereinstimmt; rückwärts entschlüsseln lässt sich ein vernünftig verschlüsseltes Passwort aber nicht. Und sog. "backdoors" einbauen zu wollen, fällt gerade Politikern und Politikerinnen immer wieder als Lösung ein; das ist aber sogar aus der Sicht amerikanischer Geheimdienstler und FBI-Chefs eine dumme Idee, weil derartige Hintertüren leider auch von denen genutzt werden, die sie nicht nutzen sollen.

Also könnten wir den Gesetzentwurf aus dem (sagte ich es schon? SPD-geführten) Justizministerium zu den Akten legen. Oder kurz darüber nachdenken, was gegen Passwortklau, ob auf Gesetzeswegen oder ungesetzlich, wirkt.

Na? Richtig: [Zweifaktorenauthentifizierung](https://de.wikipedia.org/wiki/Zwei-Faktor-Authentisierung). Also die Einrichtung, bei der die Kenntnis von Nutzername und Passwort nicht ausreicht zum erfolgreichen Login, sondern ein weiterer Faktor, ein Hardwareschlüssel oder ein *one time password*, erzeugt von einer entsprechenden App, erforderlich ist. Wer diesen Faktor nicht hat oder nicht kennt, kann sich alle Passwörter der Welt per Gerichtsbeschluss oder auch ohne besorgen - sie nützen ihm nichts. Ha!

### Aber: Das große Aber

Leider hat 2FA, wie ich sie zärtlich nenne, einen Nachteil oder zwei. Weil sie nämlich von den vielen verschiedenen Mail-Clients da draußen, von Thunderbird bis K-9 und zurück, nicht unterstützt wird, bieten viele (die meisten? Alle?) Maildienste an, zwar den Zugang zur Weboberfläche mit 2FA abzusichern, den für die Apps, also über Protokolle wie POP oder IMAP, aber auch dem zu gewähren, der nur das Passwort kennt. Wer das nicht will, kann bei solchen Diensten den Zugang via POP/IMAP sperren - und damit den Zugang von der Mobilquatsche gleich mit, da die gängigen Mailclients für Android und iOS dann vor verschlossenen Türen stehen (und Webmail auf einem Handy ist nun wirklich Quälerei!).

Einen Ausweg aus dem Dilemma 2FA vs. IMAP bieten nur die Mailanbieter, die eigene Apps zum Mailen anbieten, in denen die 2FA integriert sind. Also solche Datenschutzkünstler wie GMail, Outlook.com, GMX etc.

Immerhin: Auch der deutsche Anbieter Tutanota bietet eine solche App mit 2FA-Integration an (wobei das eine [Electron-](https://de.wikipedia.org/wiki/Electron_(Framework)) bzw. Web-App ist, was die Sache leichter macht). Aber [dort hat man andere Probleme](https://konstantinklein.com/posts/lesen-bildet-ungemein/#stunden-eine-woche-sp%C3%A4ter).

#### Update

Leser Christian F. hat natürlich völlig Recht, wenn er mir schreibt:

> Wenn Du schreibst, dass das Passwort bereits verschlüsselt übertragen wird, meinst Du dann, dass die Übertragung verschlüsselt ist? Bei serverseitiger Codeausführung  müsste ja dann JavaScript zum Beispiel das Passwort erst verschlüsseln. Würde tippen, dass das eher selten ist. Oder doch nicht?

Und deshalb habe ich den entsprechenden Absatz weiter oben korrigiert. Wenn das Passwort nicht per Javascript lokal verschlüsselt wird, kommt es nach einem hoffentlich verschlüsselten Transport natürlich in unverschlüsselter Form auf dem Server an, wird dort verschlüsselt und dann mit dem gespeicherten Wert verglichen. Danach wird es verworfen - wenn nicht eine finstere Macht es vorher irgendwo unverschlüsselt gespeichert hat. Aus Angst vor Hackern und den diversen Datenschutzverordnungen macht das aber niemand, der seine sieben Zwetschgen noch beisammen hat.
