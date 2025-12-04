# Lern-Periode-12
07.11.2025 bis 19.12.2025


## Projektordner
[Narrow-Roll-Game](https://github.com/Fynn8962/Narrow-Roll-Game)

&nbsp;

## Planung

### Technologien
Für die Lern-Periode-12 möchte ich meinen Fokus das Arbeiten mit Unity und C# legen. Der Grund dafür ist die Vorbereitung auf mein IMS-Praktikum, in welchem ich im Bereich interaktive Technologie arbeiten werde. Mit Unity und C# möchte ich ein 3D Spiel erstellen, mit dem Ziel den Entwicklungsprozess von Unity besser zu verstehen von der Szenendarstellung, Physik und UI-Implementation bis hin zu Code und Dokumentation. 

&nbsp;

### Projektantrag
Ich möchte ein einfaches 3D Spiel mittels Unity und C# umsetzen. Das Spiel soll eine einfache Spielmechanik beinhalten. Der Fokus liegt hierbei eher auf dem Verstehen des Codes (Code Kommentare) und der Funktionen von Unity sowie  dem strukturierten  Dokumentieren der Arbeit. Das Ziel ist erste Erfahrungen mit Unity in Bezug auf 3D Entwicklung zu machen und einen funktionsfähigen Prototyp zu erstellen, welcher technisch durch eine Dokumentation gut nachvollziehbar ist. 

 
**Spiel Idee**                        
Der Spieler steuert eine Kugel, wobei diese nicht einfach zu kontrollieren ist, da sie über schmale Wege mit Hindernissen geführt werden muss. Das Ziel besteht darin, den Zielpunkt zu erreichen, ohne herunterzufallen. Dabei wird die Zeit gestoppt, sodass man versuchen kann, seine eigene Bestzeit zu unterbieten. Je nach Zeit und Machbarkeit können verschiedene Level mit unterschiedlichen Schwierigkeitsgraden ausgewählt werden.

&nbsp;

### Epics

- [x] Als Entwickler möchte ich mich mit Unity zurechtfinden und die Projektstruktur sowie Assets gründlich aufbauen.

- [x] Als Spieler möchte ich die Kugel mit der Tastatur steuern können, um mich über die Wege bewegen zu können.

- [x] Als Spieler möchte ich eine realistische Physiksteuerung der Kugel, damit sich die Bewegung herausfordernd und glaubwürdig anfühlt.

- [ ] Als Spieler möchte ich verschiedene Level mit ansteigendem Schwierigkeitsgrad auswählen können, um mich schrittweise zu verbessern.

- [ ] Als Spieler möchte ich eine Zeitmessung sehen, um Bestzeiten vergleichen und mich selbst herausfordern zu können.

- [x] Als Spieler möchte ich verlieren, wenn ich von der Strecke falle, damit das Spiel Ziel und Spannung hat.

- [ ] Als Spieler möchte ich ein einfaches Menü haben, um Level zu starten, neu zu beginnen oder das Spiel zu beenden, damit die Bedienung übersichtlich bleibt.

(Als Entwickler möchte ich Code und Projektstruktur klar dokumentiert und verständlich halten, damit andere (und ich selbst) das Projekt nachvollziehen und ausführen können.)

&nbsp;

&nbsp;

## 07.11.2025

**Epic:** Als Entwickler möchte ich mich mit Unity zurechtfinden und die Projektstruktur sowie Assets gründlich aufbauen.

**Arbeitspakete**
- [x] Unity-Oberfläche zusammen mit einem 3D-Objekt verstehen
- [x] Projektstruktur aufbauen (Projektmappe, Ordnerstruktur, Szenen)
- [x] Ressourcen (Assets) finden für das Projekt
- [x] Assets anwenden, lernen wie man in 3D mit Assets arbeiten

&nbsp;

**Heute habe ich...**                                                 
Zuerst habe ich ein neues Projekt erstellt und mich mit der Umgebung vertraut gemacht. Ich musste ein Tutorial anschauen um zu verstehen, was die verschiedenen Bereiche (Hirarchy, Project, Inspector) usw. alles bedeuten. Danach habe ich eine Struktur angelegt, z. B. den Ordner, in welchen in die Texturen verwalte. Anschliessend habe ich Unity eigene Objekte (cube, Shpere) hinzugefügt, um einen Boden und eine Kugel zu haben. Anhand eines Tutorials habe ich dann Texturen gefunden (Assets) und gelernt, wie man mit den Parametern, die man verstellen kann, umgeht. Dadurch habe ich eine erste kleine Spieloberfläche gebaut, mit einigermassen passenden Texturen. 


&nbsp;

&nbsp;

## 14.11.2025

**Epic:** Als Spieler möchte ich die Kugel mit der Tastatur steuern können, um mich über die Wege bewegen zu können.

**Arbeitspakete**
- [x] Das Steuerungsskript in C# für die Tastensteuerung der Kugel
- [x] kamera einstellen dass Kugel verfolgt wird
- [x] Herumschauen ermöglichen und Bewegung je nach Blickrichtung anpassen
- [x] Rein und Raus zoomen der Kamere für bessere übersicht.

&nbsp;

**Heute habe ich...**                    
Zuerst habe ich mich um die Tastatursteuerung der Kugel gekümmert. Da ich mit Unity 6 arbeite, habe ich ein `Input Action Asset` erstellt, mit welchem ich eine `Action` names Move erstellt habe, in welcher die Tasten WASD belegt werden. Die Aktion wird im Code ausgelesen und dann zur Bewegung der Kugel verwendet.

Damit die Kugel nicht der Kamera davonfährt, musste ich eine Third-Person Kamera erstellen. Um diesen Prozess zu vereinfachen habe ich das `Cinemachine Package` verwendet, welches ein Kamerasystem ist zur Kontrolle der Unity Kamera. Nach Hinzufügen des "Tracking Target" und des "Input Controllers" funktionierte das Herumschauen um die Kugel schon. Jedoch fehlt die Funktion für das Zoomen, dafür habe ich mithilfe eines Tutorials ein Script für den Third-Person Kamerazoom erstellt. Dadurch kann der Spieler je nach Präferenz den Abstand zur Kugel einstellen.

>Derzeitiges Problem ist noch das verhalten der Steuereum beim Umschauen der Kamera, soll die Kugel auf Ihrer Bahn bleiben, oder Ihre Richtung der Kamera anpassen. Im laufe der Entwicklung werde ich Testen, welches verhalten sich besser anfühlt.



&nbsp;

&nbsp;

## 21.11.2025

**Epic:** Als Spieler möchte ich eine realistische Physiksteuerung der Kugel, damit sich die Bewegung herausfordernd und glaubwürdig anfühlt.

**Arbeitspakete**
- [x] Trägheitsbasierte Steuerung einbauen, damit das Spielerlebnis schwieriger ist.
- [x] Physik der Kugel anpassen, Fallen, Bouncen, Apprallen.
- [x] Testelemte Bauen um zu Testen wie sich die Kugel in Situationen verhählt (runterfallen auf Plattform, hohe Geschwindigkeit, Steile steigung
- [x] Erste Teststrecke bauen um sicherzustellen, dass weitere Änderungen ein einem realen Szenario funktinieren.

&nbsp;

**Heute habe ich...**                         
Ich habe mich heute mit der Physik der Kugel beschäftigt. Für die Physik brauche ich `Rigidbody`, jedoch ist dieses Component nicht kompatibel mit dem `Character Controller`, daher musste ich das Skript so umschreiben, dass die Komponenten-Referenz nicht auf CharacterControll, sondern auf Rigidbody bezieht. Anschliessend habe ich die Physik der Kugel implementiert, damit ein Trägheitsgefühl vorhanden ist in der Steuerung. Dieses Trägheitsgefühl wird mit verschiedenen Parametern wie:          

- `sphereMass` --> Bestimmt, wie viel Kraft nötig ist, um die Kugel zu beschleunigen oder zu stoppen
- `Drag`/`LinearDamping` --> Luft- bzw. Bewegungswiederstand. Höherer Drag reduziert die Geschwindigkeit schneller und macht die Steuerung stabiler.
- `AngularDrag` --> Widerstand gegen Rotation, beeinflusst wie schnell die Kugel ihre Rollbewegung abbaut.
- `MoveForce` --> Grundkraft, mit der die Kugel beschleunigt wird. Hat Einfluss auf die Reaktionsfähigkeit des Balles.

Durch diese und weitere Parameter wird eine möglichst realistische Kugelsteuerung ermöglicht, welche es möglichst realistisch machen sollte.

Da es viele Werte sind, habe ich viel Zeit verbracht, diese aufeinander anzupassen für eine möglichst angenehme, fordernde und realistische Steuerung. Dafür habe ich verschieden Parkourszenarion wie Steigungen, Schräglagen oder Drops gebaut und getestet. Ich bin immer noch nicht überzeugt von der Steuerung und werde in der Schule nach Feedback fragen von Kollegen, da ich durch das ganze einstellen mit der Zeit das Gefühl verloren habe, was sich nun besser oder schlechter anfühlt.



&nbsp;

&nbsp;

## 28.11.2025

**Epic:** Als Spieler möchte ich verlieren, wenn ich von der Strecke falle, damit das Spiel Ziel und Spannung hat.


**Arbeitspakete**
- [x] Hinzufügen der Logik zur Erkennung, wenn der Ball die Strecke verlässt und herunterfällt. 
- [x] Implementieren des automatischen Zurücksetzens des Balles zur Startposition nach einem Sturz.
- [x] Hinzufügen einer Taste- und UI-Reset Funktion, um während des Spielens zurück zum Start zu gelangen. 
- [ ] Einbauen eines visuellen/akustischen Effekts beim Herunterfallen und Zurücksetzen.

&nbsp;

**Heute habe ich...**                 
Ich habe ein Skript hinzugefügt namens GameRespawn, dieses Script löst aus, wenn der Y-Wert der Kugel unter einen gewissen Wert liegt, was bedeutet, dass der Spieler heruntergefallen ist. Zusätzlich dazu habe ich im PlayerController Skript eine neue Funktion hinzugefügt, welche, wenn der Spieler die Taste `R` drückt, die Kugel auch zurücksetzt. Für dies habe ich in meiner Gameplay Action Map eine neue Action names `Reset` hinzugefügt, welche die Taste `R` benutzt. Für eine UI-Implementierung habe ich mich vorerst dagegen entschieden und werde diese hinzufügen, wenn ich das restliche UI des Games erstellen werde. 

Als Letztes wollte ich noch hinzufügen, dass die Kamera sich zurücksetzt, wenn die Kugel zurückgesetzt wird, damit diese wieder in die richtige Richtung schaut, jedoch funktioniert dies noch nicht aus noch nicht herausgefundenen Gründen. Diese werde ich versuchen, in der nächsten Sitzung zu beheben. 

Durch Probleme mit dem Zurücksetzen der Kamerarichtung hatte ich keine Zeit mehr das visuelle / akustische Feedback einzufügen, dies werde ich zu einem späteren Zeitpunkt, wahrscheinlich wenn ich das UI implementiere, hinzufügen.

>derzeitige Probleme:                         
> - Die Kamera schaut noch nicht in die richtige Richtungwenn die Kugelpostion zurückgesetzt wird.
> - Das Manuele Zurücksetzen funktioniert noch nicht einwandfrei bei zu schnellem Drücken.

&nbsp;

&nbsp;

## 05.12.2025

**Epic:** Als Spieler möchte ich eine Zeitmessung sehen, um Bestzeiten vergleichen und mich selbst herausfordern zu können.

**Arbeitspakete**
- [ ] xxx
- [ ] xxx
- [ ] xxx
- [ ] xxx

&nbsp;

**Heute habe ich...**
