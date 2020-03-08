---
AUTHOR: Maximilian Menzel
AppVersion: 16.0000
CHANGED: 20200113;20600000000000
CHANGEDBY: Frederik Beimgraben
CREATED: 20191219;800000000000
DocSecurity: 4
GENERATOR: LibreOffice 4.1.6.2 (Linux)
HyperlinksChanged: false
LinksUpToDate: false
ScaleCrop: false
ShareDoc: false
---

::: {type="HEADER"}
+---+---+---+
| \ | \ | \ |
+---+---+---+

\
:::

**Gedankengesteuerte Armprothese**

Ein Projekt von Frederik Beimgraben, Noah Ihlein und Maximilian Menzel

\
\

**Kurzfassung**

Das Ziel unserer Arbeit ist, mithilfe eines EEG-Gerätes ein Programm
(z.B. eine virtuelle - später reale Armprothese) mit zwei oder mehr
Variablen anzusteuern. So könnten billige Prothesen hergestellt werden,
welche sehr gut funktionieren, gleichzeitig aber ohne Operationen
einsetzbar sind.

Unsere Arbeit setzt sich aus dem Bau eines EEG-Gerätes und dem
Programmieren von Software, welche die Daten des EEG-Gerätes verarbeiten
kann, zusammen. Des Weiteren entstehen eine virtuelle Armprothese und
ein Programm, welches diese aus den verarbeiteten Daten des EEG-Gerätes
ansteuert.

Seit Jugend forscht 2019 haben wir ein neues EEG-Gerät gebaut und die
Software erweitert und verfeinert. Mithilfe von neuronalen Netzen können
die Daten des EEG-Gerätes trotz der hohen Komplexität erkannt werden.

