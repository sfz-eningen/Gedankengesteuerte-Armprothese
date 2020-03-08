Gedankengesteuerte Armprothese
Ein Projekt von Frederik Beimgraben, Noah Ihlein und Maximilian Menzel

Kurzfassung
Das Ziel unserer Arbeit ist, mithilfe eines EEG-Gerätes ein Programm (z.B. eine virtuelle - später reale Armprothese) mit zwei oder mehr Variablen anzusteuern. So könnten billige Prothesen hergestellt werden, welche sehr gut funktionieren, gleichzeitig aber ohne Operationen einsetzbar sind.
Unsere Arbeit setzt sich aus dem Bau eines EEG-Gerätes und dem Programmieren von Software, welche die Daten des EEG-Gerätes verarbeiten kann, zusammen. Des Weiteren entstehen eine virtuelle Armprothese und ein Programm, welches diese aus den verarbeiteten Daten des EEG-Gerätes ansteuert.
Seit Jugend forscht 2019 haben wir ein neues EEG-Gerät gebaut und die Software erweitert und verfeinert. Mithilfe von neuronalen Netzen können die Daten des EEG-Gerätes trotz der hohen Komplexität erkannt werden.
  
Inhalt
1. Einleitung	3
1.1 Ideenfindung	3
1.2 Wie möchten wir unser Vorhaben realisieren?	3
2. Vorgehensweise, Materialien und Methodik	4
2.1 Unsere Arbeitsweise	4
2.2 Funktionsweise eines EEG-Gerätes	4
2.2.1 Allgemeines	4
2.2.2 Platzierung der Elektroden	5
2.3 Bau und Aufbau des EEG-Gerätes	6
2.4 Entwicklung und Funktion der Software	8
2.4.1 Wahl der Programmiersprachen und Arbeitsteilung	8
2.4.2 Programmstruktur	8
2.4.3 Datensammlung und -verarbeitung	9
2.4.4 Random-Forest-Regressor und Features	9
2.4.5 Verwendete externe Bibliotheken	9
2.4.6 Versionsverwaltung	9
2.4.7 Vorherige Versionen	10
2.5 Bau/Programmieren der Armprothese	10
2.6 Grober zeitlicher Ablauf unserer Arbeit	11
3. Probleme	12
3.1 Hardware	12
3.2 Software	12
3.3 Sonstiges	12
4. Zukunftspläne	12
5. Ergebnisdiskussion	12
6. Zusammenfassung	13
7. Danksagung	13
8. Abbildungs- und Quellenverzeichnis	14
8.1 Abbildungen	14
8.2 Quellen/Literatur	15

 
1. Einleitung

	Ideenfindung
Zu Beginn des letzten Schuljahres überlegten wir uns ein Projekt, an welchem wir im Schülerforschungszentrum arbeiten wollten. Wir haben uns verschiedene Problembereiche angesehen und wir haben gemerkt, dass wir gerne etwas machen möchten, was sowohl mit Menschen als auch mit Technik zu tun hat. Durch Zufall hat Frederik EEG-Geräte und deren Einsatzbereiche im Internet kennengelernt. Durch Recherche haben wir entdeckt, dass voll funktionsfähige (Arm-) Prothesen bisher nur unter speziellen Bedingungen einsetzbar sind. So müssen beispielsweise bei einem Unfall mit Verlust eines Armes die Nervenenden im Arm intakt bleiben, damit eine Prothese angeschlossen werden kann. Des Weiteren werden große Operationen fällig, um eine spezielle, extra angefertigte Armprothese mit dem Körper und Gehirn zu verbinden. All dies ist natürlich auch mit hohen Kosten verbunden. So haben wir uns dazu entschlossen, eine Armprothese zu bauen, welche mit den Möglichkeiten eines EEG-Gerätes arbeitet. Dadurch sollen alle bestehenden Probleme gelöst werden. In den letzten Monaten ist uns bewusst geworden, dass wir unser System nicht nur auf Armprothesen, sondern auf jede beliebige Art von elektrotechnischen Geräten übertragen können, beispielsweise Drohnen. 

	Wie möchten wir unser Vorhaben realisieren?
