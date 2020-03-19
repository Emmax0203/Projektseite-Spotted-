# Projektseite: Spotted!

## Inhaltsverzeichnis

[ Einleitung](#Einleitung)

[ Spielidee](#Spielidee)

[ Die einzelnen Screens](#Screens)

[ Funktionen](#Funktionen)

[ MistakeFound](#MistakeFound)

[ Misclick](#Misclick)

[ Endgame](#Endgame)

[ Restart](#Restart)

[ Scoreboard](#Scoreboardfunktion)

[ Die Buttons](#Buttons)

[ Das Suchbild](#Suchbild)

[ Spielende](#Ende)

[ Das Scoreboard](#Scoreboard)

[ Schlusswort](#Schlusswort)


## Einleitung<a name="Einleitung"></a>

["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) ist eine App, welches wir im Rahmen des Informatikunterrichts des zweiten Halbjahres des 12. Jahrgangs programmiert haben. Wir haben dazu wieder die Plattform [code.org](https://studio.code.org/) verwendet, wobei wir diesmal AppLab benutzt haben, da dies wesentlich komplexer und fortgeschrittener als GameLab ist und auch die Anforderung an das neue Projekt war. Im Rahmen des Tutorials zu AppLab lernt man, ohne die Bausteine von [code.org](https://studio.code.org/) zu arbeiten und stattdessen eigenständig Code zu schreiben.

Als wir das Tutorial weitestgehend beendet hatten, haben wir uns wieder dazu entschlossen, ein Spiel zu programmieren, da wir bereits gute Erfahrungen damit gemacht hatten. Im Folgenden werden aus Übersichtsgründen teilweise nur einzelne Codeauszüge gezeigt, wenn ganze Abschnitte diesem entsprechen. Dann ist davon auszugehen, dass der folgende Code genauso aussieht und funktioniert.


## Spielidee<a name="Spielidee"></a>

["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) beinhaltet ein simples Suchbild mit 9 Fehlern. Im oberen Teil sieht man das Original, während im unteren Teil Details fehlen. Mithilfe der Maus kann man auf die Fehler im unteren Bild klicken, um diese zu spotten. Findet man alle 9 Fehler, hat man das Spiel erfolgreich abgeschlossen und landet unter Umständen mit neuer Bestzeit auf dem Scoreboard, klickt man jedoch zu häufig daneben, verliert man das Spiel und kann es von Neuem versuchen. In diesem Fall wird jedoch keine Zeit gemessen.


## Die einzelnen Screens<a name="Screens"></a>

Um die Übersicht zu wahren, haben wir viel Gebrauch von der neuen Funktion von AppLab gegenüber GameLab gemacht: Screens. Man kann verschiedene Screens anlegen und so einzelne Bestandteile der App gut strukturieren und gliedern. Durch simple Verknüpfungen über Buttons gelangt man von einem Screen zum nächsten. 

Bei ["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) gibt es insgesamt 5 Screens: Den WelcomeScreen, den man zu Beginn sieht, den GameScreen, auf welchem sich das Spiel befindet, und schließlich die beiden Enden des Spiels als GameOverScreen und CongratsScreen. Um den Ehrgeiz der Spieler zu wecken, habem wir zudem ein Scoreboard programmiert, welches auf dem ScoreboardScreen zu sehen. 

![WelcomeScreen](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/WelcomeScreen.PNG)

#### Der WelcomeScreen


![GameScreen](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/GameScreen.PNG)

#### Der GameScreen


![CongratsScreen](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/CongratsScreen.PNG)

#### Der CongratsScreen


![GameOverScreen](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/GameScreen.PNG)

#### Der GameOverScreen


![Scoreboard](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/ScoreboardScreen.PNG)

#### Das Scoreboard


## Funktionen<a name="Funktionen"></a>

Um nicht immer wieder denselben Code schreiben zu müssen, haben wir ein paar kleine Funktionen geschrieben, um nur diese bei Bedarf aufrufen zu müssen. Dies sind die MistakeFound - und die Misclick - Funktion sowie die Endgame -, Restart - und Scoreboard - Funktion. 

### MistakeFound<a name="MistakeFound"></a>

Die MistakeFound - Funktion beschränkt sich auf wenige Zeilen Code. Sie erhöht lediglich den Spotted - Counter um 1, um so den Überblick zu behalten, spielt einen Sound zur Bestätigung ab und ändert den Text über dem Suchbild, sodass man jederzeit nachschauen kann, wie viele Fehler man gefunden hat und wie viele noch fehlen.

![Spottedfunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Spottedfunktion.PNG)


### Misclick<a name="Misclick"></a>

Auch die Misclick - Funktion ist kurz gehalten. Innerhalb dieser Funktion wird dem Spieler wegen des Misclicks ein Leben abgezogen, der entsprechende Sound zur akustischen Bestätigung ausgegeben und der Text über dem Spielfeld geändert, sodass man stets weiß, wie viele Fehler man sich noch erlauben kann. Die Spielmechanik der Leben bzw. des Misclicks haben wir eingeführt, um zu verhindern, dass der Spieler einfach wahllos auf dem Suchbild herumklickt und so durch Zufall Fehler findet, sondern stattdessen wirklich sucht und nur klickt, wenn er sich sicher ist, dass er einen Fehler gefunden hat. 

![Misclickfunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Misclickfunktion.PNG)


### Endgame<a name="Endgame"></a>

Diese Funktion wird unter ["Spielende"](#Spielende) erklärt.


### Restart<a name="Restart"></a>

Nachdem das Spiel beendet ist, kann man natürlich das Spiel ein weiteres Mal spielen. Dazu müssen alle Buttons erneut auf dem Spielfeld erscheinen, der genaue Grund wird bei "Das Suchbild"(#Suchbild) ausgeführt. Zudem müssen sowohl der Lives - Counter als auch der 
Spotted - Counter zurückgesetzt werden. Desweiteren muss natürlich auch die Zeit von Neuem gemessen werden und die Texte, die die Anzahl verbleibender Fehler und Leben anzeigt, aktualisiert werden.

![Restartfunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Restartfunktion.PNG)


### Scoreboard<a name="Scoreboardfunktion"></a>

Diese Funktion erklären wir seperat bei ["Das Scoreboard"](#Scoreboard).



## Die Buttons<a name="Buttons"></a>


Mithilfe der Buttons kann man im Spiel von einem Screen zum nächsten gelangen. Dazu gibt es den Start-Button auf dem WelcomeScreen sowie die Restart-Buttons auf den SpielendeScreens und dem Scoreboard, um den GameScreen aufzurufen. Findet man alle Fehler, kann man über einen Button vom CongratsScreen das Scoreboard anschauen. Dazu haben wir onEvent - Befehle verwendet, bei denen der Screen über den setScreen - Befehl gewechselt wird. Wie im Bild zu sehen ist, wird bei jedem RestartButton die [Restartfunktion](#Restart) aufgerufen, die bereits weiter oben im Code definiert wurde und auch hier bereits erklärt wurde.

![RestartButtons](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Restartbuttons.PNG)

Die Ausnahme bildet der ScoreboardButton, da dieser noch initiiert, dass die Top 5 der schnellsten Sucher in der richtigen Reihenfolge angezeigt werden. Details dazu unter ["Das Scoreboard"](#Scoreboard).

Zudem wird bei dem StartButton die Zeitmessung gestartet, um die Zeit mssen zu können, die zum Finden aller Fehler gebraucht wird.


## Das Suchbild<a name="Suchbild"></a>

Das Suchbild ist der Hauptbestandteil von ["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU). Das Suchbild haben wir aus dem Internet importiert und zunächst selbst alle Fehler gesucht. Anschließend haben wir die Fehler mit Buttons markiert, sodass sie vollständig von Buttons bedeckt sind. Dadurch kann ein Fehler bei Anklicken des Buttons gefunden werden. Da wir 9 Fehler im Bild haben, haben wir 9 Buttons mit den Namen F1 - F9 eingeführt. Jeder Button hat denselben Code, der beim Anklicken abgerufen wird. 

![F1ButtonCode](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/F1%20Button.PNG)

Zudem ist das ganze untere Bild vom MisclickButton abgedeckt, sodass bei einem Misclick dieser Button getroffen wird. Dadurch kann das Spiel eindeutig feststellen, was angeklickt wird, ohne ein Leben abgezogen wird, wenn außerhalb des unteren Bilds geklickt wird. 

Damit man nicht immer auf denselben Fehler klicken kann, um auf 9 gefundene Fehler zu kommen, verschwinden die Buttons, die die Fehler markieren, nach dem Klicken. Dadurch sind sie nur für einmaliges Klicken verfügbar und jeder Fehler muss gefunden werden, um das Spiel erfolgreich abzuschließen. 


## Spielende<a name="Ende"></a>




## Das Scoreboard<a name="Scoreboard"></a>

Diese Funktion ist schon wesentlich umfangreicher als die beiden vorangegangenen. Diese Funktion beendet das Spiel. Sie prüft, ob mit dem aktuellen Klick entweder der letzte Fehler gefunden wurde oder das letzte Leben abgezogen wurde. 

Sollte der letzte Fehler gefunden worden


## Schlusswort<a name="Schlusswort"></a>