[![][1]]{.sd-abs-pos
style="position: absolute; top: 3.08in; left: 3.5in; width: 305px"}[![][2]]{.sd-abs-pos
style="position: absolute; top: 3.08in; left: -0.36in; width: 343px"}[![][3]]{.sd-abs-pos
style="position: absolute; top: 0.17in; left: 1.44in; width: 327px"}[
]{dir="LTR"
style="float: left; width: 3.41in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746094} *Abbildung 1 - Gruppenbild*

[ ]{dir="LTR"
style="float: left; width: 3.18in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746095} *Abbildung 2 - Arbeitsplatz Zuhause*

\
[ ]{dir="LTR"
style="float: left; width: 3.58in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746096} *Abbildung 3 - Headset*

\

**Inhalt** {#inhalt .contents-heading-western align="JUSTIFY" style="margin-bottom: 0.17in; page-break-before: always"}
==========

::: {#Table of Contents1 dir="LTR"}
\
\
:::

\
\

\
\

[]{#_Toc29745973}[]{#_Toc29745892} **1. Einleitung** {#einleitung .western align="JUSTIFY" style="page-break-before: always"}
====================================================

\
\

1.  []{#_Toc29745974}[]{#_Toc29745893} Ideenfindung {#ideenfindung .western align="JUSTIFY"}
    -----------------------------------------------

Zu Beginn des letzten Schuljahres überlegten wir uns ein Projekt, an
welchem wir im Schülerforschungszentrum arbeiten wollten. Wir haben uns
verschiedene Problembereiche angesehen und wir haben gemerkt, dass wir
gerne etwas machen möchten, was sowohl mit Menschen als auch mit Technik
zu tun hat. Durch Zufall hat Frederik EEG-Geräte und deren
Einsatzbereiche im Internet kennengelernt. Durch Recherche haben wir
entdeckt, dass voll funktionsfähige (Arm-) Prothesen bisher nur unter
speziellen Bedingungen einsetzbar sind. So müssen beispielsweise bei
einem Unfall mit Verlust eines Armes die Nervenenden im Arm intakt
bleiben, damit eine Prothese angeschlossen werden kann. Des Weiteren
werden große Operationen fällig, um eine spezielle, extra angefertigte
Armprothese mit dem Körper und Gehirn zu verbinden. All dies ist
natürlich auch mit hohen Kosten verbunden. So haben wir uns dazu
entschlossen, eine Armprothese zu bauen, welche mit den Möglichkeiten
eines EEG-Gerätes arbeitet. Dadurch sollen alle bestehenden Probleme
gelöst werden. In den letzten Monaten ist uns bewusst geworden, dass wir
unser System nicht nur auf Armprothesen, sondern auf jede beliebige Art
von elektrotechnischen Geräten übertragen können, beispielsweise
Drohnen.

\
\

2.  []{#_Toc29745975}[]{#_Toc29745894}[]{#_Toc535146336} Wie möchten wir unser Vorhaben realisieren? {#wie-möchten-wir-unser-vorhaben-realisieren .western align="JUSTIFY"}
    ------------------------------------------------------------------------------------------------

Die Möglichkeit unser Projekt zu realisieren, bekommen wir durch das
Schülerforschungszentrum in Eningen. Wir erhalten dort neben
finanzieller Unterstützung auch Beratung von Lehrern. Außerdem werden
wir finanziell durch das Mikro-Makro-MINT-Programm in Baden-Württemberg
unterstützt. Des Weiteren haben wir Zugriff auf eine Werkstatt, Computer
und auch einen 3D-Drucker. Uns stehen verschiedenste Arbeitsmaterialen
zur Verfügung. Aufgaben, wie z.B. Programmieren oder Planung betreiben
wir aufgrund des hohen Zeitaufwandes nicht nur im SFZ, sondern auch in
der Schule, oder Zuhause über Online-Sprachchats. Durch Open-Source
Projekte, wie OpenBCI erhalten wir einigermaßen kostengünstigen Zugriff
auf EEG-Hardware und haben die Möglichkeit, deren Firmware einfach zu
bearbeiten und schnell passende Software zu programmieren. Mithilfe des
EEG-Gerätes möchten wir unsere Hirnströme während bestimmter Gedanken
messen, um später mit diesen die Prothese anzusteuern. Die Daten des
EEG-Gerätes werden von einer eigens programmierten Software geordnet.
Mit diesen Daten kann dann ein neuronales Netz trainiert werden, das
bereits trainierte und wiederholt auftretende Muster erkennen kann. Die
Ergebnisse des neuronalen Netzes können schließlich zur Steuerung der
Prothese genutzt werden. Da wir aktuell keinen Zugriff auf eine
hochentwickelte bewegliche Armprothese haben, werden wir zunächst eine
simulierte Armprothese oder ein Demonstrationsmodell steuern.

\
\

\
\

[]{#_Toc29745976}[]{#_Toc29745895}[]{#_Toc535146337} **2. Vorgehensweise, Materialien und Methodik** {#vorgehensweise-materialien-und-methodik .western align="JUSTIFY" style="page-break-before: always"}
====================================================================================================

\
\

[]{#_Toc535146338}[]{#_Toc29745977}[]{#_Toc29745896} 2.1 Unsere allgemeine Vorgehensweise {#unsere-allgemeine-vorgehensweise .western align="JUSTIFY"}
-----------------------------------------------------------------------------------------

Zu Beginn unseres Projekts haben wir hauptsächlich jede Woche freitags
im Schüler-Forschungs-Zentrum in Eningen gearbeitet. Dort haben wir
Zugriff auf eine voll ausgestattete Werkstadt, Computer, 3D-Drucker und
Arbeitsmaterialien. Nachteil ist dabei die lange An- und Abfahrtszeit,
welche insgesamt über zwei Stunden dauert. Über viele Wochen hinweg hat
sich die Arbeit immer weiter nach Hause oder auf freie Zeiten in der
Schule verlagert. Vor allem beim Programmieren der Software waren wir
nicht auf das SFZ angewiesen, über das Projektmanagement-Tool „Git"
konnten wir alle immer den aktuellen Code auf unsere Computer/Laptops
laden. Über das Sprachchat-Programm Discord konnten wir miteinander
kommunizieren. Mithilfe von TeamViewer konnten wir auf die Computer des
anderen zugreifen und live sehen, was auf dem Bildschirm angezeigt wird.
Dies war besonders nützlich, wenn Frederik, Maximilian oder Noah beim
Programmieren geholfen hat. Aktuell arbeiten wir circa die Hälfte der
Zeit von zu Hause aus. Unser Betreuer im SFZ hat es uns möglich gemacht,
einen Schlüssel für das Gebäude zu bekommen, wodurch wir nicht mehr an
Freitage gebunden sind und jederzeit das SFZ aufsuchen können. So ist
ein Mix aus verschiedenen Arbeitsstandorten entstanden, was vor allem
unsere Produktivität stark gefördert hat.[![][4]]{.sd-abs-pos
style="position: absolute; top: 2.65in; left: 3.84in; width: 235px"}

[]{#_Toc29745978}[]{#_Toc29745897} 2.2 Funktionsweise eines EEG-Gerätes {#funktionsweise-eines-eeg-gerätes .western align="JUSTIFY"}
-----------------------------------------------------------------------

### []{#_Toc29745979}[]{#_Toc29745898} 2.2.1 Allgemeines {#allgemeines .western}

[]{#_GoBack} Ein EEG-Gerät (Elektroenzephalographie-Gerät) wurde bereits
im Jahr 1929 durch H. Berger entwickelt und wird bis heute
beispielsweise bei der Hirntoddiagnostik oder der Diagnose von
Epilepsien eingesetzt[^1^]. Es wird dabei die Spannungsdifferenz
zwischen zwei Elektroden gemessen bzw. abgeleitet[^2^]. Das
OpenBCI-System ist auf eine sogenannte Referenzableitung bzw. unipolare
Referenzschaltung ausgelegt. Das bedeutet, dass die spannungsaktiven
Elektroden auf dem Kopf mit einer elektrisch inaktiven Referenzelektrode
verglichen werden[^3^]. Diese kann mittig auf dem Kopf oder am Ohr
platziert werden[^4^]. Theoretisch könnte man die Referenzelektrode auch
unterhalb des Kopfes anbringen, dabei bekäme man allerdings Probleme mit
sogenannten Artefakten[^5^]. Artefakte sind Messdaten, die nicht durch
Hirnaktivität entstehen, beispielsweise durch die Bewegung eines Armes
oder statische Ladungen, welche unter anderem durch Reibung des Arms auf
einem Pullover entstehen können. Wir haben aus diesem Grund unsere
Referenzelektroden am Ohr platziert. Eigentlich ist vorgesehen, dass je
Gehirnhälfte eine Referenzelektrode getragen wird, allerdings hatte das
OpenBCI-System Probleme mit dem Erkennen von zwei Ohrelektroden. Deshalb
haben wir beschlossen diese zusammenzuschließen und nun gemeinsam für
alle Elektroden auf dem Kopf zu verwenden. Der Vorteil in der unipolaren
Referenzschaltung liegt darin, dass die Amplituden der einzelnen
Ableitpunkte besser miteinander zu vergleichen sind bzw. einzeln
ausgegeben werden, was für die Funktion der künstlichen Intelligenz (KI)
besser ist. Der Nachteil liegt darin, dass Artefakte häufiger und
stärker auftreten können. Da wir uns beim Trainieren der KI so wenig wie
möglich bewegen, sollte dies dabei allerdings kaum ein Problem
darstellen. Bei einer späteren Verwendung wird die KI Artefakte
größtenteils ignorieren, da immer mehrere Datenreihen gleichzeitig
verarbeitet werden.[ ]{dir="LTR"
style="float: left; width: 2.17in; height: 0.28in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746097} *Abbildung 4 - Unipolare Referenzschaltung*

### 2.2.2 Platzierung der Elektroden![][5][ ]{dir="LTR" style="float: left; width: 3.22in; height: 0in; border: none; padding: 0in; background: #ffffff"} {#platzierung-der-elektroden .western}

[]{#_Toc29746098} *Abbildung 5 - 10-20 System nach Jaspers*

Je weiter die Elektroden auf dem Kopf voneinander entfernt sind, desto
höher sind die Spannungsdifferenzen[^6^]. Aus diesem Grund sollten die
Elektroden alle ungefähr denselben Abstand voneinander haben. Von
OpenBCI wird für die Platzierung der Elektroden das 10-20-System nach
Jaspers[^7^] vorgeschlagen, welches international gültig ist. Nach
einigen Recherchen haben wir uns dazu entschieden, dieses System so zu
übernehmen, da für uns so die genausten Ableitungen möglich sind. Das
10-20-System bekommt seinen Namen durch die Art und Weise wie die
Elektroden auf dem Kopf platziert werden. So wird der Kopf in
Prozentabschnitte aufgeteilt. Dies findet im Groben zum einen vom Nasion
zum Inion statt, zum anderen vom linken bis zum rechten Ohr. Die
Elektroden werden nun vom ausgehend Nasion in Richtung der Ohren bis zum
Inion verteilt. Dies geschieht zuerst in einem Abschnitt von 10%,
anschließend vier Mal 20% und zu guter Letzt noch einmal 10%. So kommen
je Kopfseite (rechts und links) 100% zusammen. Dasselbe geschieht bei
den Elektroden, die vom Nasion über den Kopf Richtung Inion platziert
werden. Genauso verfährt man bei den Elektroden, die vom linken zum
rechten Ohr verteilt werden. Die C~Z~, T~7~, und T~8~-Elektroden werden
dabei mehrfach bedacht. Zwischen diesen Elektroden können im Abstand von
10% oder 20% weitere Elektroden platziert werden. Wir haben Elektroden
an folgenden Positionen platziert und als beistehenden Kanal festgelegt
(Hierbei steht F = frontal, Z = Zentral, T = temporal, P = parietal, O =
okzipital, K = Kanal auf Board): F~p1~-K1, F~p2~-K2, F~7~-K9, F~8~-K10,
T~7~-K13, T~8~-K14, P~7~-K5, P~8~-K6, O~1~-K7, O~2~-K8, F~3~-K11,
F~4~-K12, C~3~-K3, C~4~-K4, P~3~-K15, P~4~-K16. Unsere Elektroden sind
also um den Kopf herum und auf halber Höhe zwischen Ohren und der
Oberseite des Kopfes angebracht:[![][6]]{.sd-abs-pos
style="position: absolute; top: 5.95in; left: 0in; width: 224px"}[
]{dir="LTR"
style="float: left; width: 2.78in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746099} *Abbildung 6 - Platzierung der Elektroden auf dem
Ultracortex Mk-IV*

\

[]{#_Toc29745981}[]{#_Toc29745900} 2.3 Bau und Aufbau des EEG-Gerätes {#bau-und-aufbau-des-eeg-gerätes .western align="JUSTIFY" style="page-break-before: always"}
---------------------------------------------------------------------

Seit Beginn unseres Projektes haben wir zwei verschiedene EEG-Geräte
gebaut.[![][7]]{.sd-abs-pos
style="position: absolute; top: 0.03in; left: 3.48in; width: 261px"}[
]{dir="LTR"
style="float: left; width: 2.72in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746100} *Abbildung 7 - Ganglion Board*

Das erste EEG-Gerät war ein einfaches Ganglion-Board mit vier Kanälen
von OpenBCI, einem amerikanischen Unternehmen, dass sich mit der
Entwicklung von EEG-Geräten beschäftigt und gleichzeitig entsprechende
Bauteile verkauft. Wir bestellten uns das OpenBCI Ganglion-Board,
Goldelektroden und Ten20-Leitpaste. Der Zusammenbau dieser Teile
gestaltete sich als sehr einfach und es wurde zusätzlich nur eine Kappe
zum Anbringen der Elektroden am Kopf, ein Gehäuse für das Board und eine
Klammer benötigt, um die Referenzelektrode am Ohr zu befestigen. Wir
haben das OpenBCI Ganglion gewählt, da es nicht allzu teuer, aber
modifizierbar ist und ebenfalls viel frei verfügbarer Code zur
Ansteuerung vorhanden ist. Jeder Teil der Firmware ist frei verfügbar
und da auch die Pläne zum Herstellen der Boards dabei sind, könnten wir
später mit unserem Code kompatible Boards mit mehr Kanälen selbst
herstellen. Dies haben wir jedoch unterlassen, da es nicht sehr einfach
ist, die Boards selbst herzustellen und wir Sorge hatten, dass darauf
die Software möglicherweise nicht funktioniert. ![][8]

Nachdem wir mit diesem EEG-Gerät in der Lage waren, Hirnströme
auszulesen und mit unserer damaligen Software zu verarbeiten, wurde uns
bewusst, dass wir mit vier Kanälen nicht genug Daten sammeln können, um
dauerhaft zuverlässig Messwerte zu bekommen. Aus diesem Grund wollten
wir unser System auf ganze 32 Kanäle erweitern. Dies wäre jedoch ein zu
großer Schritt gewesen, da man bereits mit 16 Kanälen sehr gut die von
uns gewollte Messgenauigkeit erreichen kann. Daher haben wir uns dazu
entschieden vorerst nur auf 16 Kanäle zu erweitern. Die neuen Boards
kamen wieder von OpenBCI, zum einen das „Cyton"-Board mit 8 Kanälen und
dem „Daisy"-Board, eine Erweiterung für das „Cyton"-Board mit 8 Kanälen.
Da wir nun mit einer deutlich höheren Anzahl an Elektroden arbeiteten,
konnten wir die Elektroden nicht mehr einzeln an die Kopfhaut drücken.
Somit musste ein richtiger „Helm" hergestellt werden, an dem die
Elektroden befestigt werden konnten. Das EEG-Gerät wird von vier
Handelsüblichen AA-Batterien betrieben und ist in keiner Weise an das
Stromnetz angeschlossen.

[![][9]]{.sd-abs-pos
style="position: absolute; top: 0.03in; left: 0.08in; width: 292px"}\
\

[ ]{dir="LTR"
style="float: left; width: 3.04in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746101} *Abbildung 8 - Cyton Board mit Daisy Erweiterung*

\
\

Unser zweites EEG-Gerät besteht zu rund 70% aus Teilen, die mit dem
3D-Drucker angefertigt wurden. Die dafür benötigten Modelle sind über
die Webseite von OpenBCI frei verfügbar. Nachdem wir das Grundgerüst für
das EEG-Gerät hatten drucken lassen, mussten wir darin die
Elektrodenhalterungen befestigen. Durch Epoxidharz bekamen diese einen
festen Halt. Die Goldelektroden haben wir vorerst an der Außenseite der
großen Schrauben befestigt und durch sie hindurch mit einer weiteren
Metallschraube mit der speziell beschichteten Trockenelektrode
verbunden. Hierbei ergab sich allerdings das Problem, dass die
Leitfähigkeit der Metallschrauben weit unter dem erwarteten Wert lag,
weshalb die Messwerte zu ungenau waren und viele Störsignale auftraten.
Aus diesem Grund haben wir die Elektrodenhalter und Elektroden so
umplatziert, dass die Goldelektrode direkt an der Trockenelektrode
festgeschraubt wird. Dadurch erhalten wir nun deutlich genauere
Messwerte. Für diesen Schritt kam uns zugute, dass es einfach war, die
Elektroden vom Headset zu entfernen und in Einzelteile zu zerlegen.
Nachdem die Goldelektrode umplatziert war, konnte man alles schnell und
einfach wieder zusammenbauen.

[![][10]]{.sd-abs-pos
style="position: absolute; top: 0.42in; left: 3.32in; width: 293px"}[
]{dir="LTR"
style="float: left; width: 2.43in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746102} *Abbildung 9 - Schraubelektrode für das Headset*

![][11] [ ]{dir="LTR"
style="float: left; width: 3.05in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746103} *Abbildung 10 - Vollständiges Headset*

\
\
\

\
\

Die in *Abb. 01* dargestellten Elektroden bestehen aus einem
Elekrodenhalter (2), der leitend beschichteten Elektrode (1) und der
Goldelektrode (3), mit dem damit verbundenen Kabel. In Abb. 0-2 ist das
ganze Headset mit den montierten Boards zu sehen. Bei diesem handelt es
sich um das von OpenBCI frei zur Verfügung gestellte „Ultracortex Mark
IV" Headset. Die Platzierung der Elektroden erfolgt über das bereits
erwähnte für elelektroenzephalographische Messungen typische
10-20-Prinzip, mit dem sich Reaktionen am besten ableiten lassen.
[![][12]]{.sd-abs-pos
style="position: absolute; top: 1.28in; left: 3.52in; width: 274px"}

\
\

\
\

[ ]{dir="LTR"
style="float: left; width: 2.85in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746104} *Abbildung 11 - Aufnahme von Messdaten*

\
\

[]{#_Toc29745982}[]{#_Toc29745901} 2.4 Entwicklung und Funktion der Software {#entwicklung-und-funktion-der-software .western align="JUSTIFY" style="margin-bottom: 0.17in; page-break-before: always"}
----------------------------------------------------------------------------

### []{#_Toc29745983}[]{#_Toc29745902} 2.4.1 Wahl der Programmiersprachen und Arbeitsteilung {#wahl-der-programmiersprachen-und-arbeitsteilung .western align="JUSTIFY"}

Zum Programmieren haben wir hauptsächlich die Programmiersprache
„Python" verwendet. Die Hauptkriterien dafür waren die nicht zu
komplizierte Syntax, sodass alle Gruppenmitglieder mit der Software
umgehen können sowie die Kompatibilität mit Paketen zur Nutzung von
künstlicher Intelligenz. Trotz der simplen Syntax und der einfachen
Befehle wurde das Programmieren größtenteils von Frederik übernommen, da
dieser schon lange in Python programmiert und auch schon mit Software
wie Tensorflow und SciKit-Learn[^8^] gearbeitet hat. Während wir unsere
Software programmierten mussten wir außerdem häufiger auf weitere
Kenntnisse in anderen Programmiersprachen, wie Java, C++,
Designsprachen, wie HTML und Datenverarbeitungsprogramme, wie Matlab und
Excel zurückgreifen.

### []{#_Toc29745984}[]{#_Toc29745903} 2.4.2 Programmstruktur {#programmstruktur .western align="JUSTIFY"}

Der Übersichtlichkeit halber, haben wir unser Programm in
Subbibliotheken gegliedert, die jeweils einen Aufgabenbereich, wie z.B.
die KI-bezogenen Teile des Programms enthalten. Außerdem kann man so die
programmierten Klassen von mehreren Scripts aus verwenden. Die
letztendliche Programmabfolge befindet sich im Script
„api\_server.py"[^9^].

Dieses Script startet mehrere Prozesse, die untereinander kommunizieren
können. Außerdem erstellt und trainiert er den Random-Forest-Regressor
(RFR) mit zuvor aufgenommenen Daten. Sobald alle Prozesse gestartet, und
die RFRs trainiert sind, läuft das Script in einen Endlosschleife und
wartet auf eine Unterbrechung durch den Nutzer, woraufhin es alle
Subprozesse beenden kann.

Bei den gestarteten Prozessen handelt es sich genauer um einen
Stream-Prozess, der die ankommenden Daten vom Headset umwandelt und
speichert, sowie den API-Prozess. Der API-Prozess liest die letzten paar
Werte reagierend auf eine Web-Anfrage aus und analysiert sie dann mit
den zuvor im Hauptprozess erstellten RFRs. Das Ergebnis der Analyse wird
dann als ![][13] folgender Form über eine Web-Response zurückgegeben.

![][14]

Der Ablauf nachdem alle Prozesse gestartet wurden ist weiter in
folgender Visualisierung dargestellt:

[ ]{dir="LTR"
style="float: left; width: 6.25in; height: 0in; border: none; padding: 0in; background: #ffffff"}

[]{#_Toc29746105} *Abbildung 12 - Programmfunktion*

![][15]\
\

[ ]{dir="LTR"
style="float: left; width: 1.03in; height: 0.41in; border: none; padding: 0.05in 0.1in; background: #ffffff"}

Response

\
\

\
\

\
\

\
\

\
\

\
\

\
\

\
\

\
\

### []{#_Toc29745985}[]{#_Toc29745904} 2.4.3 Datensammlung und -verarbeitung {#datensammlung-und--verarbeitung .western align="JUSTIFY"}

Bei den Daten, die wir von unserem Headset empfangen handelt, es sich um
die Stärke fünf verschiedener Frequenzbänder für jede einzelne
Elektrode, die von der für Europa typischen Netzfrequenz (50 Hz), sowie
anderen typischen Störquellen bereinigt werden. Außerdem werden wir in
zukünftigen Versionen noch die Beschleunigungsdaten als Features für die
RFRs einbeziehen. Zum gegenwärtigen Zeitpunkt verwenden wir zum
Herausfiltern der Störungen und zur Umwandlung der Spannungswerte in
Frequenzbänder noch die OpenBCI-GUI Software, da sich eine direkte
Verbindung mit dem Board als überaus schwierig herausstellte. In
zukünftigen Versionen wird es hier jedoch auch eine Entwicklung geben.

Für das Sammeln der Trainingsdaten gibt es eine eigenes Script, in dem
man zuerst den aktuellen Zustand (bspw. 1000 = Gedanke: Arm hoch)
einträgt und dann solange der entsprechende Zustand besteht eine Taste
drückt. Das Script speichert die Aufnahmen nachdem es beendet wurde als
CSV-Datei im Unterverzeichnis „samples".

### []{#_Toc29745986}[]{#_Toc29745905} 2.4.4 Random-Forest-Regressor und Features {#random-forest-regressor-und-features .western align="JUSTIFY"}

Wie bereits mehrfach erwähnt, verwenden wir zur Auswertung der Daten den
in SciKit-Learn enthaltenen Random-Forest-Regressor[^10^]. Gründe dafür
sind, dass dieser sehr schnell trainiert werden kann und vielseitig
einsetzbar ist. Wir nutzen aktuell insgesamt 80 (*5 Bänder x 16 Kanäle*)
Features, von denen jedes eine gewöhnliche Float-Zahl ist, die die
Signalstärke eines Frequenzbandes an einer Elektrode abbildet. Trainiert
wird mit zuvor aufgenommenen Messwerten, die mit den gleichzeitigen
Zuständen verknüpft sind. Je nach zu erkennenden Gedanken, verwenden wir
zwischen 10.000 und 40.000 Messwertreihen. Die Aufnahme dieser Messwerte
erfolgt über ein eigenes Script[^11^], das die Daten dann im CSV-Format
abspeichert.

### []{#_Toc29745987}[]{#_Toc29745906} 2.4.5 Verwendete externe Bibliotheken {#verwendete-externe-bibliotheken .western align="JUSTIFY"}

Da wir nicht den gesamten Code für den Random-Forest-Regressor und die
Web-API schreiben konnten, haben wir externe Bibliotheken genutzt. Die
wichtigste ist SciKit-Learn, die vorgefertigten Tools für maschinelles
Lernen zur Verfügung stellt. Der Hauptvorteil ist hier, dass die
Bibliothek einfach eingebunden und benutzt werden kann. Des Weiteren
haben wir das API- und Web-Toolkit „Flask" bzw. „Flask Restful"
verwendet, um mit dem Programm kommunizieren zu können. Neben diesen
haben wir auch für Python-Projekte typische Bibliotheken, wie die
„Matplotlib", „Numpy", „Pandas" und „Scipy" verwendet, von denen
SciKit-Learn abhängig ist. Außerdem enthalten sie diverse Tools und
Visualisierungen. Alle verwendeten Bibliotheken sind in der Datei
„requirements.txt"[^12^] vermerkt und können von PyPi installiert
werden.

### []{#_Toc29745988}[]{#_Toc29745907} 2.4.6 Versionsverwaltung {#versionsverwaltung .western align="JUSTIFY"}

Das gemeinsame Arbeiten an Softwareprojekten erfordert ein
Versionsverwaltungssystem, um zum einen Änderungen der verschiedenen
Entwickler zu überblicken und zum anderen, um im Falle eines nicht zu
behebenden Fehlers zu vorherigen Version zurückzukehren. Aufgrund der
weiten Verbreitung und Mangel an Alternativen haben wir Git gewählt, mit
dem wir bereits zuvor gearbeitet hatten. Da wir unsere Konten bei GitHub
zu diesem Zeitpunkt bereits erstellt hatten, haben wir dort unser
Repository ohne großen Aufwand direkt erstellen können.

Wir haben die Software jedoch erst mit der auf unser neues Headset
ausgelegten Version auf GitHub gestellt.

### []{#_Toc29745989}[]{#_Toc29745908} 2.4.7 Vorherige Versionen {#vorherige-versionen .western align="JUSTIFY"}

Vor der aktuellen Version hatten wir noch ein Programm, das die Daten
unseres alten Headsets verarbeitete, jedoch noch nicht in der Lage war,
Gedanken zu erkennen. Mit dem Schreiben der neuen Version wurde die alte
vollständig gelöscht, da diese noch nicht konstruiert war, um wieder
verwendet zu werden. Außerdem haben wir unsere Python-Kenntnisse über
die Dauer des Projektes so erweitert, dass wir deutlich bessere Lösungen
fanden, um den Code zu kürzen und in mehreren Scripts zu verwenden.
![][16]![][17]

[]{#_Toc29745990}[]{#_Toc29745909} 2.5 Bau/Programmieren der Armprothese {#bauprogrammieren-der-armprothese .western}
------------------------------------------------------------------------

Ursprünglich hatten wir viele Pläne zum Bau einer Armprothese. Die
Armprothese sollte teils aus einem leicht zu bearbeitenden Material,
beispielsweise Messing und PLA (PLA ist das Filament, welches häufig von
FDM-Druckern verwendet wird), bestehen. Teilweise bestanden auch Pläne
für eine Hydraulik an den Fingern der Prothese, um ein kräftiges
Zugreifen zu gewährleisten.

Den Bau der Armprothese haben wir jedoch unter anderem auf Anraten von
Jugend-Forscht-Juroren vorerst zurückgestellt. Dafür gab es mehrere
Gründe. Zum einen stellte sich der Bau einer Armprothese, welche einem
echten Arm nahekommt, als sehr komplex dar. Da wir bisher auch nicht
genug Signale bekommen und verarbeiten können, um eine solche Prothese
zu steuern, ist der Bau einer solchen noch nicht von Nöten. Zum anderen
ist uns klar geworden, dass wir unser System nicht zwingend auf eine
Armprothese begrenzen müssen, sondern deutlich mehr Möglichkeiten haben,
beispielsweise die Steuerung einer Drohne. So trafen wir die
Entscheidung, vorerst nur eine virtuelle Armprothese zu programmieren
und für Jugend forscht ein kleines Demonstrationsmodell zu bauen.\
Dieses Demonstrationsmodell wird aus zwei Gelenken bestehen, welche
wiederum mit Stepper-Motoren angetrieben und von einem ESP8266
angesteuert werden. Die Datenübertragung läuft über das im ESP
integrierten WiFi-Modul. Die Signale, welche die KI ermittelt, werden
von einem in C++ geschriebenen Programm in Steuerungsbefehle
umgewandelt, welche wiederum analog auf die Motoren übertragen werden.

[]{#_Toc29745991}[]{#_Toc29745910}\
\

2.6 Grober zeitlicher Ablauf unserer Arbeit {#grober-zeitlicher-ablauf-unserer-arbeit .western style="page-break-before: always"}
-------------------------------------------

\
\

+----------------------+----------------------+----------------------+
| [*                   | **September &        | Ideenfindungsphase   |
| *2018**]{.underline} | Oktober**            |                      |
|                      |                      | Erkundung möglicher  |
|                      |                      | Hardware             |
|                      |                      |                      |
|                      |                      | Bestellen des        |
|                      |                      | OpenBCI-Ganglions    |
+----------------------+----------------------+----------------------+
| \                    | **November**         | Tests mit neu        |
|                      |                      | angekommener         |
|                      |                      | Hardware             |
|                      |                      |                      |
|                      |                      | Anmeldung für Jugend |
|                      |                      | forscht 2019         |
+----------------------+----------------------+----------------------+
| \                    | **Dezember**         | Programmieren der    |
|                      |                      | ersten               |
|                      |                      | Softwareversion (nur |
|                      |                      | Datenfilter)         |
|                      |                      |                      |
|                      |                      | Schreiben an der     |
|                      |                      | Langfassung          |
|                      |                      |                      |
|                      |                      | \                    |
+----------------------+----------------------+----------------------+
| [*                   | **Januar**           | Fertigstellung der   |
| *2019**]{.underline} |                      | Langfassung, erste   |
|                      |                      | Vorbereitungen für   |
|                      |                      | den Jugend forscht   |
|                      |                      | Wettkampf. Weiteres  |
|                      |                      | Ausfeilen der        |
|                      |                      | Software             |
+----------------------+----------------------+----------------------+
| \                    | **Februar**          | Intensive            |
|                      |                      | Vorbereitungen für   |
|                      |                      | den Jugend forscht   |
|                      |                      | Wettbewerb,          |
|                      |                      | Erstellen des        |
|                      |                      | Plakates.            |
|                      |                      |                      |
|                      |                      | Software             |
|                      |                      | „aufhübschen".       |
|                      |                      |                      |
|                      |                      | Jugend forscht       |
|                      |                      | Wettbewerb           |
+----------------------+----------------------+----------------------+
| \                    | **März**             | Überlegungen für     |
|                      |                      | Weiterentwicklung    |
|                      |                      | unseres Systems      |
|                      |                      |                      |
|                      |                      | -   16 oder 32       |
|                      |                      |     Kanäle?          |
|                      |                      |                      |
|                      |                      | Überlegungen,        |
|                      |                      | welches              |
|                      |                      | Mach                 |
|                      |                      | ine-Learning-Toolkit |
|                      |                      | verwendet werden     |
|                      |                      | soll und welche      |
|                      |                      | Daten es verarbeiten |
|                      |                      | soll.                |
+----------------------+----------------------+----------------------+
| \                    | **April**            | Treffen der          |
|                      |                      | endgültigen          |
|                      |                      | Entscheidungen zur   |
|                      |                      | weiteren             |
|                      |                      | Verfahrensweise      |
+----------------------+----------------------+----------------------+
| \                    | **Mai**              | Noah Ihlein tritt    |
|                      |                      | dem Projekt bei,     |
|                      |                      | wird eingeführt.     |
|                      |                      |                      |
|                      |                      | Antrag für ein       |
|                      |                      | Sponsoring von       |
|                      |                      | OpenBCI wird         |
|                      |                      | gestellt, leider     |
|                      |                      | ohne Antwort.        |
+----------------------+----------------------+----------------------+
| \                    | **Juni**             | Beantragung von      |
|                      |                      | Mikro-Makro-MINT     |
|                      |                      |                      |
|                      |                      | Beginn mit dem       |
|                      |                      | Programmieren der    |
|                      |                      | Software             |
+----------------------+----------------------+----------------------+
| \                    | **Juli**             | Weiterentwicklung    |
|                      |                      | der Software.        |
+----------------------+----------------------+----------------------+
| \                    | **August**           | Weiterentwicklung    |
|                      |                      | der Software.        |
|                      |                      |                      |
|                      |                      | Warten auf           |
|                      |                      | Bestätigung von      |
|                      |                      | Mikro-Makro-MINT     |
+----------------------+----------------------+----------------------+
| \                    | **September**        | Bestätigung von      |
|                      |                      | Mikro-Makro-MINT     |
|                      |                      |                      |
|                      |                      | Bestellen der        |
|                      |                      | Hardware             |
+----------------------+----------------------+----------------------+
| \                    | **Oktober**          | Weiterentwicklung    |
|                      |                      | der Software, Bau    |
|                      |                      | des Headsets mit     |
|                      |                      | OpenBCI „Cyton"      |
+----------------------+----------------------+----------------------+
| \                    | **November**         | Weiterentwicklung    |
|                      |                      | der Software         |
|                      |                      |                      |
|                      |                      | Anmeldung für Jugend |
|                      |                      | forscht              |
+----------------------+----------------------+----------------------+
| \                    | **Dezember**         | Zusätzlich zum       |
|                      |                      | OpenBCI „Cyton"      |
|                      |                      | erhalten wir das     |
|                      |                      | „Daisy", eine        |
|                      |                      | Erweiterung von 8    |
|                      |                      | auf 16 Kanäle findet |
|                      |                      | statt                |
|                      |                      |                      |
|                      |                      | Erweiterung der      |
|                      |                      | Software             |
|                      |                      |                      |
|                      |                      | Schreiben der        |
|                      |                      | Langfassung          |
+----------------------+----------------------+----------------------+
| [*                   | **Januar**           | Erweiterung der      |
| *2020**]{.underline} |                      | Software/Trainieren  |
|                      |                      | der KI auf drei      |
|                      |                      | verschiedene         |
|                      |                      | Zustände             |
|                      |                      |                      |
|                      |                      | Fertigstellung der   |
|                      |                      | Langfassung          |
+----------------------+----------------------+----------------------+

[]{#_Toc29745992}[]{#_Toc29745911} **3. Probleme** {#probleme .western align="JUSTIFY"}
==================================================

Leider läuft nicht immer alles wie geplant, immer wieder hatten und
haben wir mit verschiedenen Problemen zu kämpfen, die den
Projektfortschritt gefährdeten.

### []{#_Toc29745993}[]{#_Toc29745912} 3.1 Hardware {#hardware .western align="JUSTIFY"}

Im Hardwarebereich gab es die meisten und schwierigsten Probleme. So gab
es oft Verbindungsprobleme zwischen Board und Dongle. Ein anderes
Problem waren die bereits erwähnten Störsignale, welche durch
verschiedene elektrische Geräte im Raum verursacht wurden. Ein Beispiel
hierfür ist ein kaputtes Netzteil eines Computers. Durch diese Fehler
kamen viele Stunden des Ausprobierens und der Fehlersuche zustande.

Größere Probleme hatten wir auch als das Headset ausgedruckt werden
sollte. Dieses war zu groß um in den uns zur Verfügung stehenden
Druckern ausgedruckt werden können. Der Versuch, das Headset in
getrennten kleineren Stücken auszudrucken ist fehlgeschlagen. Das
Problem wurde letztendlich dadurch gelöst, dass das Headset von einem
Freund in einem größeren FDM-Drucker ausgedruckt wurde.

### []{#_Toc29745994}[]{#_Toc29745913} 3.2 Software {#software .western align="JUSTIFY"}

Auch softwaretechnisch gab es immer wieder Probleme, zu denen
hauptsächlich Bugs in der von OpenBCI zur Verfügung gestellten
GUI-Software zählten, weshalb wir mehrfach auf ältere Versionen
zurückgreifen mussten. Aufgrund dieser Unzuverlässigkeit planen wir, in
zukünftigen Versionen eine direkte Verbindung zwischen Headset und
Computer herzustellen

### []{#_Toc29745995}[]{#_Toc29745914} 3.3 Sonstiges {#sonstiges .western align="JUSTIFY"}

Abgesehen von den technischen Problemen hatten wir aufgrund der langen
Lieferzeiten unserer Boards und der Bewerbungszeit für die
Mikro-Makro-Mint-Unterstützung zwischenzeitlich sehr lange Wartezeiten,
in welchen wir nicht effektiv arbeiten konnten. Da sich alle
Gruppenmitglieder nun in der zwölften Stufe der Schule befinden, müssen
wir uns auch immer mehr mit dem regulären Schulstoff beschäftigen, was
dazu führt, dass wir uns teilweise nicht in dem Maße mit unserem Projekt
beschäftigen konnten, wie wir es gerne getan hätten.

[]{#_Toc29745996}[]{#_Toc29745915} **4. Zukunftspläne** {#zukunftspläne .western}
=======================================================

Wir hoffen, dass wir unser System auch nach Jugend forscht
weiterentwickeln können. Dafür benötigen wir vor allem bessere Hardware,
was einen hohen Kostenaufwand bedeutet.

Mit verbesserter Hardware könnten wir die KI auf noch mehr Zustände
trainieren und somit dann eine richtige Armprothese ansteuern, welche es
sich dann endlich zu bauen lohnt.

[]{#_Toc29745997}[]{#_Toc29745916} **5. Ergebnisdiskussion** {#ergebnisdiskussion .western align="JUSTIFY"}
============================================================

Wir haben es geschafft unser System so zu entwickeln, dass verschiedene
Hirnströme voneinander unterschieden werden können. Es bleibt ein großes
Entwicklungsfeld, dies auf Normalbedingungen mit Bewegung und
verschiedenen Tätigkeiten auszuweiten und auf verschiedene Geräte, wie
Armprothesen, zu übertragen. Ungeklärt ist, wie viele unterschiedliche
Signale maximal gemessen und interpretiert werden können, da man mit
einem EEG-Gerät nur die Hirnströme der obersten 2cm der Großhirnrinde
ableiten kann und die Messdaten insgesamt nicht genau genug sind. Die
Lösung für dieses Problem könnte in einem noch besseren EEG-Gerät mit
noch mehr Kanälen liegen.

\
\

\
\

\
\

[]{#_Toc29745998}[]{#_Toc29745917} **6.** **Zusammenfassung** {#zusammenfassung .western align="JUSTIFY"}
=============================================================

Das von uns entwickelte System lässt sich in der Theorie auf viele
verschiedene Bereiche anwenden, die weit über eine Armprothese
hinausgehen. Durch unsere lange Planungsphase waren wir in der Lage,
unsere weitere Vorgehensweise nach Jugend forscht 2019 zu diskutieren
und nach Lösungen für Probleme suchen. Durch unseren Wechsel auf 16
Kanäle und die Anwendung des 10-20-Systems konnten wir eine deutlich
höhere Messgenauigkeit erreichen als wir ursprünglich mit unserem
Ganglion-Board mit vier Kanälen hatten. Wir haben es geschafft, ein
Programm zu entwickeln, welches zuverlässig die Daten des EEG-Gerätes
aufnehmen und so weiterverarbeiten kann, dass eine von uns trainierte KI
diese erkennt, verarbeitet und entsprechende Signale an das
angeschlossene Gerät, dem Demonstrationsmodell, leitet.

Da wir in der Lage sind, mehr als zwei verschiedene Zustände im Gehirn
mit unserem EEG-Gerät zu erkennen, haben wir die Erwartungen vieler,
einschließlich unserer eigener, übertroffen. Das System kann von nun an
primär durch eine Verbesserung der Hardware-Komponenten weiterentwickelt
werden, wozu uns allerdings vor allem die finanziellen Mittel fehlen.

Alles in allem ist unser Projekt in jeder Hinsicht ein Erfolg. Wir
hoffen darauf, dass wir das von uns entwickelte System trotz
verschiedenster Hürden weiterentwickeln können und in Zukunft eine
richtige Armprothese ansteuern können.

[]{#_Toc29745999}[]{#_Toc29745918} **7. Danksagung** {#danksagung .western align="JUSTIFY"}
====================================================

Danken möchten wir allen, die es uns ermöglichen unsere Idee zu
verwirklichen. Vor allem danken wir Dr. Joachim Groß, Lehrer und Leiter
des Schülerforschungszentrums in Eningen unter Achalm für die Betreuung
und das finanzielle Management unseres Projekts.

Vielen Dank auch an Simon Benezan für die Hilfe unser Headset mit dem
3D-Drucker auszudrucken.

Außerdem danken wir unseren Eltern, die uns über die Dauer des ganzen
Projektes unterstützt haben.

Des Weiteren danken wir der Baden-Württemberg Stiftung für die
finanzielle Unterstützung innerhalb des Mikro-Makro-MINT-Programmes.

\
\

[]{#_Toc29746000}[]{#_Toc29745919} **8. Abbildungs- und Quellenverzeichnis** {#abbildungs--und-quellenverzeichnis .western align="JUSTIFY" style="page-break-before: always"}
============================================================================

[]{#_Toc29746001}[]{#_Toc29745920} 8.1 Abbildungen {#abbildungen .western}
--------------------------------------------------

::: {#Illustration Index1 dir="LTR"}
\
:::

[]{#_Toc29746002}[]{#_Toc29745921}\
\

\
\

8.2 Quellen/Literatur {#quellenliteratur .western style="margin-bottom: 0.17in; page-break-before: always"}
---------------------

STÖHR, Manfred; KRAUS, Regina: Einführung in die klinische
Neurophysiologie. EMG-EEG-Evozierte Potenziale. Steinkopff Verlag
Darmstadt, 2014.

\
\

HERRMANN, Björn: Methoden der kognitiven Neurowissenschaften --
Elektroenzephalographie. Leipzig, Deutschland Mai 2014, entnommen am
02.01.2019.

\
\

BERTSCH, Katja: Das EEG: Spontan-EEG und EKP, Trier, Deutschland
Dezember 2007, entnommen am 07.12.2018.

\
\

KÜBLER, Andrea und NEUPER, Christa: Gehirn-Computer-Schnittstellen
(Brain-Computer Interfaces): Anwendungen und Perspektiven, entnommen am
02.01.2019 --
<https://www.degruyter.com/view/j/nf.2008.14.issue-2/nf-2008-0205/nf-2008-0205.xml>

\
\

OpenBCI Documentation, entnommen im Oktober 2019 --

<https://docs.openbci.com/docs/Welcome.html>

\
\

OpenBCI GUI, entnommen im Oktober 2019 (Version 4.1.3) --

<https://docs.openbci.com/docs/06Software/01-OpenBCISoftware/GUIDocs>

::: {#sdfootnote1}
[1]^^ Vgl.: STÖHR, Manfred; KRAUS, Regina: Einführung in die klinische
Neurophysiologie.
:::

::: {#sdfootnote2}
[2]^^ Vgl.: ebd.
:::

::: {#sdfootnote3}
[3]^^ Vgl.: ebd.
:::

::: {#sdfootnote4}
[4]^^ Vgl.: ebd.
:::

::: {#sdfootnote5}
[5]^^ Vgl.: ebd.
:::

::: {#sdfootnote6}
[6]^^ Vgl.: STÖHR, Manfred; KRAUS, Regina: Einführung in die klinische
Neurophysiologie.
:::

::: {#sdfootnote7}
[7]^^ Vgl. ebd.
:::

::: {#sdfootnote8}
[8]^^ SciKit-Learn: <https://scikit-learn.org>
:::

::: {#sdfootnote9}
[9]^^[ Main-Script:
<https://github.com/sfz-eningen/NeuroCTRL/blob/master/api_server.py>]{lang="en-US"}
:::

::: {#sdfootnote10}
[10]^^[ Random-Forest-Regressor -]{lang="en-US"}

[<https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html>]{lang="en-US"}

[<https://github.com/sfz-eningen/NeuroCTRL/blob/master/AI/classes.py>]{lang="en-US"}
:::

::: {#sdfootnote11}
[11]^^[ "record.py" -
<https://github.com/sfz-eningen/NeuroCTRL/blob/master/record.py>]{lang="en-US"}
:::

::: {#sdfootnote12}
[12]^^[ PyPi Requirements -
<https://github.com/sfz-eningen/NeuroCTRL/blob/master/requirements.txt>]{lang="en-US"}
:::

::: {type="FOOTER"}
+---+---+---+
| \ | \ | \ |
+---+---+---+

\
:::

  [1]: eadbd800ece7491b3980a99de41c9c68_html_2dfc11bf.jpg {width="305"
  height="229"}
  [2]: eadbd800ece7491b3980a99de41c9c68_html_f7351819.jpg {width="343"
  height="229"}
  [3]: eadbd800ece7491b3980a99de41c9c68_html_9cb785b0.jpg {width="327"
  height="246"}
  [4]: eadbd800ece7491b3980a99de41c9c68_html_5bb9a16b.png {width="235"
  height="185"}
  [^1^]: #sdfootnote1sym {#sdfootnote1anc .sdfootnoteanc}
  [^2^]: #sdfootnote2sym {#sdfootnote2anc .sdfootnoteanc}
  [^3^]: #sdfootnote3sym {#sdfootnote3anc .sdfootnoteanc}
  [^4^]: #sdfootnote4sym {#sdfootnote4anc .sdfootnoteanc}
  [^5^]: #sdfootnote5sym {#sdfootnote5anc .sdfootnoteanc}
  [5]: eadbd800ece7491b3980a99de41c9c68_html_8974670a.png {width="309"
  height="358"}
  [^6^]: #sdfootnote6sym {#sdfootnote6anc .sdfootnoteanc}
  [^7^]: #sdfootnote7sym {#sdfootnote7anc .sdfootnoteanc}
  [6]: eadbd800ece7491b3980a99de41c9c68_html_1f3818d2.png {width="224"
  height="236"}
  [7]: eadbd800ece7491b3980a99de41c9c68_html_938126e3.jpg {width="261"
  height="261"}
  [8]: eadbd800ece7491b3980a99de41c9c68_html_26c29778.png {width="1"
  height="1"}
  [9]: eadbd800ece7491b3980a99de41c9c68_html_e60dad19.jpg {width="292"
  height="259"}
  [10]: eadbd800ece7491b3980a99de41c9c68_html_f7351819.jpg {width="293"
  height="196"}
  [11]: eadbd800ece7491b3980a99de41c9c68_html_1f6da567.gif
  [12]: eadbd800ece7491b3980a99de41c9c68_html_2633df98.jpg {width="274"
  height="205"}
  [^8^]: #sdfootnote8sym {#sdfootnote8anc .sdfootnoteanc}
  [^9^]: #sdfootnote9sym {#sdfootnote9anc .sdfootnoteanc}
  [13]: eadbd800ece7491b3980a99de41c9c68_html_6048b34c.gif
  [14]: eadbd800ece7491b3980a99de41c9c68_html_60b4dc6e.gif
  [15]: eadbd800ece7491b3980a99de41c9c68_html_413bae35.gif
  [^10^]: #sdfootnote10sym {#sdfootnote10anc .sdfootnoteanc}
  [^11^]: #sdfootnote11sym {#sdfootnote11anc .sdfootnoteanc}
  [^12^]: #sdfootnote12sym {#sdfootnote12anc .sdfootnoteanc}
  [16]: eadbd800ece7491b3980a99de41c9c68_html_f2c20ace.png {width="1"
  height="1"}
  [17]: eadbd800ece7491b3980a99de41c9c68_html_aced5dd6.png {width="1"
  height="1"}
  [1]: #sdfootnote1anc {#sdfootnote1sym .sdfootnotesym}
  [2]: #sdfootnote2anc {#sdfootnote2sym .sdfootnotesym}
  [3]: #sdfootnote3anc {#sdfootnote3sym .sdfootnotesym}
  [4]: #sdfootnote4anc {#sdfootnote4sym .sdfootnotesym}
  [5]: #sdfootnote5anc {#sdfootnote5sym .sdfootnotesym}
  [6]: #sdfootnote6anc {#sdfootnote6sym .sdfootnotesym}
  [7]: #sdfootnote7anc {#sdfootnote7sym .sdfootnotesym}
  [8]: #sdfootnote8anc {#sdfootnote8sym .sdfootnotesym}
  [9]: #sdfootnote9anc {#sdfootnote9sym .sdfootnotesym}
  [10]: #sdfootnote10anc {#sdfootnote10sym .sdfootnotesym}
  [11]: #sdfootnote11anc {#sdfootnote11sym .sdfootnotesym}
  [12]: #sdfootnote12anc {#sdfootnote12sym .sdfootnotesym}