Die Möglichkeit unser Projekt zu realisieren, bekommen wir durch das Schülerforschungszentrum in Eningen. Wir erhalten dort neben finanzieller Unterstützung auch Beratung von Lehrern. Außerdem werden wir finanziell durch das Mikro-Makro-MINT-Programm in Baden-Württemberg unterstützt. Des Weiteren haben wir Zugriff auf eine Werkstatt, Computer und auch einen 3D-Drucker. Uns stehen verschiedenste Arbeitsmaterialen zur Verfügung. Aufgaben, wie z.B. Programmieren oder Planung betreiben wir aufgrund des hohen Zeitaufwandes nicht nur im SFZ, sondern auch in der Schule, oder Zuhause über Online-Sprachchats. Durch Open-Source Projekte, wie OpenBCI erhalten wir einigermaßen kostengünstigen Zugriff auf EEG-Hardware und haben die Möglichkeit, deren Firmware einfach zu bearbeiten und schnell passende Software zu programmieren. Mithilfe des EEG-Gerätes möchten wir unsere Hirnströme während bestimmter Gedanken messen, um später mit diesen die Prothese anzusteuern. Die Daten des EEG-Gerätes werden von einer eigens programmierten Software geordnet. Mit diesen Daten kann dann ein neuronales Netz trainiert werden, das bereits trainierte und wiederholt auftretende Muster erkennen kann. Die Ergebnisse des neuronalen Netzes können schließlich zur Steuerung der Prothese genutzt werden. Da wir aktuell keinen Zugriff auf eine hochentwickelte bewegliche Armprothese haben, werden wir zunächst eine simulierte Armprothese oder ein Demonstrationsmodell steuern.

 
2. Vorgehensweise, Materialien und Methodik

