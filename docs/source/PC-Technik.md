# PC Technik

## Hauptplatine, Netzteil und Gehäuse

### Chipsatz

#### Entwicklung

Das Wort Chipsatz beschreibt man eine unbestimmte Anzahl von Bausteinen, die zusammengefasst wurden. Diese führen zahlreiche Steueraufgaben und für das Zusammenarbeiten dies Komponenten.

Ursprünglich bestanden dies Chipsatze aus einzelnen Schaltkreisen die überall auf dem Motherboard verteilt waren. Bis sie immer mehr Zusammengeführt wurden. Aber wegen den unterschiedlichen Geschwindigkeiten der Komponenten wurden zwei Integrierte Schaltkreise die oberhalb und unterhalb der CPU auf dem Motherboard Platziert wurden. Diese nennen wir Northbridge und Southbridge. Dies Weiterentwicklung sorgte für die Entwicklung für viele verschiedene neue Architekturen.

#### Bridge-Architektur

![Screenshot from 2022-09-23 09-31-16.png](./_static/Chipsatz_Bridge.png)

Die älteste Form, die Bridge-Architektur, hat alle Komponenten die höhere Arbeitsgeschwindigkeit (Grafik, Arbeitsspeicher) brauchten an der Northbridge. Die CPU wurde an die Northbridge via der **FSB** (**F**ront **S**ide **B**us) angeschlossen. Alle anderen Komponenten wurden an der Southbridge angeschlossen.

#### Hub-Architektur

![Screenshot from 2022-09-23 09-31-44 (2).png](./_static/Chipsatz_Hub.png)

Mit der Technischen weiterentwickeln kamen auch neue Architekturen. Eine davon war die Hub-Architektur welche die Northbridge mit der MCH (Memory Controller Hub) ersetzte. Es gab auch die GMCH (Graphics Memory Controller Hub) die manchmal noch dazu für die Grafikkarte entwickelt wurde

Dazu noch gab es den ICH (I/O Controller Hub) welcher sich um alle anderen Anbindungen sich kümmerte (USB, Laufwerke, Bios, etc.).

Um aber die Möglichkeit klassische Erweiterungen einzubauen. Gab es auch den I/O Chip. Welche funktionale Erweiterungen erlaubte.

#### Erweiterte Hub-Architektur

![Screenshot from 2022-09-23 09-32-29 (2).png](./_static/Chipsatz_erw.png)

Nachdem die Leistungsansprüche immer mehr steigen wurde eine neue Architektur entwickelt welche die Grafik und Arbeitsspeicher direkt an die CPU anschließt. Des weiteren werden nun MCH und ICH in ein Gehäuse gepackt welches man ein "Einchip"-Chipsatz nennt. Auch der Steckkarten Anschluss wurde von ICH zur MCH bewegt, da es immer populärer wird eine externe Grafikkarte ein zu bauen.

Modernere Beschreibungen und Darstellungen zeigen auch eine PCH. Die PCH wurde entwickelt unterschiedliche Funktionen auszuführen die benötigt wurden zum Beispiel: Overclocking, extra PCI_Lanes, USB 2.0, M.2, etc..

### CPU

Bei einem Motherboard kann es an sein Architektur nur eine bestimmte reihe an CPUs verwenden. Deshalb immer im voraus überprüfen ob das Motherboard mit deiner CPU kompatible ist. Es kann sein das bei nicht kompatiblen Geräten Schäden an den Komponenten entstehen können. Diese Inkompatiblen Eigenschaften können komplett andere Sockel, anderes BIOS bis zu einer anderen Pin Verlegung sein.

#### Prozessorreihen

Es gibt CPUs in unterschiedlichen Formen und Funktionen, wie zum Beispiel verwendet man CPUs auch in Smart Home Systemen diese Geräte nennt man IoTs oder Internet der Dinge. Daher muss man auch genau schauen für was die CPU gemacht worden ist. Zum Beispiel hat AMD ganz viel unterschiedliche CPUs die verwendet werden können, wie der Ryzen und Ryzen Threadripper/Pro reihe welche für Desktops und Workstations gedacht sind.

### CPU Prozessorsockel

Das Ausschlaggebendste an der Auswahl einer CPU ist ihrer Sockel denn nicht jedes Motherboard unterstützt jede CPU. Deshalb immer im Motherboard Handbuch schauen was es Unterstützt, da manche Sockel Identisch aussehen aber doch anders sind. Beim versuch von solchen Sockeln kann es zu Schäden kommen z.B. ein tödlicher Kurzschluss an der CPU womit das gesamt gerät nutzlos gemacht wird.

### Weitere Komponenten

Nicht alle Komponenten werden von dem Motherboard unterstützt so muss man dort auch immer drauf achten das die Features die man Will auch unterstützt werden.

Zum Beispiel werden Intrigierte Grafiken oder Grafikkarten nicht unterstützt auch PCI und PCIe können nicht unterstützt werden.

Aber auch Laufwerke und externe Schnittstellen(USB, etc) könnten nicht unterstützt werden.

#### BIOS-Chip

Dieser Chip ist kein direkter teil des Chipsatz, aber is trotzdem einer der wichtigsten. Ohne ihm könnte der Computer nicht laufen.

In der ist die Software die deine Betriebssystem einschaltet und die PC Process beginnt, somit ist es immer die erste Software die du startest.

Der speicher des BIOS-Chips ist ein ROM speicher was für Read-Only-Memory steht.

### Steckplätze

#### Arbeitsspeicher (Hauptspeicher)

Die Steckplätze für den Arbeitsspeicher des Computers (auch Hauptspeicher genannt, vgl. Kapitel 5 und Abschnitt 13.3) nehmen die RAM-Module auf. Diese Haben sich, ebenso wie die Steckplätze für Prozessoren, weiterentwickelt und sind untereinander nicht Kompatibel. Die Anzahl der Anschlusskontakte hat in den letzten Jahre zugenommen. Um das Einsetzen falscher Module zu verhindern, sind die Sockel mit einem Steg versehen.

Für Ältere Speichermodule verfügen einige Mainboards aus Gründen der Abwärtskompatibilität zusätzlich über Steckplätze. Aus dem Handbuch des Motherboard-Herstellers entnehmt man ob ein Mischbetrieb möglich wäre und welche Einschränkungen sich daraus ergeben. Dort steht auch welche Speicherkapazitäten durch Kombination, welche Module, in welchem Steckplatz erreicht werden können.

