![Header logo](/img/header.png)

OHC-doc
=======

## LERNERSATZLEISTUNG
im Fach Informatik an der Klaus-Groth-Schule Neumünster

vorgelegt von Tobias Schramm, Florian Siewers, Jasper Masekowsky, Tom- Calvin Haak & Finn Werft

Klasse: 12 Physik A
Lehrer: Herr Krause
Datum: 20.01.2015

## INHALTSVERZEICHNIS

1. Motivation & Idee
2. Anforderungen
3. Organisation & Zeitplan
4. Website
5. Funktionsweise
  * Hardware
  * Software
6. Bedienungsanleitung
  * Login
  * Gerät hinzufügen
  * Gerät bedienen
  * IP Adresse konfigurieren
7. Verbesserungen & Ideen für die Zukunf

## QUELLENVERZEICHNIS
Abbildung 1:
www.de.wikipedia.org/wiki/Open_Source#mediaviewer/File:Opensource.svg
abgerufen am 19.12.2014
Abbildung 2:
www.roboter-bausatz.de/media/image/thumbnail/FZ0550-2_720x600.jpg
abgerufen am 10.01.2015
Abbildung 3:
www.de.wikipedia.org/wiki/Datei:Raspberry_Pi_Logo.svg
abgerufen am 10.01.2015

## ABBILDUNGSVERZEICHNIS
Abbildung 1: Open Source
Abbildung 2: Funkmodul
Abbildung 3: Raspberry Pi
Abbildung 4: Schaltplan des Raspberry PI's mit Funkmodul
Abbildung 5: Schaltplan einer ferngesteuerten Steckdose
Abbildung 6: Schaltplan ohne Netzteil & Relais
Abbildung 7: Login
Abbildung 8: Übersichtsliste
Abbildung 9: Dimmbares Gerät
Abbildung 10: Dimmbarer Prototyp
Abbildung 11: Nicht dimmbares Gerät
Abbildung 12: IP Adresse manuell setzen
Abbildung 13: IP Adresse eingeben

## 1. Motivation & Idee
Wer kennt das nicht?
Müde und geschafft kommt man nach getaner Arbeit nach Hause, schaltet das Licht im Flur an,
anschließend im Wohnzimmer - vier neue, stimmungsvoll dimmbare Ikea Lampen (Nachdem
man dreimal ums Sofa gekrochen ist, sind sie dann auch alle gleich hell.) jetzt noch den Fernseher
und die Stereoanlage an machen. Geschafft!
Und jetzt? Gleich aufs Sofa? Nein! Lieber schnell noch was zu essen holen. Also ab in die Küche,
Licht an, Radio an, Schnittchen schmieren und eine Tüte Chips mitnehmen.

[...]

Nach dem zweiten durchlauf der Tagesschau, einer Folge TV Total und einer Wiederholung
der Heute Show ist es dann so weit: Am liebsten möchte man direkt im Bett liegen!
Daraus wird leider nichts. Denn erstmal muss man gefühlt eine halbe Stunde durchs Haus laufen,
um jede Lampe und jedes Gerät einzeln wieder auszuschalten.
Sobald der Rundgang beendet ist und man dann doch endlich im Bett liegt, hört man ein Geräusch...
Die Nachbarn? Oder habe ich mich getäuscht? Nein, da ist es wieder! Laut und deutlich!

„Ding Dang Dong! Hier ist das erste deutsche Fernsehen mit der Tagesschau!“
Verdammt! Fernseher vergessen... Also wieder aufstehen und ins Wohnzimmer laufen! Oder
war’s der Fernseher im Bad?
Egal - nach dem dritten Durchlauf der Tagesschau liegt man dann doch endlich wieder im Bett
und kann mit etwas Glück sogar durchschlafen.
Möglicherweise schlagen Sie sich seit längerem mit ähnlichen Problemen rum und dachten diese
mit einem Arsenal an Funksteckdosen beheben zu können.
Nun, entweder haben Sie ihr Auto verkauft, sämtliche Sparverträge aufgelöst, eine Hypothek
aufs Haus aufgenommen und lassen Ihre Kinder arbeiten, um ein „Premium Home Controlling
Solution System“ (oder so ähnlich) mit elektrischen Velux Fenstern finanzieren zu können oder
aber Sie schlagen sich mit den folgenden Problemen herum.
Immer dann, wenn Ihr Chef Ihnen einen Einlauf verpasst und Ihr Gehalt gekürzt hat, Ihr Sohn
eine 5 in Mathe mit nach Hause bringt und Ihre Frau das Auto gegen die Wand gesetzt hat, Sie
also bei bester Laune sind, ist die Batterie Ihrer Fernbedienung leer.
Ein anderer Fall... Sie haben neue Lampen und Steckdosen für Ihr Arbeitszimmer gekauft und
möchten diese schnell aufbauen und ausprobieren. Schade! Alle verfügbaren Frequenzen der 2
Fernbedienung sind belegt. Entweder das Arbeitszimmer wird beleuchtet, wenn Sie im Wohnzimmer
TV und Stereoanlage einschalten oder aber wenn sie das Licht im Schlafzimmer an
machen - oder doch lieber zusammen mit dem TV im Bad?

Klingt alles nicht nach einer zufriedenstellenden Lösung! Und die Fernbedienung liegt sowieso
immer am falschen Ende Ihres Hauses. Jetzt könnten Sie natürlich für jeden Raum eine Fernbedienung
anschaffen, dann haben Sie allerdings bald genug Systeme, um sie über fünf Generationen
an sämtliche Nachfahren zu vererben... Diese werden sich sicher freuen!
Eines kann Sie aber noch schlimmer treffen! Der Super GAU!

