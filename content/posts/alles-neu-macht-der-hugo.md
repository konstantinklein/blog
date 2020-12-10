+++
title = "Alles neu macht der Hugo"
date = 2018-08-16T15:18:52+02:00
draft = false
tags = ["Blogging","Hugo"]
categories = ["Blog"]
cover = "/images/takkatakka.jpg"
authors = ["kkl"]
+++
OK, ich geb's zu: Blöde Überschrift, das. Aber es geht - zur unermesslichen Begeisterung aller technisch weniger Interessierten - mal wieder um [Hugo](../hugo/), und - auch wenn es nicht so aussieht - hier ist alles neu. Und dabei ist noch nicht einmal Mai.

Was ist geschehen?

Nun, eine neue Version von Hugo ist herausgekommen. Und anders als z.B. in der WordPress-Welt, wo der Mensch mit einem Mausklick und etwas Nervenflattern alles auf den neuesten Stand bringt, ist das in der Hugo-Welt nicht ganz so einfach - vor allem, wenn der Mensch, so wie ich, einige Versionen ausgelassen hat.

### Wozu überhaupt Updates?
Eigentlich sind Updates nur dann vonnöten, wenn das Blogsystem der persönlichen Wahl auf einem Server hockt und von außen, also auch von Finsterlingen, erreichbar ist. Dann ist es immer wieder anfällig für Angriffe, die neu entdeckte Sicherheitslücken ausnützen.

Wenn man dagegen seinen Hugo auf dem heimischen PC hocken hat und selbst der einzige Finsterling ist, der darauf Zugriff hat (das ist allerdings Bedingung!), kann man auf Jahre hinaus mit der gleichen alten Hugo-Version und dem gleichen alten Theme arbeiten, wenn man damit zufrieden ist, ohne Angst vor Sicherheitslücken haben zu müssen.

Und dennoch war ich begeistert, als ich kurz nach dem Beginn dieses Abenteuers Hugo 0.40 einfach mit Hugo 0.41 überschrieb - und alles lief wie zuvor.

### Bekenntnis eines Windows-Users
Jahrelang habe ich mit OSX und vor allem Linux herumcomputerisiert. Daher kenne ich auch den Umgang mit Github, dem Repository, wo auch Hugo und das hier verwendete Theme herkommen. Brav habe ich als Inzwischen-wieder-Windows-Nutzer auch git installiert (doch, das geht auch unter Windows) und die Erstinstallation von Hugo damit gemacht. Aber irgendwie kommt mir das unter Windows verkrampfter vor als unter Linux - weshalb ich das erste Hugo-Update eben nicht mehr über git gemacht habe, sondern - wehe mir! - einfach die damals aktuelle Windows-Implementation der Version 0.41 darübergebügelt habe. Hat ja auch geklappt, und wird weiter klappen, bis die Hugomacher die ganze Struktur umschmeißen und mir das alles auf die Füße fallen wird.

### Und dann kam 0.46
Während ich also fröhlich mit der Version 0.41 weiterbloggte (oder auch nicht, aus den bekannten [gesundheitlichen Gründen](../entschuldigungszettel)), blieb die Community nicht faul und entwickelte Hugo weiter - und der Macher [des hier verwendeten Themes Minimo](https://themes.gohugo.io/minimo/) sein Theme. Das kann nun einige Dinge, die ich vorher vermisst habe (mehr dazu, wenn ich das alles auch mal ausprobiert habe), erwartet aber mindestens Hugo 0.45.

Systematisch-unsystematisch, wie ich nun mal bin, bügelte ich zunächst den aktuellen Hugo über den alten und lies ihn zur Probe laufen. Und erhielt mehrere Seiten Fehlermeldungen.

### Go oder nicht Go
Mein Problem ist, dass ich von Go, der Sprache, in der Hugo geschrieben ist, vorläufig so gut wie keine Ahnung habe. Entsprechend schlecht verstehe ich auch, was in den Hugo-Handbuch-Seiten und -Foren so steht. Ich verstand nur, dass mit Version 0.45 einige größere Änderungen gekommen waren.

Version 0.45? Das war doch die, die Minimo jetzt verlangt?

Also zog ich auch die aktuelle Version von Minimo (mangels git-Begeisterung als .zip-Datei), packte sie zu dem brandneuen Hugo, und voilá: Die Kiste läuft.

Ganz so einfach, wie beschrieben, war die Sache auch nicht.  Denn immer, wenn ich hier von "drüberbügeln" fasele, mache ich genau das *nicht* - und das sollte auch sonst niemand machen. Stattdessen kopiere ich fröhlich ganze Verzeichnisse in ihr eigenes Backup und sorge dafür, dass ich immer weiß, welche der vielen Dateien mit dem Namen hugo.exe welche Version ist. So ist meine Hugo-Installation jetzt voll mit mehreren unterschiedlich benannten hugo.exe-Dateien und mit einem kompletten Backup des alten Themes, so dass ich bei Bedarf ~~den ganzen neumodischen Scheiß~~ die neuen Versionen wegschmeißen und dort weitermachen kann, wo ich vor der Entdeckung der neuen Versionen war.

So, und jetzt gucke ich mir an, was der neue Hugo und das neue Theme zusammen so können...