Um den Spektrum und damit auch den Datendurchsatz zu erhöhen, sollten bei neueren Board die Speichermodule immer Paarweise (Dual Channel) bzw. zu dritt/zu viert eingesteckt werden (Triple Channel/Quad Channel) Dazu sind paare (Steckplätze) oft farbig gekennzeichnet. Im Beispiel oben sollten die ersten zwei Speichermodule in die Blauen Steckplötze gesteckt werde. 

![Steckplätze.png](./_static/Steckplaetze.png)

Viele Speichermodulen-Hersteller bieten für die Einrichtung der unterschiedlichen Channel-Konfigurationen spezielle Kit-Varianten ihrer Speichermodule an, wo mit Kit mehrere Speichermodule gemeint sind. Im Lieferumfang befinden sich zwei identische Speichermodule wodurch eine optimale Leistung erreicht wird.

#### Erweiterungssteckplätze von ISA zu PCI

Mit den Erweiterten Steckplätzen des integrierten Bussystems, auch **Slots** genannt kann man den Computer um zusätzliche Funktionalitäten erweitern, zum Beispiel eine Netzwerkkarte.

Der Standartbus war in der PC-Welt der PCI (Peripheral Component Interconnect) im Jahre 1995 bis 2003. Bei diesem parallelen Bus teilen sich alle angeschlossenen Geräte die nutzbare Bandbreite von etwa 133 MB/s (PCI2.0). In laufe der Zeit sind immer schnellere Versionen erschienen, die bis zu 533 MB/s und bei speziellen Ausführungen aus dem Serverbereich bis zu 4 GB/s transportierten /PCI-X-533. Zwischen 1 und 6 PCI-Steckplätze befanden sich auf einem Mainboard.

In seltenen Fällen gab es in Kombination mit dem PCI-Bus noch einen schwarzen Steckplatz für den sogenannten ISA-Bus (Industry Standard Architecture) auf dem Mainboard. Alte Karten des XT-oder AT-Busses konnten so weiterverwendet werden. Der ISA Bus arbeitete in der Regel mit einer Taktfrequenz von 8,33 MHz und erreichte in einem 16 Bit System eine Datentransferrate von 5,33 MB/s.

Die ersten IBM gefertigten 8Bit Personal Computer wurden als XT (e**X**tended **T**echnology) bezeichnet, die neueren 16bit Versionen wurde dann als AT (**A**dvanced **T**echnology) bezeichnet.

Gegen Ende der 90er Jahre wurde **AGP** (Accelerated Graphics Port) für eine schnellere Anbindung der Grafikkarte eingeführt. Obwohl AGP auf PCI-Protokoll basiert, handelt es sich nicht um ein Paralleles Bussystem, sondern um eine Punk zu Punkt Verbindung. Dieser Steckplatz ist oft braun. Die Übertragungsgeschwindigkeit ist wischen 0,266gb/s und 2,1 GB/s. Seit circa 2006 ist diese Grafikschnittstelle veraltet und wurde durch den **PCI Express** (PCIe) ersetzt.

#### PCI Express (PCIe)

PCI Express verwendet genau wie die AGP Punkt-zu-Punkt Verbindung. Diese Verbindungen werden **Lanes** genannt. Zur Erhöhung können 16 Lanes der Übertragungsbandbreite an einem Steckplatz angeschlossen werden. Die Anzahl der Lanes wird mit einem ,,x" und einer gefolgten Zahl bestimmt. Mögliche Steckplötze wären mit x1, x4, x8 und x16. PCIe 4.0 ist im Jahre 2017 erschienen. Im Jahr 2020 hätte PCIe 5.0 erscheinen sollen. Für welches Jahr die jeweiligen PCIe Spezifikationen vorgesehen sind und die Höhe der jeweiligen Übertragungsraten, kann den nachfolgenden Tabellen entnommen werden.

![asdf.png](./_static/asdf.png)

![fdas.png](./_static/fdas.png)

2017 wurde bereits der PCIe 4.0 Standard Ratifiziert, die Hersteller halten sich mit dem Einsatz dieses Anschlusses aber weiterhin zurück. Erst 2020 nimmt die Anzahl der Boards mit PCIe 4.0 Unterstützung zu. Der PCIe 3,x bleibt weiterhin Standard, weil es am breiten Angebot von Grafikkarten fehlt.

Viele neue Motherboards verfügen über eine ganze Reihe unterschiedliche PCI-Express-Steckplätze, die je nach Leistungsfähigkeit der Erweiterungskarten Verwendung finden. 

Der sogenannte **PEG**\-Steckplatz (PCIE Express for Graphics) ist im Prinzip wie ein normaler PCIe-x16-Slot, der PEG-Steckplatz ist jedoch stärker, da er mehr Leistung aufnehmen kann (kann 75W statt 25W). Mit einem Zusatz Stecker von der Stromversorgung zu einer PCIe-Karte, den **PEG-Connector**, kann die maximale Leistung der Grafikkarte höher sein. Über einen 6-poligen Anschluss kann die Leistung um bis zu 75W höher sein und ein 8-poliger bis zu 150W. Dies sollte aber bei der Auswahl der PSU (Netzteil) berücksichtigt werden!

Bei den neusten Prozessoren ist der anfängliche PCI-Bus nicht mehr ein Bauteil des Chipsatzes und sollt mit einer PCIe-to-PCI-Bridge nachgebaut werden.

Die Aktuellen Motherboards verfügen nahezu ausschließlich über PCIe-Slots. Stellen sie daher vor dem Kauf eine Erweitertungssteckkarte unbedingt den Typ des Motherboards und dessen Anschlussmöglichkeiten fest. 

### Anschluss

#### Interne Laufwerke

Bei neuen Desktop Mainboard sind die Controller für Festplatten und optische Laufwerke auf der Platine integriert. Damals waren IDE- bzw. EIDE-Controller der Standard, heutzutage sind sie nahezu vollständig durch SATA oder M. 2 abgelöst worden.

Sata (Serial ATA) ist der gängige Standard auf neune Motherboards. Auch dieser Anschluss hatte sich über die Jahre entwickelt und unterstützt heute drei Betriebsarten, die abwärtskompatibel zueinander sind. Diese sind:

SATA I                                     150 Mbyte/s  
SATA II / SATA 300                  300 Mbyte/s  
SATA III / SATA 600                 600 Mbyte/s  

