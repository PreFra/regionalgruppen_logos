# S4F Regionalgruppen-Logos [![Build Status](https://travis-ci.com/s4f-dortmund/regionalgruppen_logos.svg?branch=master)](https://travis-ci.com/s4f-dortmund/regionalgruppen_logos)

Die aktuellen Logos gibt es als Download im [Release Bereich](https://github.com/s4f-dortmund/regionalgruppen_logos/releases).

## Neue Regionalgruppe hinzufügen

> Es ist nicht nötig Logos lokal auf dem eigenen Rechner zu erstellen

Um eine neue Regionalgruppe hinzuzufügen ist es am einfachsten,
über das GitHub Webinterface die Datei [regionalgruppen.txt](regionalgruppen.txt) zu bearbeiten.
Ansonsten gerne per Mail oder [Issue](https://github.com/s4f-dortmund/regionalgruppen_logos/issues/new) eine neue Gruppe anfragen.

Dafür einfach die Datei anklicken und dort auf das Bleistift Icon klicken.
Dann an der alphabetisch korrekten Stelle eine neue Zeile mit dem Text für die Regionalgruppe einfügen und danach
den Button für einen neuen Pull Request drücken.

## Hintergrund

Das Logo wird als LaTeX-Dokument definiert und mit inkscape in svg und png umgewandelt.
Jedes Logo wird in allen drei Formaten zur Verfügung gestellt.
Ein python script erzeugt für jede Regionalgruppe die entsprechende LaTeX Datei und ruft LaTeX und inskscape um die
pdf, png und svg Logos zu erstellen.
Am Ende wird alles in eine Zip datei pro Regionalgruppe und eine für alles zusammen gepackt.

Für neue releases werden die Logos automatisch mit Github Actions gebaut.
Um ein neues Logo hinzuzufügen muss nur eine entsprechende Zeile in die Datei regionalgruppen.txt eingefügt werden.

Benötigt werden:

* python ≥ 3.6
* inkscape <https://inkscape.org/de/>
* TeXLive <https://www.tug.org/texlive/>
* Montserrat Font <https://www.fontsquirrel.com/fonts/montserrat>
