+++
title = "Ein Rückblick, oder so"
date = 2019-01-20T11:57:05+01:00
draft = false
tags = ["Blogging","Blog","Werkstatt","Geschichte"]
categories = ["Blog"]
cover = "/images/rueckblick.jpg"
authors = ["kkl"]
+++
[Ein Weblog also](https://konstantinklein.com), mit [sehr überschaubarem Funktionsumfang](../hugo/), mit überschaubarem Beitragsaufkommen, mit überschaubarer Laufzeit (seit Mai 2018). Niemand sieht, dass Blogging in dieser meiner Ecke des Netzes schon eine gewisse Tradition hat, niemand sieht - eine bloghistorische Schande, aber nicht mehr zu ändern, und man muss auch lassen können - die Vielfalt von ~~Dummheiten~~ Themen, die ich an dieser Stelle schon angeschrieben habe. Aber als alter Blogzausel&trade; nehme ich mal die Gelegenheit wahr und erzähle von früher, von der Technik von NewsPro bis [Hugo](https://gohugo.io/).

Angefangen hat alles im Herbst 2000. Ich arbeitete als freier Journalist in Washington, DC, betrieb eine Website unter der bekloppten Domain worldwideklein.com (schon lange in den Fängen von Domainvermarktern) und hatte den Eindruck, ich müsste zusätzlich zu den Informationen über mich und meine Angebote *content* anbieten, um Lesern einen Anreiz zum regelmäßigen Vorbeigucken zu bieten. Dass es sowas schon gab, dass man sowas "Weblog" nannte und dass es sogar schon erste Softwarelösungen dafür gab, wußte ich nicht. Man war ja  so ahnungslos.

### NewsPro

Also machte ich mich (immerhin: ein Internet zum Suchen gab es damals schon, und es hieß schon damals Google!) auf die Suche nach einer Möglichkeit, täglich neue Inhalte in meine Website zu packen, ohne ständig neue Seiten mit der Hand (nun ja, mit *copy'n'paste*) erzeugen zu müssen, und fand **NewsPro**, ein [CGI-Script](https://de.wikipedia.org/wiki/Common_Gateway_Interface), das Textdateien erzeugte, die ich dann mit [Server Side Includes](https://de.wikipedia.org/wiki/Server_Side_Includes) in ein selbstgeschriebenes Template einbaute. Alles furchtbar primitiv, und schon damals im NewsPro-Forum als veraltet kritisiert.

Zum Glück war im selben Forum hoffungsvoll die Rede von [Coranto](http://www.coranto.org/shtml/), dem Nachfolgeprojekt für NewsPro, an dem der geheimnisumwitterte NewsPro-Entwickler arbeiten sollte, der nur unter seinem Pseudonym **elvii** bekannt war. Das war schon im Jahr 2001, in dem Jahr also, in dem elvii... spurlos aus dem Netz verschwand, unter Zurücklassung eines fast fertigen Coranto, und mich mit einem Weblog-System (inzwischen wusste ich schon, dass es sowas gab) ohne Zukunft zurückließ.

Coranto wurde übrigens schließlich von NewsPro- und Coranto-Fans fertiggestellt; die letzte Version (siehe Link) stammt von 2007.

### phpWebLog

Neben meiner frühen Bloggerei suchte ich also nach Alternativen, und da mein damaliger Hosting-Anbieter puretec (heißt heute 1&1, oder Ionos, oder was) gerade PHP als Scriptsprache anbot, landete ich bei meiner ersten PHP-Webloglösung [phpWebLog](https://en.wikipedia.org/wiki/PhpWebLog). Wer dem Wikipedialink folgt, sieht auch gleich das Problem: Im Mai 2001 stellte ich mein Weblog - schon damals unter Zurücklassung der alten Inhalte, denn Importieren war nur durch Abtippen möglich (oder durch *copy'n'paste*) - auf phpWebLog um - und im Oktober des gleichen Jahres stellte der Entwickler die Arbeit an phpWebLog ein. Na, super.

Immerhin stellte das System einen großen Sprung in meiner persönlichen Lernerfahrung dar. Es arbeitete nämlich noch mit tabellenbasiertem Layout (den Älteren werden jetzt mehr oder weniger wohlige Schauer über den Rücken laufen), und ich verbrachte unzählige Stunden damit, meine Seite mit phpWebLog in ein reines CSS-gesteuertes Layout umzubauen. Hinterher sah die Seite genau gleich aus, aber ich hatte viel gelernt. Unter anderem, dass auch phpWebLog keine Zukunft hatte...

### Bewegliche Lettern

Es folgte die erste (von insgesamt drei) Phasen, in denen ich [MovableType](https://movabletype.org/) benutzte, damals ein aufstrebendes Blogsystem, inzwischen [ein Klassiker](https://en.wikipedia.org/wiki/Movable_Type), der statische Seiten (!) ausschrieb. Auch damit war es einfach, ein eigenes Layout zu entwerfen und zu schreiben und dann die Inhalte von MT einzubauen. MovableType war (und ist es vermutlich immer noch) sehr flexibel, und als immer noch in Washington bloggender Blogger betrieb ich mein Blog auf deutsch und auf englisch - mit Querverlinkungen und Teasern auf der jeweils anderen Seite.

Leider stieß ich dabei an die Grenzen meines Hosting-Accounts. Damals war es offenbar üblich, bei *shared hosting*-Accounts die Laufzeit von Skripten eng begrenzt zu halten, damit die anderen Nutzer des gleichen Servers nicht darunter zu leiden hatten. Bei den ganzen Kreuz-Verlinkungen in meinen Blogs passierte es recht schnell, dass beim Ausschreiben der Seiten MT in ein Timeout rasselte und mich mit halben oder leeren Seiten zurückließ. Das Problem hatte offenbar nicht nur ich, und die Entwickler von MovableType boten später auch die Lösung an, die Seiten in einzelnen Schüben auszuschreiben, aber da hatte sie schon begonnen...

### ...die Zeit mit Ellis

(Jetzt wäre es langsam mal Zeit für einen Screenshot oder ein anderes Bild, nicht? Schade, dass ich das damals für überflüssig gehalten habe.)

Im Jahr 2002 wies mich jemand aus [Kleinbloggersdorf](../kleinbloggersdorf-revisited/), also der deutschsprachigen Weblog-Gemeinde auf ein vielversprechendes neues System hin: **pMachine**, mit "p" wie "publishing". pMachine arbeitete wie phpWebLog unter PHP, hatte wie *meine* Version von phpWebLog ein CSS-gesteuertes Layout und kam, wie viele derartige Systeme damals, nur mit einem Standardlayout und der Möglichkeit, den PHP-Code leicht in ein eigenes Layout einzubauen. Mit der pMachine experimentierte ich fleißig herum, baute und betrieb sogar eine wüste Kombi aus *drei Blogs*, zwei auf deutsch, eines auf englisch, *mit einer pMachine-Instanz* (war aber richtig viel Arbeit, gleich drei Blogs auf einmal zu füttern...) und hatte viel Spaß damit - bis [der Entwickler Rick Ellis](https://en.wikipedia.org/wiki/EllisLab) schrieb, dass pMachine ein Auslaufmodell sei...

Zum Glück blieb die pMachine aber nicht ohne Nachfolger. Ellis arbeitete an der [ExpressionEngine](https://expressionengine.com/), einem kommerziellen CMS, und weil ich mich schon an der deutschen Übersetzung der pMachine-Oberfläche beteiligt hatte, schrieb ich für die erste Version der ExpressionEngine wieder die deutsche Übersetzung und bekam dafür eine lebenslange Lizenz - die ich dann ungefähr bis 2005 auch nutzte.

(Jetzt wird es aber wirklich Zeit für ein Bild, um den Augen Erholung von dieser ~~Blei~~ Buchstabenwüste zu gönnen. Bittesehr:)

![Zwei Macs im Dreivierteltakt](/images/macsphere.jpg "Zwei Macs im Dreivierteltakt")

So arbeitete ich 2005 also - mit einem schon damals ehrwürdigen [PowerMac Cube](https://de.wikipedia.org/wiki/Power_Mac_G4_Cube) und einem der ersten Intel-MacBooks. Und auf dem Bildschirm ist [ein Blog](https://vowe.net) zu sehen, dass der Autor lange Jahre - evtl. immer noch? - mit MovableType betrieben hat, quasi der exakte Gegenentwurf zu meiner Bloglaufbahn, die im Grunde eine Reihe von Test- und Probefahrten der jeweiligen Systeme war.

### Zwischenspiel mit blogger

In diesem Jahr - 2005 - ging das Gemeinschaftsblog, das ich mit der EE betrieb, ein wenig den Bach hinunter, und um nicht aus der Übung zu kommen, setzte ich ein Nebenblog auf - mit der inzwischen auch ehrwürdigen, längst von Google gekauften und betriebenen Maschine [blogger](https://draft.blogger.com/blogger.g#welcome). blogger hatte damals eine Funktion, die ich kurz darauf sehr vermisste: Anders als heute musste der blogger-Nutzer sein Blog nicht unter einer der wg. vieler Spamschleudern anrüchigen blogger-Domains hosten, sondern konnte das fertige bzw. jeweils aktualisierte Blog als statische Seiten (!) auf einen Webspace der eigenen Wahl (!!) kopieren lassen.

### Noch ein Klassiker

Im Herbst 2006 (hatte ich damals denn keinen Job und kein Privatleben? Doch, aber ich kam offenbar mit sehr viel weniger Schlaf aus als heute...) probierte ich dann, ob es wirklich wahr war, was die Macher von [WordPress](https://wordpress.org/) behaupteten: eine Installation in fünf Minuten? Das kannte ich so noch nicht.

Nun, jetzt kenne ich es - wie die Mehrheit der Blogger, die ebenfalls WordPress benutzen. Auch mit WordPress spielte ich noch ein wenig herum, bis ich meine Prioritäten anders setzte und einfach nur bloggte, mal mehr, mal weniger, mal gar nicht, aber immer mit WordPress. Das System ist so verbreitet, dass ich dazu nichts weiter zu sagen habe.

### Statisch und doch dynamisch

Wer mir bis jetzt durch diese lang~~weilig~~e Geschichte gefolgt ist, hat vielleicht bemerkt, dass meine Bloghistorie durch einen regelmäßigen Wechsel von statisch erzeugten (HTML-) und dynamisch servierten (PHP-) Seiten gekennzeichnet ist. Dynamisch erzeugte Seiten wirken, nun ja, dynamischer (dem Leser dürfte das m.E. sowieso wurscht sein), sind aber aufgrund der verwendeten Systeme gerne ein wenig anfällig für unsaubere Angriffe. Weshalb ich schon die letzten paar Jahre  im WordPress-Land immer wieder statische Seiten-Generatoren testete, bis ich im letzten Mai endlich bei [Hugo](../hugo) und der derzeitigen Version meines Blogs landete. Uff!

### Irrungen und Wirrungen

Ach ja, da gab es noch zwei völlig bekloppte und zum Glück nicht lange anhaltende Episoden - einmal der Versuch, mit dem CMS [Joomla](https://www.joomla.org/) ein Blog aufzusetzen und zu betreiben (doch, es geht&trade;, war aber irrwitzig umständlich), und dann der Versuch, mit selbstgeschriebenen [Shell-Skripten](https://de.wikipedia.org/wiki/Kommandozeile) (!) ein Blog zu betreiben. Das blieb nicht-öffentlich, weil es nicht über das Stadium einer Fingerübung hinauskam, aber: Auch das ging&trade;!