Berücksichtigen Sie bei Anschluss einer Festplatte die interne Geschwindigkeit der HDD. Erst bei der Verwendung eines SSD (Solid State Drive) ist es möglich, das Leistungspotenzial von SATA II oder SATA III vollkommen auszunutzen.

#### M.2/U.2

Obwohl der M.2 Steckplatz für die Verwendung unterschiedlicher Erweiterungsmodule erstellt wurde, wird dieser häufig mit dem Betrieb von M.2-SSD Laufwerken oder einem Intel Optane Memory Modul in Verbindung gebracht. 

#### Peripheriegeräte

Bei ATX-Mainboards sind die externen Anschlüsse am Rand der Platine aufgelötet und so direkt von außen nutzbar.

Externe Schnittstellen bei einem Pentium-4-Board von 2003:

1) PS/2-Anschlüsse für Tastatur und Maus  
2) Digitalsound optisch und koaxial (SPDIF)  
3) Parallelschnittstelle  
4) Serielle Schnittstelle  
5) USB-Anschlüsse  
6) Netzwerkanschluss (RJ45)  
7) Sound-Anschlüsse analog 

![Externe Schnittstellen bei einem Pentium 4 board von 2003 (2).png](./_static/Externe_Schnittstelle.png)

Auf aktuellen Mainboards finden sich eventuell noch Anschlüsse für FireWire (IEEE 1394) oder wie in der folgenden Abbildung Monitoranschlüsse, falls ein Onboard-Grafikchip vorhanden ist.

Externe Schnittstellen von einem aktuelleren Board:

1) USB 2.0  
2) Kombi-PS/2-Anschluss Tastatur/Maus  
3) Monitorausgang analog VGA  
4) Monitorausgang digital DVI  
5) Sound digital (SPDIF) optisch  
6) Monitor/TV-Ausgang digital HDMI  
7) Monitor/TV-Ausgang digital DisplayPort  
8) FireWire 400  
9) eSATA (externes SATA)  
10) Gigabit Ethernet  
11) USB 3.x  
12) Sound-Anschlüsse analog

![Externe Schnittstellen bei akutellen Mainboard.png](./_static/Externe_Schnittstellen_akutellen.png)

#### PS/2-Anschlüsse

Der Anschluss für die Maus ist grün, der für die Tastatur violett. Die PS/2-Anschlüsse für Tastatur und Maus sind zwar baugleich, unterscheiden sich aber in ihrer Funktion. Bei den Peripheriegeräten (interne oder externe Geräte) sind die Stecker meist in der entsprechenden Farbe hergestellt, sodass das Verwechslungsrisiko erniedrigt ist.

Wenn die Anschlussbuchsen nicht farbig gekennzeichnet sind, weist ein Symbol für Tastatur und Maus neben dem entsprechenden Steckplatz auf das anzuschließende Gerät hin. Außerdem befindet sich der Anschluss für die Maus in aller Regel über dem PS/2-Tastaturanschluss (siehe 1) Schnittstellen-Anschlüsse an einem ATX-Board von 2003). Sind auf einem neuen Board noch PS/2 Anschlüsse vorhanden, ist dies meist ein Kombi-PS/2-Anschluss.

Möchten Sie weiterhin Ihre Tastatur und Maus an PS/2 betreiben, benötigen Sie einen Y-Adapter für PS/2-Geräte

### Baugrößen von Mainboard und Gehäuse

#### Mainboard-Formfaktoren

Bei Mainboards gibt es mehrere funktionale Abmessungen oder Formfaktoren. Der Formfaktor bestimmt die Abmessungen des Mainboards sowie Art und Lage der Bauteile und Anschlüsse.  
Im Laufe der Entwicklung haben sich verschiedene Formfaktoren gebildet, die jeweils für bestimmte Prozessorgenerationen und die entsprechende Peripherie geeignet sind:

![Mainboard Faktoren.png](./_static/Mainboard_Faktoren.png)Der Formfaktor eines Mainboards bestimmt außerdem den Gehäusetyp und das verwendbare Netzteil. Der Wechsel zu einem neuen Mainboard kann deshalb auch ein neues Gehäuse erforderlich machen. Grundsätzlich passen ATX- und microATX-Mainboards nicht in ein BTX- oder ITX-Gehäuse und umgekehrt auch nicht.

#### ATX

Das ATX-Format (AT Extended) von 1996 ist der Nachfolger des Baby-AT-Formats (Advanced Technology) aus den 80er-Jahren. Entwicklungsziele für diesen Formfaktor waren unter anderem eine bessere Übersicht und Praxis sowie verbesserte Kühlung und eine abnehmende Lautstärke.

Das ATX-Konzept ist inzwischen sehr optimiert und hat sich auf dem Markt erfolgreich durchgesetzt. Weitere Vorteile und Features des ATX-Formfaktors sind:  
\-Auf der Board-Unterseite befindet sich ein aufgelötetes Input/Output-Panel, wodurch externe Peripheriegeräte (Maus, Tastatur, Drucker etc.) direkt angeschlossen werden können.  
\-Die Kabelanschlüsse für Gehäusekomponenten (Lautsprecher, Reset, Power-On) sind seitlich sehr übersichtlich in einer Reihe angebracht.  
\-Die Stromversorgung des Mainboards erfolgt mit einem verpolungssicheren Steckanschluss und kann daher auch von unerfahrenen Benutzern fachgerecht angeschlossen werden.  
\-CPU und Speicherbänke sind zueinander versetzt. Die Steckplätze bzw. Sockel sind oft so angeordnet, dass sie leicht erreichbar sind, ohne dass bei der Aufrüstung Erweiterungskarten ausgebaut werden müssen.  
\-ATX-Mainboards können die CPU-Temperatur oder Lüfterdrehzahl überwachen. Der Nutzer kann diese Daten über eine mitgelieferte Software jederzeit am Bildschirm verfolgen. Falls die Temperatur einen schlimmen Schwellenwert übersteigt, schaltet sich der Rechner automatisch ab.  

Der ATX-Standard schreibt für Mainboards ein Zonenmodell vor, in dem festgelegt wird, in welchen Bereichen des Mainboards, bestimmte Bauteile und Funktionsgruppen untergebracht werden müssen. Alle möglichen Maße vom Freiraum rund um den CPU-Sockel bis hin zu den Positionen der Befestigungslöcher sind geregelt. So ist sichergestellt, dass jedes ATX-Board in jedes ATX-Gehäuse passt.

#### microATX

