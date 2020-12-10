+++
title = "Yes, back to the roots!"
date = 2020-08-17T16:27:42+02:00
draft = false
tags = ["blogging","Hugo","Linux","Ubuntu"]
categories = ["Blog"]
cover = "/images/root2.jpg"
authors = ["kkl"]
+++
...aber anders, als [an dieser Stelle](/posts/back-to-the-roots/) angedacht und beschrieben. Ich blogge selbstverständlich weiter mit Hugo, und doch ist hinter den Kulissen einiges anders. Weil das aber von außen keiner sieht, könnte ich mir diesen Text auch sparen. Mache ich aber nicht, weil hier schon länger nichts Neues (oder wie ich zur unendlichen Anödung meiner Kollegen im dienstlichen Zusammenhang oft schreibe: "Nick's Neuss") stand.

Also: Von 2005 bis 2008 und nochmal von 2010 bis 2016 war Linux das Hauptbetriebssystem in meinem Hause; dazwischen hatte ich meine Mac-Phase, die allerdings abrupt endete, als mein Mac Mini genau nach dem Ende der Garantiefrist ganz entschieden (mit einem Festplattenschaden) die Biege machte und das Macbook schon in den Händen der Ehefrau war. 2016 dann war ich etwas angefressen, als mein damals neu gekaufter, angeblich zu 100 % Linux-kompatibler Laptop genau das nicht war, sondern regelmäßig einfror und nur mit einem Kaltstart wieder zu wecken war. Also packte ich das mitgelieferte Windows wieder drauf, und als zwei Jahre später auch der Desktoprechner ersetzt werden musste, lief auch darauf das mitgelieferte Windows.

Inzwischen altert mein Klapprechner allerdings zusehends, und das ist ja gerne ein Anlass, der Hardware mit Linux den *second wind* einzuhauchen und selbst nicht ganz aus der Übung zu kommen.

Auf dem kleinen Rechner läuft jetzt also (wieder) Ubuntu, und offenbar haben die Entwickler die letzten vier Jahre genutzt: Das Dings friert auch nicht mehr ein.

### Und Hugo?

Ja. Hugo ist ja unter Windows immer so ein wenig ein Fremdkörper geblieben. Selbstverständlich gab und gibt es fertige .exe-Versionen für Windows. Aber irgendwie... irgendwie stimmte das nicht (was natürlich Quatsch ist, weil es ja funktioniert). Beispielsweise errechnet das für seine Geschwindigkeit berühmte Hugo auf der eindeutig älteren Hardware unter Ubuntu die Seiten mehr als doppelt so schnell wie auf dem drei Jahre jüngeren Windows-Rechner (Geschwindigkeitsmonster sind beide nicht). Und überhaupt hat Hugo in meinen Augen einen ganz eindeutigen &ast;nix-Hintergrund, und den möchte ich in der nächsten Zeit näher erforschen und ausnutzen.

Was das besonders Schöne an diesem Text ist: Er entstand gleich nach dem Kopieren meines Blog-Verzeichnisses auf den frischen Ubuntu-Rechner und der Installation von Hugo aus dem Repository. Dort, also im Repository, liegt eine minimal ältere Version von Hugo, die diese Seiten aber problemlos ausschreibt. Und weil Ubuntu bzw. seine Macher ja immer alles anders machen wollen, gibt es auch eine [Snap-Version](https://de.wikipedia.org/wiki/Snappy_(Paketverwaltung)), die gleich mehrere Versionsstufen neuer ist und mit dem Theme nicht zusammenarbeiten will - weshalb ich die ältere Version installiert habe und ich mich als nächstes daran machen werde, dass sie bei den sonst sehr komfortablen Aktualisierungen eben *nicht* aktualisiert wird.

**Update:** Wieder was gelernt (und das nach all den Jahren!):

    # sudo apt-mark hold hugo

Und so findet mein Blog einstweilen auf dem Laptop statt. Und hier natürlich. *That's all.*

#### Kommentar

Peter van I. meldete sich umgehend und schrieb:

> Respect!
>    
> /&ast;sounds of thunderous applause, not often heard outside the hallowed grounds of the Chinese Communist Party headquarters during its yearly assembly&ast;/

Und weiter:

> reason for another round using Hugo is this little typo near the end
>    
>> ich mich sls nächstes daran

Und ich dachte immer, das wäre meine ganz persönliche Berufskrankheit, der sog. Gemeine Redakteursblick, der den Patienten sofort kleine und kleinste Tippfehler (umgehend korrigiert) finden lässt.
