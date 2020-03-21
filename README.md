# Projektseite: Spotted!

## Inhaltsverzeichnis

[1. Einleitung](#Einleitung)

[2. Spielidee](#Spielidee)

[3. Die einzelnen Screens](#Screens)

[4. Funktionen](#Funktionen)

[4.1. MistakeFound](#MistakeFound)

[4.2. Misclick](#Misclick)

[4.3. Endgame](#Endgame)

[4.4. Restart](#Restart)

[4.5. Scoreboardfunktion](#4)

[5. Die Buttons](#Buttons)

[6. Das Suchbild](#Suchbild)

[7. Spielende](#Ende)

[8. Das Scoreboard](#Scoreboard)

[9. Schlusswort](#Schlusswort)


## Einleitung<a name="Einleitung"></a>

["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) ist eine App, welche wir im Rahmen des Informatikunterrichts des zweiten Halbjahres des 12. Jahrgangs programmiert haben. Wir haben dazu wieder die Plattform [code.org](https://studio.code.org/) verwendet, wobei wir diesmal AppLab zum Programmmieren benutzt haben, da dies wesentlich komplexer und fortgeschrittener als GameLab ist und dies zudem auch die Anforderung an das neue Projekt war. Im Rahmen des Tutorials zu AppLab lernt man auch, ohne die Bausteine von [code.org](https://studio.code.org/) zu arbeiten und stattdessen eigenständig Codezeilen zu schreiben.

Als wir das Tutorial weitestgehend beendet hatten, haben wir uns wieder dazu entschlossen, ein Spiel zu programmieren, da wir bereits gute Erfahrungen damit gemacht hatten. Im Folgenden werden aus Übersichtsgründen teilweise nur einzelne Codeauszüge gezeigt, wenn ganze Abschnitte diesem entsprechen. Dann ist davon auszugehen, dass der folgende Code genauso aussieht und funktioniert.


## Spielidee<a name="Spielidee"></a>

["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) beinhaltet ein simples Suchbild mit neun Fehlern. Im oberen Teil sieht man das Original, während im unteren Teil Details fehlen. Mithilfe der Maus kann man auf die Fehler im unteren Bild klicken, um diese zu spotten. Findet man alle neun Fehler, hat man das Spiel erfolgreich abgeschlossen und landet unter Umständen mit neuer Bestzeit auf dem [Scoreboard](#Scoreboard), klickt man jedoch zu häufig daneben, verliert man das Spiel und kann es von Neuem versuchen. In diesem Fall wird jedoch keine Zeit gemessen.


## Die einzelnen Screens<a name="Screens"></a>

Um die Übersicht zu wahren, haben wir viel Gebrauch von der neuen Funktion von AppLab gegenüber GameLab gemacht: [Screens](#Screens). Man kann verschiedene [Screens](#Screens) anlegen und so einzelne Bestandteile der App gut strukturieren und gliedern. Durch simple Verknüpfungen über [Buttons](#Buttons) gelangt man von einem [Screen](#Screens) zum nächsten. 

Bei ["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) gibt es insgesamt fünf [Screens](#Screens): Den WelcomeScreen, den man zu Beginn sieht, den GameScreen, auf welchem sich das Spiel befindet, und schließlich die beiden Enden des Spiels als GameOverScreen und CongratsScreen. Um den Ehrgeiz der Spieler zu wecken, haben wir zudem ein [Scoreboard](#Scoreboard) programmiert, welches auf dem ScoreboardScreen zu sehen ist. 

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

Um nicht immer wieder denselben Code schreiben zu müssen, haben wir ein paar kleine Funktionen geschrieben, um nur diese bei Bedarf aufrufen zu müssen. Dies sind die [MistakeFound](#MistakeFound) - und die [Misclick - Funktion](#Misclick) sowie die [Endgame](#Endgame) -, [Restart](#Restart) - und [Scoreboard - Funktion](#Scoreboard). 

### MistakeFound<a name="MistakeFound"></a>

Die [MistakeFound - Funktion](#MistakeFound) beschränkt sich auf wenige Zeilen Code. Sie erhöht lediglich den Spotted - Counter um 1, um so den Überblick zu behalten, spielt einen Sound zur Bestätigung ab und ändert den Text über dem [Suchbild](#Suchbild), sodass man jederzeit nachschauen kann, wie viele Fehler man gefunden hat und wie viele noch fehlen.

![Spottedfunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Spottedfunktion.PNG)


### Misclick<a name="Misclick"></a>

Auch die [Misclick - Funktion](#Misclick) ist kurz gehalten. Innerhalb dieser Funktion wird dem Spieler wegen des Misclicks ein Leben abgezogen, der entsprechende Sound zur akustischen Bestätigung ausgegeben und der Text über dem Spielfeld geändert, sodass man stets weiß, wie viele Fehler man sich noch erlauben kann. Die Spielmechanik der Leben bzw. des Misclicks haben wir eingeführt, um zu verhindern, dass der Spieler einfach wahllos auf dem Suchbild herumklickt und so durch Zufall Fehler findet, sondern stattdessen wirklich sucht und nur klickt, wenn er sich sicher ist, dass er einen Fehler gefunden hat. 

![Misclickfunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Misclickfunktion.PNG)


### Endgame<a name="Endgame"></a>

Diese Funktion wird unter ["Spielende"](#Spielende) erklärt.


### Restart<a name="Restart"></a>

Nachdem das Spiel beendet ist, kann man natürlich das Spiel ein weiteres Mal spielen. Dazu müssen alle [Buttons](#Buttons) erneut auf dem [Spielfeld](#Suchbild) erscheinen, der genaue Grund wird bei ["Das Suchbild"](#Suchbild) ausgeführt. Zudem müssen sowohl der Lives - Counter als auch der 
Spotted - Counter zurückgesetzt werden. Desweiteren muss natürlich auch die Zeit von Neuem gemessen werden und die Texte, die die Anzahl verbleibender Fehler und Leben anzeigt, aktualisiert werden.

![Restartfunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Restartfunktion.PNG)


### Scoreboard

Diese Funktion erklären wir seperat bei ["Das Scoreboard"](#Scoreboard).



## Die Buttons<a name="Buttons"></a>


Mithilfe der [Buttons](#Buttons) kann man im Spiel von einem [Screen](#Screens) zum nächsten gelangen. Dazu gibt es den Start-Button auf dem WelcomeScreen sowie die Restart-Buttons auf den SpielendeScreens und dem [Scoreboard](#Scoreboard), um den GameScreen aufzurufen. Findet man alle Fehler, kann man über einen [Button](#Buttons) vom CongratsScreen das [Scoreboard](#Scoreboard) anschauen. Dazu haben wir onEvent - Befehle verwendet, bei denen der Screen über den setScreen - Befehl gewechselt wird. Wie im Bild zu sehen ist, wird bei jedem RestartButton die [Restartfunktion](#Restart) aufgerufen, die bereits weiter oben im Code definiert wurde und auch hier bereits erklärt wurde.

![RestartButtons](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Restartbuttons.PNG)

Die Ausnahme bildet der ScoreboardButton, da dieser noch initiiert, dass die Top 5 der schnellsten Sucher in der richtigen Reihenfolge angezeigt werden. Details dazu unter ["Das Scoreboard"](#Scoreboard).

Zudem wird bei dem StartButton die Zeitmessung gestartet, um die Zeit messen zu können, die zum Finden aller Fehler gebraucht wird.


## Das Suchbild<a name="Suchbild"></a>

Das [Suchbild](#Suchbild) ist der Hauptbestandteil von ["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU). Das [Suchbild](#Suchbild) haben wir [aus dem Internet](https://www.google.com/search?q=finde+den+fehler+suchbild&rlz=1C1CHBF_deDE884DE884&source=lnms&tbm=isch&sa=X&ved=2ahUKEwiVvKX24KvoAhXJ0KQKHXM2DqMQ_AUoAXoECAwQAw&biw=1920&bih=969#imgrc=6Nwu1fCRoTiWoM) importiert und zunächst selbst alle Fehler gesucht. Anschließend haben wir die Fehler mit [Buttons](#Buttons) markiert, sodass sie vollständig von [Buttons](#Buttons) bedeckt sind. Dadurch kann ein Fehler bei Anklicken des [Buttons](#Buttons) gefunden werden. Da wir neun Fehler im Bild haben, haben wir neun [Buttons](#Buttons) mit den Namen F1 - F9 eingeführt. Jeder [Button](#Buttons) hat denselben Code, der beim Anklicken abgerufen wird. Beim Klicken wird jedes Mal mit der [Endgame - Funktion](#Endgame) geprüft, ob das Spiel zu Ende ist sowie die [MistakeFound - Funktion](MistakeFound) abgerufen. 

![Suchbild mit sichtbaren Buttons](https://github.com/AntoniaJohannes/Stundenprotokoll-2/blob/master/Suchbild%20Fehler%20Markiert.PNG)

#### Das Suchbild mit den Buttons auf den Fehlern

![F1ButtonCode](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/F1%20Button.PNG)

#### Code für die FehlerButtons, exemplarisch F1


Zudem ist das ganze untere Bild vom MisclickButton abgedeckt, sodass bei einem Misclick dieser [Button](#Buttons) getroffen wird. Dadurch kann das Spiel eindeutig feststellen, was angeklickt wird, ohne dass ein Leben abgezogen wird, wenn außerhalb des unteren Bilds geklickt wird. 

![MisclickButton Code](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/MisclickButton.PNG)

Damit man nicht immer auf denselben Fehler klicken kann, um auf neun gefundene Fehler zu kommen, verschwinden die [Buttons](#Buttons), die die Fehler markieren, nach dem Klicken. Dadurch sind sie nur für einmaliges Klicken verfügbar und jeder Fehler muss gefunden werden, um das Spiel erfolgreich abzuschließen. 


## Spielende<a name="Ende"></a>
Das Spiel endet in zwei verschiedenen Szenarien: Entweder der Spieler drückt zu oft daneben und verliert seine drei Leben. Dann erscheint der GameOverScreen und er kann es von Neuem versuchen.
Oder der Spieler findet erfolgreich alle neun Fehler, sodass das Spiel gewonnen ist. Dann erscheint der CongratsScreen mit der Möglichkeit, nachzuschauen, ob die eigene Zeit unter den Top 5 Bestzeiten liegt. Je nach Spielende wird ein entsprechender Sound abgespielt, um eine ansprechende Audioausgabe zu haben. 

![Endgamefunktion](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Endgamefunktion.PNG)

Um die Spielenden vernünftig im Spiel integrieren zu können, haben wir die [Endgamefunktion](#Endgame) eingeführt. Sie besteht aus zwei 
if - Schleifen, die gleichzeitig prüfen, ob der Spieler den neunten Fehler gefunden oder sein letztes Leben verloren hat. Sollte eine der Möglichkeiten eintreten, beendet die [Endgamefunktion](#Endgame) auf die entsprechende Weise das Spiel. 

Um die Spielzeit zu messen, wurde ja bereits die Zeit mit dem Klick auf den StartButton gestartet. Nun, mit dem Klick auf den neunten Fehler, wird die Zeit gestoppt und die Differenz der beiden Zeitpunkte gebildet, um die Spielzeit zu erhalten. Um die Spielzeit nicht in Millisekunden, sondern in Sekunden zu erhalten, rechnen wir die Playtimevariable noch in Sekunden um mit Playtime/1000, um sie als Seconds angemessen ausgeben zu können.


## Das Scoreboard<a name="Scoreboard"></a>

Jedes gute Spiel hat ein [Scoreboard](#Scoreboard). Und so haben auch wir uns dazu entschlossen, eines in unser Spiel einzubauen. Dies gestaltete sich jedoch schwieriger als erwartet. 
Zunächst legten wir einen neuen [Screen](#Screens) an, den HighscoreScreen. Im Anschluss haben wir uns Gedanken dazu gemacht, wie ein [Scoreboard](#Scoreboard) eigentlich funktioniert. Herausgekommen ist letzten Endes diese Funktion:

![Scoreboard Funktion 1](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Scoreboardfunktion1.PNG)

![Scoreboard Funktion 2](https://github.com/AntoniaJohannes/Projektseite-Spotted-/blob/master/Scoreboardfunktion2.PNG)

#### Die Scoreboardfunktion

Der erste Teil dieser Funktion behandelt die Ausgabe des [Scoreboards](#Scoreboard) auf dem ScoreboardScreen. Bei erfolgreichem Abschluss wird der Counter "Games" um 1 erhöht, um zu ermitteln, wie viele Spiele bereits erfolgreich abgeschlossen wurden. Je nach Anzahl wird die entsprechende Anzahl Plätze auf dem [Scoreboard](#Scoreboard) angezeigt. Erst bei fünf Spielen werden alle fünf Plätze angezeigt. Dies hat einen Grund: Durch den Code werden teilweise Zeiten zweimal auf dem [Scoreboard](#Scoreboard) eingetragen, teilweise sogar in der falschen Reihenfolge. Doch durch die Reduzierung der angezeigten Plätze wird die Dopplung von wenigen Zeiten umgangen, da dieser zwar auf dem [Scoreboard](#Scoreboard) vorhanden sind, jedoch auf dem Screen nicht für den Spieler sichtbar sind. 

Um jedoch nicht nur einfach eine Zeit nach der anderen chronologisch auf dem [Scoreboard](#Scoreboard) einzutragen, sondern auch die Reihenfolge nach Schnelligkeit zu ermitteln, prüft der zweite Teil der Scoreboardfunktion die Zahlenwerte der aktuellen Spielzeit im Vergleich mit den bereits eingetragenen Spielzeiten auf dem [Scoreboard](#Scoreboard). Dazu haben wir einen Array verwendet, der fünf Plätze für die Top 5 hat. 
Nun vergleicht die Funktion die Spielzeit mit den einzelnen Plätzen. Wenn eine Zeit zwischen zwei bereits eingetragenen Zeiten liegt, wird sie zwischen diese Zeiten eingeschoben und der Rest wird nach hinten raus um einen nach unten versetzt. Dadurch wird der Array natürlich länger als fünf Plätze. Durch die visuelle Ausgabe der ersten fünf sind die darunterliegenden Zeiten jedoch irrelevant. So kann der Array theoretisch ins Unendliche wachsen, das [Scoreboard](#Scoreboard) wird stets ausschließlich die Top 5 anzeigen.

Zum ScoreboardScreen gelangt man über den ScoreboardButton auf dem CongratsScreen. Auf dem ScoreboardScreen befindet sich ein PlayAgainButton, mit welchem man das Spiel neu starten kann.


## Schlusswort<a name="Schlusswort"></a>

Abschließend können wir mit ein wenig Stolz von uns behaupten, mit ["Spotted!"](https://studio.code.org/projects/applab/QcTGX701NMCFbWlbQdbyFKavp3incRN2BAAxgA9jyGU) wieder ein für unsere Verhältnisse sehr tolles Spiel programmiert zu haben, da wir vor einem Dreivierteljahr keinerlei Kenntnisse hatten und uns alles selbst erarbeitet haben. Nachdem es mit GameLab alles super funktioniert hatte, lief auch mit AppLab alles wie am Schnürchen, wobei natürlich die Einarbeitung mithilfe des Tutorials von code.org wieder einmal auf Dauer etwas mühselig war, aber ohne kommen wir eben nicht aus. 
Wir sind sehr zufrieden mit unserem Ergebnis, vor allem mit unserem funktionierenden Scoreboard, welches uns die meisten Nerven gekostet hat.