Das microATX-Format ist eine Weiterentwicklung des ATX-Formats. Die Position der Steckplätze und externen Anschlüsse wurden beibehalten, um eine Verträglichkeit mit bestehenden ATX-Gehäusen zu ermöglichen. Nur ein Teil der Montagebohrungen wurde an die geringere Größe des microATX-Mainboards angepasst. 

Die geringere Boardgröße ermöglicht insgesamt kleinere PC-Gehäuse und kann helfen, die Systemkosten zu erniedrigen. Der dichte Aufbau kann allerdings zu Problemen bei der Wärmeabfuhr von leistungsfähigeren Prozessoren führen und setzt engere Grenzen bei der Erweiterung durch Steckkarten.

Die schnelle Evolution, besonders der Prozessoren und Chipsätze, zwingt auch bei Mainboards zu ständiger Weiterentwicklung. Dabei stehen die fortschreitende Integration von elektronischen Bauteilen und eine Beschränkung der mechanischen Bedienelemente (Jumper) im Vordergrund. Um ständig aktuellen Trends gerecht werden zu können, besitzen Mainboards oft nur minimal längere Produktzyklen als die eingesetzten CPUs.

#### BTX-Format

Das BTX-Format (Balanced Technology Extended) wurde 2003 von Intel mit dem Ziel vorgestellt, ein MainboardDesign festzuschreiben, das die Hauptwärmequellen (Prozessor, Grafikkarte und Chipsatz) so platziert, dass eine nutzvolle Kühlung auch extrem heißer Prozessoren und Grafikkarten möglich ist. Dabei wurde der Aufbau und Führung des Luftstroms im Gehäuse mit einbezogen, sodass in einigen Fällen nur ein einzelner großer Lüfter zur Kühlung des Computers benötigt wird. Dies führt zu einer deutlichen Lärmreduzierung und macht das BTXFormat prinzipiell überall dort interessant, wo leise Geräte benötigt werden. 

Das BTX-Format konnte sich jedoch kaum etablieren und wurde im Jahr 2007 wieder vom Markt genommen.

#### Mini-ITX-Format

Das ursprüngliche ITX-Format wurde 2001 von VIA vorgestellt und später um die Formate Mini-ITX, Nano-ITX und Pico-ITX ergänzt. 2008 kam die Version 2.0 heraus. Vor allem Mini-ITX ist recht erfolgreich und wird z. B. für Thin Clients (ein Thin client ist ein Gerät, über das Nutzer auf virtuelle Desktops zu greifen) verwendet. Mini-ITX-Boards lassen sich prinzipiell mit einem ATX-Netzteil betreiben und passen auch in ATX-Gehäuse.

#### Computergehäuse

Passend zu den verschiedenen Mainboard- und Netzteil-Formfaktoren werden unterschiedliche Gehäuse angeboten. Da die externen Anschlüsse in die entsprechende Aussparung im Gehäuse passen müssen, können nur bestimmte Formfaktoren in den Gehäusen befestigt werden. 

### Netzteil

Ein Netzteil ist notwendig, um den Computer am Stromnetz nutzen zu können. Der PC wird an die übliche Haushaltsspannung von 230 V mit 50 Hz angeschlossen. Im Rechner selbst werden allerdings deutlich kleinere Spannungen benötigt.

Die Aufgabe des Netzteils ist es, die von außen angelegte Wechselspannung von 230 V auf verschiedene Gleichspannungen von 3.3 V, 5 V und 12 V umzuwandeln. Aus diesen Spannungen erzeugen die Spannungswandler auf dem Mainboard alle weiteren benötigten Betriebsspannungen.

Bei dem in einem Computer eingesetzten Netzteil handelt es sich um ein Schaltnetzteil. Bei Schaltnetzteilen wird die Eingangsspannung zuerst gleichgerichtet (Umwandlung einer Wechselspannung in eine pulsierende Gleichspannung) und anschließend in Wechselspannung einer höheren Frequenz (meistens im kHz-Bereich) gewandelt. Diese Spannung wird dann in eine Spannung mit geringerer Amplitude (Schwingungshöhe einer Wechselspannung) umgewandelt. Zum Schluss wird die Niedrigspannung wieder gleichgerichtet und die gewünschte Gleichspannung ist hergestellt.

Die Gleichrichtung wird bei modernen Netzteilen durch einen aktiven oder passiven Leistungsfaktorkorrekturfilter (PFC, Power Factor Correction) erreicht. In hochwertigen Netzteilen wird mit einer Kombination aus aktiver PFC und passivem Filter gearbeitet.

Das Netzteil ist ein eigeständiges elektrisches Gerät, welches keine zu reparierende teile hat. Im inneren des Netzteils sind lebensgefährliche Berührungsspannen zu finden. Falls etwas mit dem Netzteil an sich nicht stimmt dann versuchen sie es nicht zu reparieren tauschen sie es als ein Komplettes teil aus.

#### Anschluss der Stromversorgung

Jedes Motherboard braucht einen Anschluss, über den dann die Spannung zugeführt wird. Bei den ATX-Mainboards wurde der Stecker verpolungssicher hergestellt.

Das Mainboard, Netzteil und das Gehäuse müssen aufeinander abgestimmt sein. Für ein ATX-Mainoard brauchen sie ein ATX-Netzteil und ein ATX-Gehäuse. Am anfang wurden ATX-Mainboards über 20-polige Anschlüsse mit Strom versorgt (ATX 1.0 u. 1.3). Wegen modernen Grafikkarten wurden die Stromanschlüsse um 4 weiter Pins erweitert.

Durch den hohen Strombedarf der Prozessoren und Grafikkarten hat die Leistungsfähigkeit der Netzteile immer mehr zugenommen. 

![](./_static/24poligeranschluss.png)

#### Zusätzliche Stromversorgung für Prozessoren

Mainboards mit neuen Prozessoren reicht der ATX-Stromanschluss nicht mehr aus, um ihn mit dem benötigten Strom ausreichend zu versorgen.

Aus dem Grund befindet sich seit der ersten Revision des ATX-Standards auf diesen Mainboard noch ein wieterer, meist quadratischer 12-Volt-Stromanschluss, der verpolungssicher ausgeführt ist. Der 4-polige Anschluss wird ,,ATX12V" oder ,,Intel-P4-fähig" genannt.  

Bei Serverboards oder stromhungirge Prozessoren wird manchmal auch der 8-polige zusätzliche EPS12V-Stromanschluss verwendet, auch in Form von zwei 4-poligen ATX12V-Stecker, die nebeneinander eingesteckt werden.

