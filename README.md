# Projektseite: Spotted!

## Inhaltsverzeichnis

[1. Einleitung](#Einleitung)

[2. Spielidee](#Spielidee)

[3. Die einzelnen Screens](#Screens)

[4. Funktionen](#Funktionen)

[5. Die Buttons](#Buttons)

[6. Das Suchbild](#Suchbild)

[7. Spielende](#Ende)

[8. Das Scoreboard](#Scoreboard)

[9. Schlusswort](#Schlusswort)


## Einleitung<a name="Einleitung"></a>

"Spotted!" ist eine App, welches wir im Rahmen des Informatikunterrichts des zweiten Halbjahres des 12. Jahrgangs programmiert haben. Wir haben dazu wieder die PLattform code.org verwendet, wobei wir diesmal AppLab benutzt haben, da dies wesentlich komplexer und fortgeschrittener als GameLab ist und auch die Anforderung an das neue Projekt war. Im Rahmen des Tutorials zu AppLab lernt man, ohne die Bausteine von code.org zu arbeiten und stattdessen eigenständig Code zu schreiben.

Als wir das Tutorial weitestgehend beendet hatten, haben wir uns wieder dazu entschlossen, ein Spiel zu programmieren, da wir bereits gute Erfahrungen damit gemacht hatten. Im Folgenden werden aus Übersichtsgründen teilweise nur einzelne Codeauszüge gezeigt, wenn ganze Abschnitte diesem entsprechen. Dann ist davon auszugehen, dass der folgende Code genauso aussieht und funktioniert.


## Spielidee<a name="Spielidee"></a>

"Spotted!" beinhaltet ein simples Suchbild mit 9 Fehlern. Im oberen Teil sieht man das Original, während im unteren Teil Details fehlen. Mithilfe der Maus kann man auf die Fehler im unteren Bild klicken, um diese zu spotten. Findet man alle 9 Fehler, hat man das Spiel erfolgreich abgeschlossen und landet unter Umständen mit neuer Bestzeit auf dem Scoreboard, klickt man jedoch zu häufig daneben, verliert man das Spiel und kann es von Neuem versuchen. In diesem Fall wird jedoch keine Zeit gemessen.


## Die einzelnen Screens<a name="Screens"></a>

Um die Übersicht zu wahren, haben wir viel Gebrauch von der neuen Funktion von AppLab gegenüber GameLab gemacht: Screens. Man kann verschiedene Screens anlegen und so einzelne Bestandteile der App gut strukturieren und gliedern. Durch simple Verknüpfungen über Buttons gelangt man von einem Screen zum nächsten. 

Bei "Spotted!" gibt es insgesamt 5 Screens: Den WelcomeScreen, den man zu Beginn sieht, den GameScreen, auf welchem sich das Spiel befindet, und schließlich die beiden Enden des Spiels als GameOverScreen und CongratsScreen. Um den Ehrgeiz der Spieler zu wecken, habem wir zudem ein Scoreboard programmiert, welches auf dem ScoreboardScreen zu sehen. 


## Funktionen<a name="Funktionen"></a>




## Die Buttons<a name="Buttons"></a>


Mithilfe der Buttons kann man im Spiel von einem Screen zum nächsten gelangen. Dazu gibt es den Start-Button auf dem WelcomeScreen sowie die Restart-Buttons auf den SpielendeScreens und dem Scoreboard, um den GameScreen aufzurufen. Findet man alle Fehler, kann man über einen Button vom CongratsScreen das Scoreboard anschauen. Dazu haben wir onEvent - Befehle verwendet, bei denen der Screen über den setScreen - Befehl gewechselt wird.


## Das Suchbild<a name="Suchbild"></a>

Das Suchbild ist der Hauptbestandteil von "Spotted!". Das Suchbild haben wir aus dem Internet importiert und zunächst selbst alle Fehler gesucht. Anschließend haben wir die Fehler mit Buttons markiert, sodass sie vollständig von Buttons bedeckt sind. Dadurch kann ein Fehler bei Anklicken des Buttons gefunden werden. Da wir 9 Fehler im Bild haben, haben wir 9 Buttons mit den Namen F1 - F9 eingeführt. Jeder 


## Spielende<a name="Ende"></a>




## Das Scoreboard<a name="Scoreboard"></a>




## Schlusswort<a name="Schlusswort"></a>


