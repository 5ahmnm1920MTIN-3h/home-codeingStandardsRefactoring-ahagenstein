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



 