#### ATX-Netzteilstandards

Der ATX-Standard wurde 2000 in ATX12V umbenannt. Version 1.0 brachte den zusätzlichen vierpoligen Stromanschluss.

Mit Version 2.0 wurde 2003 der Anschluss für die Stromversorgung auf 24 Pole verbreitert. Anschlüsse für die SATA-Stromversorgung wurden zwingend erforderlich. Außerdem wurde die Leistungsabgabe der 12V-Schienen verstärkt.

Version 2.1 und 2.2 brachten die 6-poligen und 8-poligen PCIe-Stecker (75 W bzw. 150 W zusätzlich für die Stromversorgung der Grafikkarte). Zusammen mit den 75 W des PEG-Slots kann eine einzelne Grafikkarte nun bis zu 300 W ziehen. Version 2.3 machte kleine Änderungen bei der geforderten Energieeffizienz, die mindestens 70 % fordert und 80 % empfiehlt. Im Zusammenhang mit der Einführung der Intel Haswell Microarchitektur  
wurde die ATX Version auf 2.4 erhöht.

#### Auswahl des passenden Netzteils

Nachdem fast ausschließlich Netzteile im ATX Format in den Desktop PCs verbaut wurde, haben sich mittlerweile andere Formfaktoren auf dem Markt fest gefügt.

![](./_static/Netzteil_formfaktor.png)Ein Grund dafür wäre, weil es Trend geworden ist kleinere und kompaktere Computer auf dem Arbeitsplatz zu haben.

#### Kabelmanagment

Bei Netzteilen unterscheidet man Geräte, bei denen die Anschlusskabel direkt aus dem Netzteilgehäuse kommen (non-modular) und solche, die anstelle von festen Kabeln Steckverbindungen verwenden (modular). Der Vorteil der modularen Geräte liegt in einer ordentlicheren Kabelverlegung und dem Verzicht auf nicht benötigte Kabel, was die Luftzirkulation innerhalb des Gehäuses verbessern kann.

#### Leistung

Moderne PCs haben einen großen Energiebedarf, der bei Einsatz mehrerer Grafikkarten unter Volllast in den Bereich von 1.000 Watt und mehr reichen kann. Normal ausgestattete Büro- oder Heim-PCs brauchen jedoch selten mehr als 400 W. Die Angabe der Gesamtleistungsaufnahme ist meist nur ein Richtwert, denn je nach Anwendung und Motherboard werden die Leitungen mit 12 V und 5 V unterschiedlich stark belastet. Je nach Anwendungsgebiet und Ausstattung muss das Netzteil den Anforderungen stets gewachsen sein, sonst drohen Instabilitäten und Abstürze. 

#### Energieeffizienz

Alle Netzteile sind im Bereich zwischen 40 % und 80 % ihrer Maximalleistung am effizientesten. Die Energieeffizienz sollte so nah wie möglich an 100 heranreichen. Achten Sie beim Kauf auf das „80 PLUS“-Logo, das es in mehreren Stufen gibt: 80 PLUS (weiß), Bronze, Silber, Gold, Platinum. Das Logo wird allerdings erst ab einer Leistung ab 350 W vergeben, sodass schwächere Netzteile, die für den Aufbau besonders sparsamer Computer interessant sind.

#### Wege zum Leisen PC

Bei jeder PC-Komponente sollten Sie auf eine niedrige Lärmentwicklung achten. Dazu gehört die Auswahl angemessen leistungsfähiger Bauteile mit möglichst leiser Kühlung.

Neben besonders leisen Silent-Netzteilen können auch normale Netzteile leise sein. Für einen leisen Betrieb sollten Sie den Energieverbrauch des Computers im Auge behalten.

Das größte Sparpotenzial ergibt sich bei der Auswahl der Grafikkarte und der CPU. Hier lassen sich 50 W und mehr schon im Leerlauf und Teillastbereich einsparen.

Moderne Prozessoren und Grafikkarten verfügen über ausgeklügelte Stromsparmechanismen. Erst wenn die volle Leistung abgefordert wird, schnellt der Stromverbrauch in die Höhe. So kann bei Grafikkarten der Stromverbrauch im Leerlauf bei 20 W liegen, bei Volllast dagegen bei über 300 W. Bei Prozessoren reicht diese Spanne von 20 W bis 140 W.

Wenn die Leistung der integrierten Chipsatz- oder Prozessorgrafik ausreicht, sollten Sie auf eine eigenständige Grafikkarte verzichten. 

Nicht zu unterschätzen ist auch der Stromverbrauch von mechanischen Festplatten. Jede Desktop-Festplatte im üblichen 3,5"-Format benötigt im Betrieb zwischen 6 W und 12 W.  Die günstigste Lösung ist ein Solid State Drive (SSD), dass schnell, lautlos und stromsparend ist (0,3 bis 4 W).

#### Ausfallsicherheit und Redundanz

Bei Workstations und vor allem Servern werden oft redundante Netzteile eingesetzt, um die Ausfallsicherheit zu erhöhen. Auch werden besonders für Serverracks USV-Anlagen installiert.

### Unterbrechungsfreie Stromversorgung

Eine USV überbrückt im fall eines Stromausfall die Zeit bis zum Anschalten eines Notstromaggregates oder des Speichern und saubere Herunterfahren des Computers. Davon gibt es 3 Unterschiedliche formen.

#### Online-USV

**Anderer Name:** Voltage and Frequency Independent

![Screenshot from 2022-09-23 09-03-57.png](./_static/USV_online.png)
*In der Schaltskizze fehlt ein Schalter der es dir erlaubt die Batterie zu Wechseln.*

Im Normalen Betrieb werden die 230V Wechselspannung in Gleichspannung gerichtet und lädt eine Bakterie und an der ausgangsseitig wieder in Wechselspannung gewandelt. In der Schaltskizze ist es die Grüne Leitung.

Aber im fall eines Stromausfalls, repräsentiert in Rot, Zieht er die Gleichspannung gleich aus der Batterie und wandelt sie um zu Wechselstrom.

| Vorteile                                                           | Nachteile       |
| ------------------------------------------------------------------ | --------------- |
| Konstante saubere und Gleichförmige Wechselspannung am Verbraucher | teuerste Lösung |

#### Line Interactive USV

 **Anderer Namen:**

* Voltage Independent
* netzinteraktiv
* aktiver Mitlaufbetrieb