2.1 Unsere allgemeine Vorgehensweise
Zu Beginn unseres Projekts haben wir hauptsächlich jede Woche freitags im Schüler-Forschungs-Zentrum in Eningen gearbeitet. Dort haben wir Zugriff auf eine voll ausgestattete Werkstadt, Computer, 3D-Drucker und Arbeitsmaterialien. Nachteil ist dabei die lange An- und Abfahrtszeit, welche insgesamt über zwei Stunden dauert. Über viele Wochen hinweg hat sich die Arbeit immer weiter nach Hause oder auf freie Zeiten in der Schule verlagert. Vor allem beim Programmieren der Software waren wir nicht auf das SFZ angewiesen, über das Projektmanagement-Tool „Git“ konnten wir alle immer den aktuellen Code auf unsere Computer/Laptops laden. Über das Sprachchat-Programm Discord konnten wir miteinander kommunizieren. Mithilfe von TeamViewer konnten wir auf die Computer des anderen zugreifen und live sehen, was auf dem Bildschirm angezeigt wird. Dies war besonders nützlich, wenn Frederik, Maximilian oder Noah beim Programmieren geholfen hat. Aktuell arbeiten wir circa die Hälfte der Zeit von zu Hause aus. Unser Betreuer im SFZ hat es uns möglich gemacht, einen Schlüssel für das Gebäude zu bekommen, wodurch wir nicht mehr an Freitage gebunden sind und jederzeit das SFZ aufsuchen können. So ist ein Mix aus verschiedenen Arbeitsstandorten entstanden, was vor allem unsere Produktivität stark gefördert hat.
2.2 Funktionsweise eines EEG-Gerätes
2.2.1 Allgemeines
Ein EEG-Gerät (Elektroenzephalographie-Gerät) wurde bereits im Jahr 1929 durch H. Berger entwickelt und wird bis heute beispielsweise bei der Hirntoddiagnostik oder der Diagnose von Epilepsien eingesetzt . Es wird dabei die Spannungsdifferenz zwischen zwei Elektroden gemessen bzw. abgeleitet . Das OpenBCI-System ist auf eine sogenannte Referenzableitung bzw. unipolare Referenzschaltung ausgelegt. Das bedeutet, dass die spannungsaktiven Elektroden auf dem Kopf mit einer elektrisch inaktiven Referenzelektrode verglichen werden . Diese kann mittig auf dem Kopf oder am Ohr platziert werden . Theoretisch könnte man die Referenzelektrode auch unterhalb des Kopfes anbringen, dabei bekäme man allerdings Probleme mit sogenannten Artefakten . Artefakte sind Messdaten, die nicht durch Hirnaktivität entstehen, beispielsweise durch die Bewegung eines Armes oder statische Ladungen, welche unter anderem durch Reibung des Arms auf einem Pullover entstehen können. Wir haben aus diesem Grund unsere Referenzelektroden am Ohr platziert. Eigentlich ist vorgesehen, dass je Gehirnhälfte eine Referenzelektrode getragen wird, allerdings hatte das OpenBCI-System Probleme mit dem Erkennen von zwei Ohrelektroden. Deshalb haben wir beschlossen diese zusammenzuschließen und nun gemeinsam für alle Elektroden auf dem Kopf zu verwenden. Der Vorteil in der unipolaren Referenzschaltung liegt darin, dass die Amplituden der einzelnen Ableitpunkte besser miteinander zu vergleichen sind bzw. einzeln ausgegeben werden, was für die Funktion der künstlichen Intelligenz (KI) besser ist. Der Nachteil liegt darin, dass Artefakte häufiger und stärker auftreten können. Da wir uns beim Trainieren der KI so wenig wie möglich bewegen, sollte dies dabei allerdings kaum ein Problem darstellen. Bei einer späteren Verwendung wird die KI Artefakte größtenteils ignorieren, da immer mehrere Datenreihen gleichzeitig verarbeitet werden.
2.2.2 Platzierung der Elektroden
Je weiter die Elektroden auf dem Kopf voneinander entfernt sind, desto höher sind die Spannungsdifferenzen . Aus diesem Grund sollten die Elektroden alle ungefähr denselben Abstand voneinander haben. Von OpenBCI wird für die Platzierung der Elektroden das 10-20-System nach Jaspers  vorgeschlagen, welches international gültig ist. Nach einigen Recherchen haben wir uns dazu entschieden, dieses System so zu übernehmen, da für uns so die genausten Ableitungen möglich sind. Das 10-20-System bekommt seinen Namen durch die Art und Weise wie die Elektroden auf dem Kopf platziert werden. So wird der Kopf in Prozentabschnitte aufgeteilt. Dies findet im Groben zum einen vom Nasion zum Inion statt, zum anderen vom linken bis zum rechten Ohr. Die Elektroden werden nun vom ausgehend Nasion in Richtung der Ohren bis zum Inion verteilt. Dies geschieht zuerst in einem Abschnitt von 10%, anschließend vier Mal 20% und zu guter Letzt noch einmal 10%. So kommen je Kopfseite (rechts und links) 100% zusammen. Dasselbe geschieht bei den Elektroden, die vom Nasion über den Kopf Richtung Inion platziert werden. Genauso verfährt man bei den Elektroden, die vom linken zum rechten Ohr verteilt werden. Die CZ, T7, und T8-Elektroden werden dabei mehrfach bedacht. Zwischen diesen Elektroden können im Abstand von 10% oder 20% weitere Elektroden platziert werden. Wir haben Elektroden an folgenden Positionen platziert und als beistehenden Kanal festgelegt (Hierbei steht F = frontal, Z = Zentral, T = temporal, P = parietal, O = okzipital, K = Kanal auf Board): Fp1-K1, Fp2-K2, F7-K9, F8-K10, T7-K13, T8-K14, P7-K5, P8-K6, O1-K7, O2-K8, F3-K11, F4-K12, C3-K3, C4-K4, P3-K15, P4-K16. Unsere Elektroden sind also um den Kopf herum und auf halber Höhe zwischen Ohren und der Oberseite des Kopfes angebracht: 
2.3 Bau und Aufbau des EEG-Gerätes
Seit Beginn unseres Projektes haben wir zwei verschiedene EEG-Geräte gebaut.
Das erste EEG-Gerät war ein einfaches Ganglion-Board mit vier Kanälen von OpenBCI, einem amerikanischen Unternehmen, dass sich mit der Entwicklung von EEG-Geräten beschäftigt und gleichzeitig entsprechende Bauteile verkauft. Wir bestellten uns das OpenBCI Ganglion-Board, Goldelektroden und Ten20-Leitpaste. Der Zusammenbau dieser Teile gestaltete sich als sehr einfach und es wurde zusätzlich nur eine Kappe zum Anbringen der Elektroden am Kopf, ein Gehäuse für das Board und eine Klammer benötigt, um die Referenzelektrode am Ohr zu befestigen. Wir haben das OpenBCI Ganglion gewählt, da es nicht allzu teuer, aber modifizierbar ist und ebenfalls viel frei verfügbarer Code zur Ansteuerung vorhanden ist. Jeder Teil der Firmware ist frei verfügbar und da auch die Pläne zum Herstellen der Boards dabei sind, könnten wir später mit unserem Code kompatible Boards mit mehr Kanälen selbst herstellen. Dies haben wir jedoch unterlassen, da es nicht sehr einfach ist, die Boards selbst herzustellen und wir Sorge hatten, dass darauf die Software möglicherweise nicht funktioniert. 
Nachdem wir mit diesem EEG-Gerät in der Lage waren, Hirnströme auszulesen und mit unserer damaligen Software zu verarbeiten, wurde uns bewusst, dass wir mit vier Kanälen nicht genug Daten sammeln können, um dauerhaft zuverlässig Messwerte zu bekommen. Aus diesem Grund wollten wir unser System auf ganze 32 Kanäle erweitern. Dies wäre jedoch ein zu großer Schritt gewesen, da man bereits mit 16 Kanälen sehr gut die von uns gewollte Messgenauigkeit erreichen kann. Daher haben wir uns dazu entschieden vorerst nur auf 16 Kanäle zu erweitern. Die neuen Boards kamen wieder von OpenBCI, zum einen das „Cyton“-Board mit 8 Kanälen und dem „Daisy“-Board, eine Erweiterung für das „Cyton”-Board mit 8 Kanälen. Da wir nun mit einer deutlich höheren Anzahl an Elektroden arbeiteten, konnten wir die Elektroden nicht mehr einzeln an die Kopfhaut drücken. Somit musste ein richtiger „Helm“ hergestellt werden, an dem die Elektroden befestigt werden konnten. Das EEG-Gerät wird von vier Handelsüblichen AA-Batterien betrieben und ist in keiner Weise an das Stromnetz angeschlossen.

 
Unser zweites EEG-Gerät besteht zu rund 70% aus Teilen, die mit dem 3D-Drucker angefertigt wurden. Die dafür benötigten Modelle sind über die Webseite von OpenBCI frei verfügbar. Nachdem wir das Grundgerüst für das EEG-Gerät hatten drucken lassen, mussten wir darin die Elektrodenhalterungen befestigen. Durch Epoxidharz bekamen diese einen festen Halt. Die Goldelektroden haben wir vorerst an der Außenseite der großen Schrauben befestigt und durch sie hindurch mit einer weiteren Metallschraube mit der speziell beschichteten Trockenelektrode verbunden. Hierbei ergab sich allerdings das Problem, dass die Leitfähigkeit der Metallschrauben weit unter dem erwarteten Wert lag, weshalb die Messwerte zu ungenau waren und viele Störsignale auftraten. Aus diesem Grund haben wir die Elektrodenhalter und Elektroden so umplatziert, dass die Goldelektrode direkt an der Trockenelektrode festgeschraubt wird. Dadurch erhalten wir nun deutlich genauere Messwerte. Für diesen Schritt kam uns zugute, dass es einfach war, die Elektroden vom Headset zu entfernen und in Einzelteile zu zerlegen. Nachdem die Goldelektrode umplatziert war, konnte man alles schnell und einfach wieder zusammenbauen.


