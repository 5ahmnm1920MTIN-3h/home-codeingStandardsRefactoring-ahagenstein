# home-codeingStandardsRefactoring-ahagenstein

## Ausarbeitung zu Refactoring

### Was ist Refactoring, Definition in eigenen Worten?
Refactoring soll einen Code kürzer und übersichtlicher machen und vor allem einfacher zu verstehen. Das wichtigste dabei ist jedoch, dass das Refactoring an der Funktion oder Verhaltensweise eines Programms nichts ändert, es soll jediglich das Programm, vor allem für Außenstehende welche nicht an dem Code arbeiten, klarer und verständlicher machen und ihn somit verbessern.

### Welche Vorteile/ Nachteile birgt Refactoring?
Vorteile: Code viel leichter lesbar, vor allem zukünftige Änderungen können einfacher vorgenommen werden und das Risiko, dass das Programm nach einer Änderung auf einmal nicht mehr funktioniert, wird minimiert da alles am Code viel klarer ist. Der gecleante Code ist meistens kürzer (ist auf das wichigste reduziert) wodurch einer bessere Performance des Prozesses ermöglicht wird (schnellerer Ablauf und weniger Unterbrechungen)

Nachteil: Refactoring kann auch schnell genau in die falsche Richtung gehen. Es kann passieren das der Code nicht mehr funktioniert/ Fehler entstehen und somit wird der Lauf des Prozesses unterbrochen. Es ist außerdem aufwendig und kann viel Zeit beanspruchen, obwohl das Endprodukt dasselbe bleibt.