![Screenshot from 2022-09-23 09-11-14.png](./_static/USV_line.png)Im Normalendbetrieb, in Grün, werden die 230V Wechselspannung gefiltert, dass beseitigt Spannungsspitzen. Vor der Batterie hängt dann ein Spannungsrichter welcher die Batterie lädt.

Aber im fall eines Stromausfalls, Rot, Wird die Gleichspannung zurück in Wechselstrom verwandelt und in das System gefüttert.

| Vorteile                           | Nachteile                 |
| ---------------------------------- | ------------------------- |
| Günstiger als die Online-USV       | keine Frequenzanpassungen |
| Schutz vor Über- und Unterspannung | Umschaltzeit 2-4ms        |

#### Offline-USV

 **Anderer Namen:** Voltage and Frequency Dependent

![Screenshot from 2022-09-23 09-20-40.png](./_static/USV_Offline.png)
Im Normalen betrieb wird die Wechselspannung am Eingang gefiltert und an den USV Ausgang sofort weitergeleitet. Ein teil davon wir in Gleichstrom gerichtet und in eine Batterie geleitet.

Im Fehlerfall (Rot) wird die Gleichspannung von der Batterie über eine Wechselrichter in Wechselspannung gerichtet und über ein Relay an den Ausgang geleitet. 

| Vorteile                  | Nachteile                                                                |
| ------------------------- | ------------------------------------------------------------------------ |
| Günstigste Lösung         | Kein wirksamer Schutz von Frequenz- und Spannungsschwankungen am Eingang |
| Schutz vor Überspannungen | lange Umschaltzeit von bis zu 10ms                                       |

#### Alle USV-Typen

Alle USV-Typen haben einen Anschluss über den der Computer Zeitgleich über den Fehler Informiert werden kann, um ein Herunterfahren zu Initialisiere. 

## Externe Schnittstelle

Im Allgemeinen ist eine Schnittstelle ein Übergabepunkt, an dem eine Verbindung zwischen zwei eigenständigen Komponenten hergestellt wird. Standardisierte Schnittstellen gibt es sowohl als Software als auch als Hardware, um bestimmte Geräte miteinander zu verbinden. Zu den ausgedienten, etablierten Schnittstellen zählen die seriellen Schnittstellen (RS232), der Parallel-Port (IEEE-1284) und die PS/2 Anschlüsse, welche heutzutage immer noch aus Kompatibilitätsgründen verbaut werden.

### PS/2 (Eingabe)

Der PS/2 Anschlüsse wurden mit der Einführung von ATX Mainboards zum
Anschluss von Tastatur und Maus von IBM bei der Personal-System-Reihe/ 2-Reihe
eingesetzt. Auf dem neuen Mainboard ist, wenn überhaupt, nur noch ein Kombi-
Anschluss verbaut, aber zum größten Teil komplett weggelassen.

Um die Abwärtskompatibilität zu gewährleisten, lassen sich PS/2 Geräte
über einen Adapter mit USB betreiben, wenn das Gerät beide Protokolle
unterstützt.

Lila steht normalerweise für die Tastatur und grün für die Maus

### USB (Ein- und Ausgabe)

Der “Universal Serial Bus” ist der am meisten verwendete Anschluss für externe Geräte. USB ist um ein wesentliches leistungsfähiger als die alte RS232 Schnittstelle und wird von allen aktuellen Betriebssystemen unterstützt. USB-Datenträger eignen sich daher gut für den Datenaustausch zwischen mehreren Geräten, da inzwischen viele Geräte eine USB-Verbindung besitzen. USB unterstützt bis zu 127 Geräte gleichzeitig, die alle eine eigene Geräte ID haben, dies ermöglicht die Verwendung von USB-Hubs, die mehrere Stecker besitzen und alle von einem Host verwaltet werden können.

#### USB 1.X

Das USB 1.0 kam 1996 auf den Markt und wurde 1998 mit USB 1.1 1998 überarbeitet. USB gab es in zwei Varianten, Low und Full- Speed mit jeweils 1,5 MBits und 12MBits desweiteren beherrst USB Plug and Play und Hot Swap

#### USB 2.0

USB 2.0 ist abwärtskompatibel zu USB 1.1 und bietet eine Datentransferrate von maximal 480 MBits. USB 2.0 findet sich auf fast jedem aktuellen Mainboard wieder. Falls dies nicht der Fall ist kann man PCi Erweiterungskarten benutzen

#### USB 3.0 (SuperSpeed)

2010 wurden erstmals Geräte mit USB 3.0 veröffentlicht, auch dieser Standard ist mit vorherigen Versionen kompatibel, weist in der ersten Version aber schon eine deutlich höhere Geschwindigkeit von 5 Gbit/s auf.

Im Laufe der Zeit wurden mehrere Abwandlungen der Spezifikation entwickelt wobei es häufig auch zu Umbenennungen kam, alle USB Versionen sind zur besseren Übersicht in einer Tabelle dargestellt:

![](./_static/USB_standards.png)

#### USB 4

USB 4 basiert auf dem von Intel zur Verfügung gestellten Thunderbolt 3 Protokoll und kann ausschließlich mit Type-C Steckern genutzt werden. Dank Thunderbolt enthält USB 4 nun standardmäßig DisplayPort und PCIe. Vorherige Versionen wurden optional mit Displayport ausgestattet.

Die Geschwindigkeiten reichen von mindestens 20 Gbit/s bis 80 Gbit/s bei Version 2.

#### USB Kabel

In USB 1.x und 2.0 werden 4 sogenannte “Adern” (Kabel) verwendet. Zwei dienen der Datenübertragung und die anderen zwei der Stromleitung. Die Abschirmung des Kabels kann auch für verschiedene erwartete Datenübertragungsraten variieren.

Der Maximalstrom beträgt 2,5W (5V * 500mA) für 1.x und 2.0. Bei 3.0 wurde dieser auf 4,5W (5V*900mA) gesteigert , mit dem sich Festplatten auch nur mit einem Kabel betreiben und lesen lassen.

Mit USB “PowerDelivery” wurde ein neuer Standard vorgestellt, der mehr Energie zur Verfügung stellen kann. Es gibt zwei verschiedene Stufen, welche beide einen Type-C Stecker voraussetzen: Standard Power Range (SPR) stellt bis zu 100W zur Verfügung, während die "Extended Power Range” (EPR) bei 240W liegt.

#### USB Stecker

Die zwei ersten USB Stecker waren die Typen A und B.