Die in Abb. 01 dargestellten Elektroden bestehen aus einem Elekrodenhalter (2), der leitend beschichteten Elektrode (1) und der Goldelektrode (3), mit dem damit verbundenen Kabel.                           In Abb. 0-2 ist das ganze Headset mit den montierten Boards zu sehen. Bei diesem handelt es sich um das von OpenBCI frei zur Verfügung gestellte „Ultracortex Mark IV“ Headset. Die Platzierung der Elektroden erfolgt über das bereits erwähnte für elelektroenzephalographische Messungen typische 10-20-Prinzip, mit dem sich Reaktionen am besten ableiten lassen. 


 
2.4 Entwicklung und Funktion der Software
2.4.1 Wahl der Programmiersprachen und Arbeitsteilung
Zum Programmieren haben wir hauptsächlich die Programmiersprache „Python“ verwendet. Die Hauptkriterien dafür waren die nicht zu komplizierte Syntax, sodass alle Gruppenmitglieder mit der Software umgehen können sowie die Kompatibilität mit Paketen zur Nutzung von künstlicher Intelligenz. Trotz der simplen Syntax und der einfachen Befehle wurde das Programmieren größtenteils von Frederik übernommen, da dieser schon lange in Python programmiert und auch schon mit Software wie Tensorflow und SciKit-Learn  gearbeitet hat.  Während wir unsere Software programmierten mussten wir außerdem häufiger auf weitere Kenntnisse in anderen Programmiersprachen, wie Java, C++, Designsprachen, wie HTML und Datenverarbeitungsprogramme, wie Matlab und Excel zurückgreifen.
2.4.2 Programmstruktur
Der Übersichtlichkeit halber, haben wir unser Programm in Subbibliotheken gegliedert, die jeweils einen Aufgabenbereich, wie z.B. die KI-bezogenen Teile des Programms enthalten. Außerdem kann man so die programmierten Klassen von mehreren Scripts aus verwenden. Die letztendliche Programmabfolge befindet sich im Script „api_server.py“ .  
Dieses Script startet mehrere Prozesse, die untereinander kommunizieren können. Außerdem erstellt und trainiert er den Random-Forest-Regressor (RFR) mit zuvor aufgenommenen Daten. Sobald alle Prozesse gestartet, und die RFRs trainiert sind, läuft das Script in einen Endlosschleife und wartet auf eine Unterbrechung durch den Nutzer, woraufhin es alle Subprozesse beenden kann. 
Bei den gestarteten Prozessen handelt es sich genauer um einen Stream-Prozess, der die ankommenden Daten vom Headset umwandelt und speichert, sowie den API-Prozess. Der API-Prozess liest die letzten paar Werte reagierend auf eine Web-Anfrage aus und analysiert sie dann mit den zuvor im Hauptprozess erstellten RFRs. Das Ergebnis der Analyse wird dann als dict folgender Form über eine Web-Response zurückgegeben. 
{"data\"": [Ergebnis1,…,ErgebnisN]}
 Der Ablauf nachdem alle Prozesse gestartet wurden ist weiter in folgender Visualisierung dargestellt:










2.4.3 Datensammlung und -verarbeitung
Bei den Daten, die wir von unserem Headset empfangen handelt, es sich um die Stärke fünf verschiedener Frequenzbänder für jede einzelne Elektrode, die von der für Europa typischen Netzfrequenz (50 Hz), sowie anderen typischen Störquellen bereinigt werden. Außerdem werden wir in zukünftigen Versionen noch die Beschleunigungsdaten als Features für die RFRs einbeziehen. Zum gegenwärtigen Zeitpunkt verwenden wir zum Herausfiltern der Störungen und zur Umwandlung der Spannungswerte in Frequenzbänder noch die OpenBCI-GUI Software, da sich eine direkte Verbindung mit dem Board als überaus schwierig herausstellte. In zukünftigen Versionen wird es hier jedoch auch eine Entwicklung geben.
Für das Sammeln der Trainingsdaten gibt es eine eigenes Script, in dem man zuerst den aktuellen Zustand (bspw. 1000 = Gedanke: Arm hoch) einträgt und dann solange der entsprechende Zustand besteht eine Taste drückt. Das Script speichert die Aufnahmen nachdem es beendet wurde als CSV-Datei im Unterverzeichnis „samples“.
2.4.4 Random-Forest-Regressor und Features
Wie bereits mehrfach erwähnt, verwenden wir zur Auswertung der Daten den in SciKit-Learn enthaltenen Random-Forest-Regressor . Gründe dafür sind, dass dieser sehr schnell trainiert werden kann und vielseitig einsetzbar ist. Wir nutzen aktuell insgesamt 80 (5 Bänder x 16 Kanäle) Features, von denen jedes eine gewöhnliche Float-Zahl ist, die die Signalstärke eines Frequenzbandes an einer Elektrode abbildet. Trainiert wird mit zuvor aufgenommenen Messwerten, die mit den gleichzeitigen Zuständen verknüpft sind. Je nach zu erkennenden Gedanken, verwenden wir zwischen 10.000 und 40.000 Messwertreihen. Die Aufnahme dieser Messwerte erfolgt über ein eigenes Script , das die Daten dann im CSV-Format abspeichert.
2.4.5 Verwendete externe Bibliotheken
Da wir nicht den gesamten Code für den Random-Forest-Regressor und die Web-API schreiben konnten, haben wir externe Bibliotheken genutzt. Die wichtigste ist SciKit-Learn, die vorgefertigten Tools für maschinelles Lernen zur Verfügung stellt. Der Hauptvorteil ist hier, dass die Bibliothek einfach eingebunden und benutzt werden kann. Des Weiteren haben wir das API- und Web-Toolkit „Flask“ bzw. „Flask Restful“ verwendet, um mit dem Programm kommunizieren zu können. Neben diesen haben wir auch für Python-Projekte typische Bibliotheken, wie die „Matplotlib“, „Numpy“, „Pandas“ und „Scipy“ verwendet, von denen SciKit-Learn abhängig ist. Außerdem enthalten sie diverse Tools und Visualisierungen. Alle verwendeten Bibliotheken sind in der Datei „requirements.txt“  vermerkt und können von PyPi installiert werden. 
2.4.6 Versionsverwaltung
Das gemeinsame Arbeiten an Softwareprojekten erfordert ein Versionsverwaltungssystem, um zum einen Änderungen der verschiedenen Entwickler zu überblicken und zum anderen, um im Falle eines nicht zu behebenden Fehlers zu vorherigen Version zurückzukehren. Aufgrund der weiten Verbreitung und Mangel an Alternativen haben wir Git gewählt, mit dem wir bereits zuvor gearbeitet hatten. Da wir unsere Konten bei GitHub zu diesem Zeitpunkt bereits erstellt hatten, haben wir dort unser Repository ohne großen Aufwand direkt erstellen können.
Wir haben die Software jedoch erst mit der auf unser neues Headset ausgelegten Version auf GitHub gestellt.
2.4.7 Vorherige Versionen
Vor der aktuellen Version hatten wir noch ein Programm, das die Daten unseres alten Headsets verarbeitete, jedoch noch nicht in der Lage war, Gedanken zu erkennen. Mit dem Schreiben der neuen Version wurde die alte vollständig gelöscht, da diese noch nicht konstruiert war, um wieder verwendet zu werden. Außerdem haben wir unsere Python-Kenntnisse über die Dauer des Projektes so erweitert, dass wir deutlich bessere Lösungen fanden, um den Code zu kürzen und in mehreren Scripts zu verwenden. 
2.5 Bau/Programmieren der Armprothese
Ursprünglich hatten wir viele Pläne zum Bau einer Armprothese. Die Armprothese sollte teils aus einem leicht zu bearbeitenden Material, beispielsweise Messing und PLA (PLA ist das Filament, welches häufig von FDM-Druckern verwendet wird), bestehen. Teilweise bestanden auch Pläne für eine Hydraulik an den Fingern der Prothese, um ein kräftiges Zugreifen zu gewährleisten.
Den Bau der Armprothese haben wir jedoch unter anderem auf Anraten von Jugend-Forscht-Juroren vorerst zurückgestellt. Dafür gab es mehrere Gründe. Zum einen stellte sich der Bau einer Armprothese, welche einem echten Arm nahekommt, als sehr komplex dar. Da wir bisher auch nicht genug Signale bekommen und verarbeiten können, um eine solche Prothese zu steuern, ist der Bau einer solchen noch nicht von Nöten. Zum anderen ist uns klar geworden, dass wir unser System nicht zwingend auf eine Armprothese begrenzen müssen, sondern deutlich mehr Möglichkeiten haben, beispielsweise die Steuerung einer Drohne. So trafen wir die Entscheidung, vorerst nur eine virtuelle Armprothese zu programmieren und für Jugend forscht ein kleines Demonstrationsmodell zu bauen.
Dieses Demonstrationsmodell wird aus zwei Gelenken bestehen, welche wiederum mit Stepper-Motoren angetrieben und von einem ESP8266 angesteuert werden. Die Datenübertragung läuft über das im ESP integrierten WiFi-Modul. Die Signale, welche die KI ermittelt, werden von einem in C++ geschriebenen Programm in Steuerungsbefehle umgewandelt, welche wiederum analog auf die Motoren übertragen werden.
 