Ihr Nachbar ist neuerdings auch stolzer Besitzer einer Sammlung von Funksteckdosen... Er funkt
auf derselben Frequenz.
Der folgende Wettbewerb um die Beleuchtungshoheit ist für Außenstehende mit Sicherheit
lustig anzusehen, für Sie jedoch einfach nur nervtötend.
Wir von OpenHC dachten: „Es muss eine Lösung geben!“ und schon war die Idee unseres
Projektes geboren. Wir wollten ein in jeder Hinsicht besseres System zur Kontrolle der Elektrogeräte
im Haushalt entwerfen und konstruieren. 

## 2. Anforderungen
Zu Beginn der Projektarbeit müssen wir uns natürlich zunächst über die Anforderungen an unser
Vorhaben Gedanken machen und dementsprechende Zielsetzungen entwerfen.
Diese sind zum einen durch die Vorgaben aus dem Unterricht gegeben (Arbeitsauftrag: Programmieren
Sie eine Android Applikation), zum anderen aber auch durch unsere Kritikpunkte
an bisherigen Systemen zur Fernsteuerung von Haushaltsgeräten.
Da es nicht unsere Absicht ist aus dem Projekt Profit zu schlagen,
ist das erste Kriterium schnell gefunden. Um das System so
kostengünstig wie möglich zu gestalten, aber auch um jedem die
Möglichkeit zu lassen, es nach seinen eigenen Wünschen zu erweitern
und zu optimieren, steht unsere Entscheidung fest, den
gesamten Code als Open Source Software offenzulegen.

![Open Source](/img/opensource-middle.png)


Ein weiterer Punkt ist die erforderliche Hardware. Diese besteht
zum einen aus dem Android Gerät des jeweiligen Anwenders,
zum anderen aber auch aus zwei Geräten, die wir im Rahmen
des Projektes entwickeln müssen. Eines der beiden Geräte ist im
Prinzip eine handelsübliche Funksteckdose, die zwischen das Stromnetz und Endgerät geschaltet
wird und sobald sie ein entsprechendes Funksignal empfängt, die Stromzufuhr ein- oder ausschaltet.
Das andere Gerät stellt hingegen die Schnittstelle zwischen dem Android Gerät und der
„Steckdose“ dar. Es ist entweder über WLAN oder aber per LAN Kabel in das Heimnetzwerk
des Anwenders integriert und empfängt Signale von der App des Android Gerätes, welches sich
entweder im selben WLAN befindet oder aber über einen VPN Zugang von außerhalb zugreift.
Diese Signale leitet es dann per Funk an die App weiter. Hierbei legen wir großen Wert auf die
Verwendung entsprechender Funkstandards, um einen sicheren und zuverlässigen Betrieb zu
gewährleisten.
Natürlich entschließen wir uns auch dazu, die Schaltpläne der Hardware offenzulegen, um beispielsweise
die Option zu erhalten, die „Funksteckdose“ in anderer Bauart an Stelle eines Lichtschalters
für die Kontrolle der Deckenbeleuchtung in die Wand zu integrieren.

## 3. Organisation & Zeitplan
Die Organisation unserer Projektarbeit stützt sich auf die vorhergegangenen Unterrichtsinhalte.
Demnach fangen wir mit der Projektdefinition und -planung an, indem wir uns auf die genannten
„Anforderungen“ einigen und sie als Zielsetzung festhalten. Um das gesamte Projekt übersichtlicher
zu strukturieren, teilen wir die Arbeit in Verantwortungsbereiche auf.
Tobias - Programmierung & Hardware
Florian & Jasper - Website
Tom - Design & Marketing
Finn - Organisation & Dokumentation
Trotz dieser Aufteilung arbeiten wir auch Resort-übergreifend zusammen, besprechen bei unseren
wöchentlichen Treffen im Informatikunterricht bzw. in den Ferien die Fortschritte und
Probleme und entwerfen beispielsweise das Logo und den Namen (OpenHC) in Teamarbeit.
Während der anschließenden Arbeitsphase erfolgt die Projektkontrolle aufgrund des langen Zeitraums
nur an Hand von groben Deadlines6
, welche im Zeitplan festgehalten werden, im Rahmen
des wöchentlichen Informationsaustausches, der auch der Dokumentation dient.
In der Projektabschlussphase in den Weihnachtsferien treffen sich Florian und Jasper, um die
letzten Details an der Website zu besprechen und diese letztendlich fertigzustellen, während
Tobias und Finn sich mit dem letzten Feinschliff an Code und Hardware befassen und die Informationen
für die Dokumentation zusammenstellen.

Kalenderwoche | Datum | Aufgaben
------------- | ----- | --------
36 - 36 | 25.08. - 05.09.14 | Im Unterricht bei Frau Dr. Kröger werden die Grundlagen des Projektmanagements in Bezug auf Softwareprojekte erarbeitet. 
32 - 38 | 08.09. - 19.09.14 | Wir einigen uns darauf eine Android Applikation als Projektarbeit zu erstellen. Ziel ist es, das Projekt an Hand des Gelernten erfolgreich zu strukturieren und bis zur Deadline nach den Weihnachtsferien 2014/15 abzuschließen. Des Weiteren teilen wir uns in Gruppen ein.