Typ A wird heute noch weit verbreitet genutzt und ist als Host Konnektor gedacht. 1.x und 2.0 haben 4 Adern und 3.x hat 9, jedoch mit Abwärtskompatibilität. Der Typ B hingegen dient als “Slave” Stecker und wird an Peripheriegeräte angesteckt (Hauptsächlich Festplatten und bis heute noch Drucker). Diesen gibt es jedoch in der USB 1.x und 2.0 Version sowie in einer abgewandelten 3.0 Version, die jeweils nicht kompatibel miteinander sind.

Hinzu kommen weitere Client-Stecker, wie Mini-USB und Micro USB und später der aktuelle Type-C Stecker, die für kleinere oder mobile Endgeräte gedacht sind.

#### USB Hubs

Es gibt aktive und passive USB-Hubs. Aktive Hubs versorgen oft mobile Endgeräte und dienen zugleich als Schnittstelle für Datentransfer von Daten und Video Signal. Dies ist praktisch, um zum Beispiel einen Laptop zu laden und zugleich die Anschlüsse zu vervielfältigen. Passive Hubs sind hingegen einfacher und dienen nur als Vervielfältigung der USB Anschlüsse.

### Thunderbolt (Ein- und Ausgabe)

Thunderbolt entstand als Kollaboration zwischen Intel und Apple und wurde 2011 vorgestellt. Mittlerweile hat der Standard auch in Windows Notebooks von Intel seinen Platz gefunden. Der Standard überträgt USB, PCI-E, Ethernet sowie Displayport-Signale über ein Kabel.

Thunderbolt 1 überträgt 10 Gbit/s, Thunderbolt 2 schafft 20 Gbit/s und Thunderbolt 3 erreicht 40Gbit/s an Throughput.

Thunderbolt 1 & 2 benutzen einen eigens entwickelten Stecker, jedoch wurde mit der dritten Generation auf einen USB-C Stecker gewechselt.