2.6 Grober zeitlicher Ablauf unserer Arbeit

2018	September & Oktober	Ideenfindungsphase
Erkundung möglicher Hardware
Bestellen des OpenBCI-Ganglions
	November	Tests mit neu angekommener Hardware
Anmeldung für Jugend forscht 2019
	Dezember	Programmieren der ersten Softwareversion (nur Datenfilter)
Schreiben an der Langfassung

2019	Januar	Fertigstellung der Langfassung, erste Vorbereitungen für den Jugend forscht Wettkampf. Weiteres Ausfeilen der Software
	Februar	Intensive Vorbereitungen für den Jugend forscht Wettbewerb, Erstellen des Plakates. 
Software „aufhübschen“.
Jugend forscht Wettbewerb
	März	Überlegungen für Weiterentwicklung unseres Systems
	16 oder 32 Kanäle?
Überlegungen, welches Machine-Learning-Toolkit verwendet werden soll und welche Daten es verarbeiten soll.
	April	Treffen der endgültigen Entscheidungen zur weiteren Verfahrensweise
	Mai	Noah Ihlein tritt dem Projekt bei, wird eingeführt. 
Antrag für ein Sponsoring von OpenBCI wird gestellt, leider ohne Antwort.
	Juni	Beantragung von Mikro-Makro-MINT
Beginn mit dem Programmieren der Software
	Juli	Weiterentwicklung der Software.
	August	Weiterentwicklung der Software.
Warten auf Bestätigung von Mikro-Makro-MINT
	September	Bestätigung von Mikro-Makro-MINT
Bestellen der Hardware
	Oktober	Weiterentwicklung der Software, Bau des Headsets mit OpenBCI „Cyton“
	November	Weiterentwicklung der Software
