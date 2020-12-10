+++
title = "Aus dem Maschinenraum"
date = 2019-06-01T12:50:36+02:00
draft = false
tags = ["blogging","Hugo","WordPress","Indieweb"]
categories = ["blog"]
cover = "/images/engine.jpg"
authors = ["kkl"]
+++
Nö. Denkverbote gibt's hier nicht. Weshalb ich mir auch (in einem meiner schwächeren Augenblicke) erlaube, darüber nachzudenken, was wäre, wenn... Doch wieder ein CMS? Gar etwa eine Rückkehr zu WordPress, nach mehr als einem Jahr mit [statisch erzeugten Seiten](../hugo/)? Einfach, weil es ungleich viel einfacher ist, Änderungen vorzunehmen - oder gar [neue Funktionen](../ganz-genau/) einzubauen? Mit Hugo ist es eine Menge *trial and error*, in der Welt von WordPress ein Klick, mit dem ein Plugin installiert wird. Und das, wo mein Hostingaccount ohnehin "Managed WordPress" enthält, also automatische WP-Updates, wann immer sie kommen.

Aber dann gucke ich in die Statistiken dieser Seite und stelle fest, dass eine der beliebteren Dateien dieser Domain "wp-login.php" ist. Über 600 Aufrufe pro Monat fragen (vergeblich, versteht sich) nach dieser Datei; mehr als 20 Mal am Tag versucht jemand (sprich: nicht ich), sich in meine (seit einem Jahr nicht mehr vorhandene) WordPress-Installation einzuloggen.

*Nope.*

Was lernt uns das? Erstens: Bots sind doof und lernunfähig. Zweitens: Ein Ziel, das nicht angeboten wird, kann auch nicht ausgenutzt werden.

### Erste Schritte zum Indieweb

[Hier springt einer auf den Indieweb-Zug auf](https://uninform.at/2019/05/28/webmentions/) und veranlasst mich, den gleichen Sprung zu tun. Die ersten beiden Schritte habe ich schon geschafft: Meine zur Zeit noch verbliebenen Netz-Identitäten, also mein Twitter-Account, mein (ganz neuer und quasi unbenutzter) Mastodon-Account und diese Seiten hier, sind indieweb-gerecht im Header markiert:

    <link rel="me" href="https://konstantinklein.com/" />
    <link rel="me" href="https://twitter.com/konstantinklein/" />
    <link rel="me" href="https://mastodon.sdf.org/@kkl" />
    <link rel="authorization_endpoint" href="https://indieauth.com/auth" />

... und mit der vierten Zeile habe ich [gemäß dieser Anleitung](https://www.amitgawande.com/indiewebify-hugo-website/) auch schon das "Web Sign-in via IndieAuth" vorbereitet. Was das eigentlich ist, kriege ich sicher auch noch heraus.

Und dann habe ich, ebenfalls nach der Anleitung von [Amit Gawande](http://amitgawande.com/), meine Identiät via h-card auf die Seiten gepackt:

    <p class="h-card vcard">
    	<a style="text-decoration: none" href=https://konstantinklein.com class="p-name u-url url author metatag" rel="me"> Konstantin Klein</a> /
	    <a class="p-nickname u-email email metatag" rel="me" href="mailto:mail@konstantinklein.com">Konstantin</a>
    	<img class="u-photo" src="/images/bluemesquare.png" alt="" />
    </p>

Der nächste Schritt ist dann der, die Inhalte indieweb-gerecht, also maschinenlesbar auszuzeichnen. Das ist mit Hugo nicht ganz so einfach; während die beiden angeführten Änderungen einfach durch Overrides des hier genutzten Themes eingebaut waren, muss ich für die Auszeichnung des Inhalts in die Tiefen des Themes eintauchen.

Bevor ich das aber mache, denke ich lieber noch mal darüber nach, ob ich bei dem hier verwendeten Theme [Minimo](https://themes.gohugo.io/minimo/) bleiben will. Im vergangenen Jahr habe ich mehr als einmal festgestellt, dass der Minimo-Autor gelegentlich unorthodoxe Wege beschreitet, die Erweiterungen und Änderungen an Hugo schwerer machen - einfach, weil die Theme-Struktur von Minimo oft anders (und komplizierter) ist als die in den diversen HOWTOs beschriebene.

Und weil an diesem Wochenende wunderschönes Frühsommerwetter herrscht, verschiebe ich diese Gedanken noch etwas.