Ein Thunderbolt Kabel mit Kupferkabeln kann maximal 3 Meter lang sein, jedoch kann dies mit Glasfaser deutlich verlängert werden (jedoch mit entsprechend hohen Preisen.

### eSATA (Ein- und Ausgabe)

Der einzige Unterschied besteht im Geschirmten Kabel, zudem hält eine größere mechanische Belastung aus, die beim An und Aus stecken auftreten können. Je nach SATA Controller können Daten mit Geschwindigkeiten von 150 MB/s bis 600 MB/s übertragen werden.

Die SATA Verbindung ist theoretisch Hot-Plug-fähig, dies hat in der Praxis aber nur halbwegs funktioniert.

eSATA liefert keinen Strom, man benötigt also einen zusätzlichen Anschluss für die Stromversorgung.

Insgesamt konnte sich eSATA nicht durchsetzen

### FireWire (Ein- und Ausgabe)

Die FireWire Schnittstelle wurde 1995 von Apple eingeführt, an das serielle Bussystem können bis zu 63 Geräte angeschlossen werden. Der Vorteil von FireWire ist die OpenHCI-Schnittstelle. Verbundene Geräte können Daten untereinander austauschen. FireWire ist zudem HotPlug-fähig und wird in erster Linie zur Verbindung von digitaler Unterhaltungselektronik verwendet. 

Die Datenübertragungsrate reicht von 400 MBits bei FireWire 400 bis 800 MBits bei FireWire 800. Die letzten Apple Produkte mit FireWire kamen 2011 auf den Markt.

![](./_static/USB_Anschluss.png)

## Grafikkarten

Aktuelle Grafikkarten können alle gängigen Videoformate in Hardware decodieren und aufbereiten. Hierdurch wird die CPU beim Abspielen deutlich entlastet. Auch ist dies deutlich stromsparender als Decodieren durch die CPU. Die GPU ist bei der Umwandlung von Videodateien in andere Formate und dem Videoschnitt deutlich effizienter als die CPU.

Die Leistungsfähigkeit moderner Grafikkarten kann auch für wissenschaftliche Berechnungen genutzt werden.

Mit speziellen Anwendungen kann die parallele Architektur gut ausgelastet werden. Hier ist die Effizienz bis zu 30-mal schneller als bei einer schnellen CPU.

### Grafikspeicher

#### Funktion und Typen des Grafikspeichers

Der Grafikspeicher oder Videospeicher dient der Grafikkarte zur Ablage von Bildinformationen. Die Helligkeits- und Farbwerte der darzustellenden Pixel werden im Grafikspeicher abgelegt und können bei jeder Aktualisierung des Bildinhalts erneut ausgelesen oder aktualisiert werden. Der Bildspeicher ist Teil des Grafikspeichers und wird auch Framebuffer genannt.

Leistungsfähige moderne 3D-Beschleuniger legen auch Texturinformationen, Daten zur räumlichen Darstellung und Programmcode (Shader) im Grafikspeicher ab.

Als Grafikspeicher werden entweder auf der GPU integrierte Speicherchips oder Teile des PC-Arbeitsspeichers verwendet. Lese- und Schreibvorgänge der Bilddarstellung müssen den Systembus passieren, wodurch der für die Grafikkarte reservierte Teil des Arbeitsspeichers nicht mehr für das Betriebssystem zur Verfügung steht. Dieses Shared-Memory-Konzept findet deshalb hauptsächlich bei Notebooks und preiswerten Büro-Computern Anwendung, bei denen die Grafikleistung nicht im Vordergrund steht.

Direkt auf der Karte verbaute RAM-Bausteine für den Video-Speicher bieten Optimale Leistungen. Der Grafikspeicher soll möglichst schnell sein, damit auch bei hohen Auflösungen noch hohe Bildwiederholraten möglich sind. Deshalb kommen für Grafikkarten DDR-RAM-Bausteine zum Einsatz. Double-Data-Rate-RAM kann durch Nutzung der ansteigenden und abfallenden Flanken des Taktsignals für die Datenübertragung eine deutlich höhere Transferrate und damit verbesserte Leistung erreichen.

#### Grafikspeicherbedarf berechnen

In der Anfangszeit der Grafikkarten war die Größe des Arbeitsspeichers auf der Grafikkarte entscheidend für die mögliche Bildschirmauflösung und Farbtiefe. Moderne Grafikkarten benutzen dazu einen Speicherbereich als Bildspeicher, der doppelt oder sogar dreimal so groß ist wie der Bildinhalt (Double Buffering bzw. Triple Buffering). Jedes neue Bild wird zunächst im Puffer abgelegt und anschließend die Bildschirmausgabe auf diesen Teil des Puffers umgeschaltet.

Der RAM-Bedarf einer Grafikkarte ist in erster Linie abhängig von der gewünschten Auflösung und Farbtiefe. Für jedes Pixel muss eine von der Farbtiefe abhängige Anzahl an Bitwerten gespeichert werden, beispielsweise 24 Bit = 3 Byte für 16,7 Millionen Farben. Der minimale Grafikspeicherbedarf ergibt sich einfach als Produkt aus Auflösung und Farbtiefe: 1024x768 Pixel x 3 Byte pro Pixel = 2359296 Byte = 2,25MB.

Aktuelle Grafikkarten besitzen oft 6GB oder mehr Grafikspeicher, bei professionellen 3D-Grafikkarten können es auch bis zu 24GB sein. Für das Speichern der Pixel des Monitorbildes wäre diese Kapazität völlig überdimensioniert, aber bei 3D-Anwendungen werden u. a. die riesigen Texturen und zahlreichen Rauminformationen im Speicher abgelegt, etwa bei realistischen dreidimensionalen Darstellungen in Spielen oder bei der Berechnung komplexer Modelle im CAD-Bereich. Im professionellen Bereich werden darüber hinaus Auflösungen bei Farbtiefen von bis zu 128 Bit verwendet. Diese Aufgaben erfordern sehr große Videospeicher.

### SDRAM-Chips einer Grafikkarte

#### Bustypen und Schnittstellen für Grafikkarten

##### PCI-Express-Grafikkarten
![](./_static/Grafik_PCIe.jpeg)

Der RAMDAC (Random Access Memory Digital/Analog Converter) ist ein Chip der auf der Grafikkarte für die Umwandlung von digitalen Videosignalen zu analogen Bildsignalen verantwortlich ist. Er wird nur benötigt wenn ein Monitor beispielsweise über VGA angeschlossen wird.

Der PCI-Express-Steckplatz, an dem 16 Lanes angeschlossen sind (PCIe x16), wird zur Anbindung der Grafikkarte verwendet. Dieser wird auch als PCI-Express for Graphics (PEG) bezeichnet. Mit PCIe 3.0 ergibt sich eine theoretische Übertragungsrate von 15,75GB/s.

### Monitorschnittstelle

#### VGA – Video Graphics Array
![](./_static/Grafik_VGA.png)

Die VGA-Buchse ist 15-Polig. VGA stellt neben den analogen Bildsignalen für die drei Farbauszüge Rot, Grün und Blau separate horizontale und vertikale Synchronsignale bereit, die den Monitor steuern. Außerdem kann dem PC über ein zusätzliches VGA-Signal mitgeteilt werden, ob ein Monitor angeschlossen ist. Auch der Betriebszustand des Monitors kann geändert werden.

##### DVI – Digital Visual Interface

![](./_static/Grafik_VGA_type.png)

DVI bietet die Möglichkeit, unter Umgehung des RAMDAC der Grafikkarte digitale Videosignale direkt an einen angeschlossenen Monitor zu übergeben. Ein Buchsentyp mit 5 zusätzlichen Kontakten kann auch die bisherigen Analogsignale ausgeben („digital and analog“).

Die von der kombinierten Buchse ausgegebenen Analogsignale entsprechen den bisherigen VESA-Standards ab VGA.

DVI beherrscht darüber hinaus Plug & Play und Hot-Plugging (Automatische Erkennung eines Bildschirms und Anschluss von Bildschirmen im laufenden Betrieb). Beide Versionen unterscheiden sich nicht in Form und Abmessungen. Digitale Monitore mit DVI-Stecker können folglich an beide Typen von DVI-Buchsen angeschlossen werden.

Eine mit 24 Kontakten versehene DVI-Buchse stellt ausschließlich Digitalsignale zur Verfügung („digital only“).

#### HDMI – High Definition Multimedia Interface

![](./_static/Grafik_HDMI.png)

HDMI ist der Nachfolger von DVI Hier werden zusätzlich noch Audiosignale übertragen und der Kopierschutz HDCP hinzugefügt, der die Wiedergabe von HD-Inhalten auf dem Monitor zulässt. Praktischerweise ist HDMI auch rückwärtskompatibel, sodass man über einfache Adapter eine Verbindung zwischen Geräten mit DVI und HDMI herstellen kann.

#### HDMI-Buchse Typ A

In der Version 2.1 kann HDMI mit diversen Audio- und Videoformaten umgehen. Typ Breite x Höhe Pin Beschreibung.

A: Standard 15mm x 5,5mm 19 weit verbreiteter Standardstecker

B: Dual Link 21,3mm x 4,45mm 29 Dual-Link-fähig, nur im Profi-Bereich verbreitet

C: Mini 11,2mm x 3,2mm 19 per Adapter zu Typ A kompatibel

D: Micro 6,4mm x 2,8mm 19 noch kleiner als Micro-USB.

#### DisplayPort

![](./_static/Grafik_DP.png)

Mit DisplayPort wurden die Bandbreiten und Geschwindigkeiten kontinuierlich erhöht, um neue Auflösungen wie 4K/8K zu ermöglichen.

Im Gegensatz zu HDMI überträgt DisplayPort keine Toninformationen.

#### Thunderbolt

![](./_static/Grafik_TB.png)

Diese Schnittstelle ist der direkte Nachfolger von Mini DisplayPort. Sie ist mechanisch und elektrisch rückwartskompatibel mit Mini-DP.

Sie stellt nicht nur eine Videoverbindung dar, sondern überträgt Daten. Mit der Einführung von Thunderbolt 3 sind Übertragungen mit bis zu 40GBit/s über diesen Anschluss möglich. Intel nahm eine Steigerung auf 100GBit/s bis zum Jahr 2019 an. Damit steht Thunderbolt in direkter Konkurrenz zu USB 3.x, eSATA, FireWire, Gigabit-Ethernet und natürlich allen bisherigen digitalen Videoverbindungen. Intern kann Thunderbolt mit den Protokollen PCI Express oder DisplayPort arbeiten.

### Multiple Grafikausgabe

Sowohl der Multimonitorbetrieb mit mehreren Grafikkarten als auch Dual Head bzw. Multi Head mit einer einzelnen Karte müssen vom Betriebssystem und dem Grafikkartentreiber unterstützt werden. Dies ist bei Windows sowie Mac OS und Linux der Fall. Multi Head ist bei heutigen Grafikkarten Standard.