Anmeldung für Jugend forscht
	Dezember	Zusätzlich zum OpenBCI „Cyton“ erhalten wir das „Daisy“, eine Erweiterung von 8 auf 16 Kanäle findet statt
Erweiterung der Software
Schreiben der Langfassung
2020	Januar	Erweiterung der Software/Trainieren der KI auf drei verschiedene Zustände
Fertigstellung der Langfassung
3. Probleme
Leider läuft nicht immer alles wie geplant, immer wieder hatten und haben wir mit verschiedenen Problemen zu kämpfen, die den Projektfortschritt gefährdeten. 
3.1 Hardware
Im Hardwarebereich gab es die meisten und schwierigsten Probleme. So gab es oft Verbindungsprobleme zwischen Board und Dongle. Ein anderes Problem waren die bereits erwähnten Störsignale, welche durch verschiedene elektrische Geräte im Raum verursacht wurden. Ein Beispiel hierfür ist ein kaputtes Netzteil eines Computers. Durch diese Fehler kamen viele Stunden des Ausprobierens und der Fehlersuche zustande. 
Größere Probleme hatten wir auch als das Headset ausgedruckt werden sollte. Dieses war zu groß um in den uns zur Verfügung stehenden Druckern ausgedruckt werden können. Der Versuch, das Headset in getrennten kleineren Stücken auszudrucken ist fehlgeschlagen. Das Problem wurde letztendlich dadurch gelöst, dass das Headset von einem Freund in einem größeren FDM-Drucker ausgedruckt wurde.
3.2 Software
Auch softwaretechnisch gab es immer wieder Probleme, zu denen hauptsächlich Bugs in der von OpenBCI zur Verfügung gestellten GUI-Software zählten, weshalb wir mehrfach auf ältere Versionen zurückgreifen mussten. Aufgrund dieser Unzuverlässigkeit planen wir, in zukünftigen Versionen eine direkte Verbindung zwischen Headset und Computer herzustellen
3.3 Sonstiges
Abgesehen von den technischen Problemen hatten wir aufgrund der langen Lieferzeiten unserer Boards und der Bewerbungszeit für die Mikro-Makro-Mint-Unterstützung zwischenzeitlich sehr lange Wartezeiten, in welchen wir nicht effektiv arbeiten konnten. Da sich alle Gruppenmitglieder nun in der zwölften Stufe der Schule befinden, müssen wir uns auch immer mehr mit dem regulären Schulstoff beschäftigen, was dazu führt, dass wir uns teilweise nicht in dem Maße mit unserem Projekt beschäftigen konnten, wie wir es gerne getan hätten.
4. Zukunftspläne
Wir hoffen, dass wir unser System auch nach Jugend forscht weiterentwickeln können. Dafür benötigen wir vor allem bessere Hardware, was einen hohen Kostenaufwand bedeutet. 
Mit verbesserter Hardware könnten wir die KI auf noch mehr Zustände trainieren und somit dann eine richtige Armprothese ansteuern, welche es sich dann endlich zu bauen lohnt.
5. Ergebnisdiskussion
Wir haben es geschafft unser System so zu entwickeln, dass verschiedene Hirnströme voneinander unterschieden werden können. Es bleibt ein großes Entwicklungsfeld, dies auf Normalbedingungen mit Bewegung und verschiedenen Tätigkeiten auszuweiten und auf verschiedene Geräte, wie Armprothesen, zu übertragen. Ungeklärt ist, wie viele unterschiedliche Signale maximal gemessen und interpretiert werden können, da man mit einem EEG-Gerät nur die Hirnströme der obersten 2cm der Großhirnrinde ableiten kann und die Messdaten insgesamt nicht genau genug sind. Die Lösung für dieses Problem könnte in einem noch besseren EEG-Gerät mit noch mehr Kanälen liegen.