## Was sind die Refactoring-Schritte?
- Testcase definieren und zu beginn schauen, ob es einwandfrei funktioniert (damit man es nachher nicht auf das Refactoring schieben kann)
- Fängt Teil des Codes an zu verbessern (bsp. leere Code Zeilen löschen oder Magic Values austauschen).
- Testcase wird getestet ob es noch immer so funktioniert wie es funktionieren soll bzw wie es vor dem Refactoring funktioniert hat
- Wenn ja, wird commit für Änderungen erstellt mit klarer Commit Message (git commit -m"Refactoring:...) auf gitHub.

### Prinzipien von guten Code?

- leicht lesbar
- verständlich für andere Personen
- keine Redundanzen
- funktioniert

DRY - Mehrfache Nennungen von Code verhindern - mit Variablen arbeiten

KISS - Der Code soll so einfach wie möglich gestaltet werden

YAGNI - "Extras", die nicht unbedingt für die Funktion des Programms nötig sind, sollen entfernt werden

Principle of Least Surprise - Die Funktionen sollten so sein, wie man es sich erwartet (keine Überraschungen)

SoC - Der Code sollte in klare Abschnitte gegliedert sein

Single Responsibility Principle - Klassen sollten nur für eine Sache zuständig sein und nicht mehrere Funktionen erfüllen

### Was versteht man unter Code Smell?

Unter Code Smell versteht man Teile des Codes, die nicht benötigt werden zum funktionieren bzw unnötig lange Teile des Codes welche man leicht verbessern/ löschen könnte. Das ist nicht ordentlich und wird oft sowieso nicht gebraucht. Ein Code Smell ist also ein "falscher" Code welcher zwar gleich funktioniert wie der cleande Code aber mit Code Smells ist der Code unordentlich, meist viel zu lange und sehr Fehleranfällig (also genau das Gegenteil von einem cleanen Code)

### Recherche von 10 Code Smells die Eure Projekt betreffen können, inkl. Beschreibung und Beispiel.

#### 1.  Kommentare    
- Kommentare sollen den Code unterstützen aber nicht mehr als der Code selber ausmachen, zu viele Kommentare sind auch nicht hilfreich

#### 2. Namen sollten Sinnbehaftet sein
- Variablen, Klassen, Methoden usw sollten so benannt werden, dass es Sinn ergibt und man davon die Funktion ablesen kann

#### 3. Redundanter Code
- Doppelter Code sollte vermieden werden, macht alles viel unübersichtlicher

#### 4. Zu lange Methoden
- Eine Methode soll nur eine Funktion erfüllen und nicht zuviele Zeilen Code beinhalten. Es sollte vor allem auf Grund der Verständlichkeit und Unübersichtlichkeit vermieden werden.

#### 5. Namen/ Bezeichnung zu kurz
- Methoden, Klassen und Variablen sollten mit Sinnbehafteten Namen benannt werden und nach dem Bennenungsstandard, nur einzelne Buchstaben machen keinen Sinn und führen zur unverständlichkeit des Codes

#### 6. Zu lange Namen
- Jedoch sind viel zu lange Namen auch nicht Sinnvoll und führen genau zum selben wie zu kurze Namen - Sinnbehaftete Namen sind wichtig!!

#### 7. Verschachtelungen
- Verschachtelungen erschweren die Lesbarkeit und Verständlichkeit sehr.

#### 8. Unnötige Leerzeilen
- Unnötige Leerzeilen sollten vermieden werden, weniger ist mehr. Leerzeilen sind oft unnötiger Verbrauch von Zeilen.

#### 9. Unbenutzer Code
- Unbenutzer Code sollte gelöscht werden, genau so wie ausgeblendeter Code wenn er nicht gebraucht wird. Führt zu mehr Übersicht.

#### 10. Falsche Klammern
- Kann passieren das es am Anfang noch funktioniert aber kann schnell zu fehlerhaften Code führen und im Nachhinein Probleme verursachen.

 


# Santa Run

### Project description: 
This is a simple 2D side-scroll game. The Santa runs from left to right and has to avoid some obstacles by jumping over them.
The game ends when the Santa hits an obstacle.  The goal is to avoid as many obstacles as possible.

### Development platform: 
Windows 10, Unity version 2019.1.14f1, Visual Studio Community 2017, Scripting Runtime Version: .NET 4.0

### Target platform: 
WebGl and Standalone, RefRes: 1920 * 1080


### Visuals: 
<div>
<img src = "./Screenshots/sketch-SantaRun.JPG" width = "500">
</div>

[![SANTA RUN](https://i9.ytimg.com/vi/2C74XxBkFfI/mq1.jpg?sqp=CNWnze8F&rs=AOn4CLBrmO-tJ3gQ2BNeMxvrmQcsIhhcgQ)](https://www.youtube.com/embed/2C74XxBkFfI "Santa RUN")

https://www.youtube.com/embed/2C74XxBkFfI

### Necessary setup/execution steps: 
For playing the game go to: 
* WebGL: https://hs-teaching.github.io/WegGL-SantaRun/
* Standalone (.exe): Clone project and publish as Standalone

For development: Clone this project. 

### Third party material: 
* This game is based on the game Santa Run developed by Raja Biswas in the Udemy-course Unity 2018 Game Developmen by Example 
[Unity 2018 Game Development by Example](https://www.udemy.com/course/unity-2d-game-development-by-example/).
* Sprites are used from https://www.gameart2d.com/santa-claus-free-sprites.html


### Project state: 
Program is working correctly, no errors, refactoring is needed.
Refactoring needed: 
* del not used namespaces
* del unused variables
* del needless debugs
* del needless comments
* del unused methods
* rename variables (coding standards)
* rename methods (coding standards)
* fix poor conditional clauses
* fix poor formating
* replace magic string
* replace magic number

### Limitations: 
Only one level is implemented. 

### Lessons Learned: 
* Create 2D Scenes
* Use Quads for moving Backgrounds (Textures instead of Sprites)
* Use Particle System for snowing effect.
* Use Scene Management for switching between Scenes
* Create and control Animations (Animation, Animator and Scripts)
* Use the singelton pattern
* Spawn objects
* Use UI elements and manipulate UI elements with scrips


Copyright by smeerws