6. Zusammenfassung
Das von uns entwickelte System lässt sich in der Theorie auf viele verschiedene Bereiche anwenden, die weit über eine Armprothese hinausgehen. Durch unsere lange Planungsphase waren wir in der Lage, unsere weitere Vorgehensweise nach Jugend forscht 2019 zu diskutieren und nach Lösungen für Probleme suchen. Durch unseren Wechsel auf 16 Kanäle und die Anwendung des 10-20-Systems konnten wir eine deutlich höhere Messgenauigkeit erreichen als wir ursprünglich mit unserem Ganglion-Board mit vier Kanälen hatten. Wir haben es geschafft, ein Programm zu entwickeln, welches zuverlässig die Daten des EEG-Gerätes aufnehmen und so weiterverarbeiten kann, dass eine von uns trainierte KI diese erkennt, verarbeitet und entsprechende Signale an das angeschlossene Gerät, dem Demonstrationsmodell, leitet.
Da wir in der Lage sind, mehr als zwei verschiedene Zustände im Gehirn mit unserem EEG-Gerät zu erkennen, haben wir die Erwartungen vieler, einschließlich unserer eigener, übertroffen. Das System kann von nun an primär durch eine Verbesserung der Hardware-Komponenten weiterentwickelt werden, wozu uns allerdings vor allem die finanziellen Mittel fehlen.
Alles in allem ist unser Projekt in jeder Hinsicht ein Erfolg. Wir hoffen darauf, dass wir das von uns entwickelte System trotz verschiedenster Hürden weiterentwickeln können und in Zukunft eine richtige Armprothese ansteuern können.
7. Danksagung
Danken möchten wir allen, die es uns ermöglichen unsere Idee zu verwirklichen. Vor allem danken wir Dr. Joachim Groß, Lehrer und Leiter des Schülerforschungszentrums in Eningen unter Achalm für die Betreuung und das finanzielle Management unseres Projekts.
Vielen Dank auch an Simon Benezan für die Hilfe unser Headset mit dem 3D-Drucker auszudrucken.
Außerdem danken wir unseren Eltern, die uns über die Dauer des ganzen Projektes unterstützt haben.
Des Weiteren danken wir der Baden-Württemberg Stiftung für die finanzielle Unterstützung innerhalb des Mikro-Makro-MINT-Programmes. 
 
8. Abbildungs- und Quellenverzeichnis
8.1 Abbildungen
Abbildung 1 - Gruppenbild	1
Aufgenommen von Thorsten Beimgraben, am 31.12.2019 
Abbildung 2 - Arbeitsplatz Zuhause	1
Aufgenommen von Frederik Beimgraben, am 27.12.2019
Abbildung 3 - Headset	1
Aufgenommen von Linus Beimgraben und Maximilian Menzel, am 28.12.2019
Abbildung 4 - Unipolare Referenzschaltung	4
https://www.sciencedirect.com/science/article/abs/pii/S143948471730056X  
Abbildung 5 - 10-20 System nach Jaspers	5
https://www.bci2000.org/mediawiki/index.php/User_Tutorial:EEG_Measurement_Setup 
Abbildung 6 - Platzierung der Elektroden auf dem Ultracortex Mk-IV	5
Screenshot aus der OpenBCI GUI, aufgenommen von Maximilian Menzel, am 10.01.2020
Abbildung 7 - Ganglion Board	6
Aufgenommen von Frederik Beimgraben, 2018
Abbildung 8 - Cyton Board mit Daisy Erweiterung	6
Aufgenommen von Linus Beimgraben und Maximilian Menzel, am 28.12.2019
Abbildung 9 - Schraubelektrode für das Headset	7
Aufgenommen von Maximilian Menzel, am 08.01.2020
Abbildung 10 - Vollständiges Headset	7
Aufgenommen von Linus Beimgraben und Maximilian Menzel, am 28.12.2019
Abbildung 11 - Aufnahme von Messdaten	7
Aufgenommen von Noah Ihlein, am 10.01.2020
Abbildung 12 - Programmfunktion	8
Grafik, Erstellt von Frederik Beimgraben, am 10.01.2020

 
8.2 Quellen/Literatur  
STÖHR, Manfred; KRAUS, Regina: Einführung in die klinische Neurophysiologie. EMG-EEG-Evozierte Potenziale. Steinkopff Verlag Darmstadt, 2014.

HERRMANN, Björn: Methoden der kognitiven Neurowissenschaften – Elektroenzephalographie. Leipzig, Deutschland Mai 2014, entnommen am 02.01.2019.

BERTSCH, Katja: Das EEG: Spontan-EEG und EKP, Trier, Deutschland Dezember 2007, entnommen am 07.12.2018.

KÜBLER, Andrea und NEUPER, Christa: Gehirn-Computer-Schnittstellen (Brain-Computer Interfaces): Anwendungen und Perspektiven, entnommen am 02.01.2019 – https://www.degruyter.com/view/j/nf.2008.14.issue-2/nf-2008-0205/nf-2008-0205.xml

OpenBCI Documentation, entnommen im Oktober 2019 – 
https://docs.openbci.com/docs/Welcome.html

OpenBCI GUI, entnommen im Oktober 2019 (Version 4.1.3) –
https://docs.openbci.com/docs/06Software/01-OpenBCISoftware/GUIDocs 
