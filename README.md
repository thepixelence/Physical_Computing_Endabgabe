# Physical Computing 

Abgabe zum Kurs Physical Computing SoSE 2021

Repository zur ersten Aufgabe im Kurs Physical Computing.

Tom Schmitt | Sommersemester 21 | Intermedia Design

# About
Ich wählte den Kurs Physical Computing vor allem um eine erste Einführung ins Thema zu bekommen. Arduino und der umgang mit Arduinos o.ä. Mikrocontrollern war für mich neu. Mein Ziel war es vor allem zu sehen wie schnell ich einen Einstieg und erste Erfolge im bereich Physical Computing erzielen kann. Mit meinem Projekt wollte ich diese ersten Erfahrungen in einem umsetzbaren Rahmen erfüllen. Mein Ziel war es eine erste Human-Interface interaktion zu erstellen, um die möglichkeiten des Arduino Mikrocontrollers kennenzulernen. 

Durch den eher Programmierlastigen teil meines Projekts konnte ich mich weiter in den Software-Anteil von Physical Computing einarbeiten. Es war sehr motivierend schnelle Ergebnisse zu sehen, auch ohne vorheriges Wissen über Elektronik oder Programmierung in C/C++. 

Ich denke ich habe mein Ziel insofern erreicht, als das ich nun eine ungefähre Vorstellung davon habe, was in diesem Bereich für mich möglich ist. Mit der Fertigstellung meines Projekts habe ich einen Ausgangspunkt an dem ich mich weiter in die Welt der Mikrocontroller einarbeiten kann. 


https://user-images.githubusercontent.com/35604723/127353151-1fbb592c-2558-47f3-a91e-4cb8d00b1c2c.mp4

# Schritt 1 

## Entstehungsprozess:

* 1 - Projektsuche 
* 2 - Teile bestellen
* 3 - Umsetzung in TinkerCAD
* 4 - Umsetzung auf dem Breadboard

### Folgende Komponenten wurden benötigt:

* 1x Arduino Uno
* 1x LCD Panel 16x2
* 1x Breadboard
* 1x Widerstand 220 ohm
* 1x Push-button switch
* 8x Verbindungskabel

## Software 

### Folgende Libraries und Software wurden benutzt:

* PlattformIO
* Grove_LCD_RGB_Backlight-master
* LiquidCrystal 

# Code

Da der zu verwendende Code in meinem Tutorial sehr ausführlich beschrieben wurde, hatte ich die Hoffnung sehr schnell Ergebnisse zu sehen. 
Mein verwendetes Display war nur leider nicht dasselbe, dass im Tutorial benutzt wurde, weshalb ich den Code an Stellen anpassen musste.

Folgende Anpassungen musste ich vornehmen:

* #include <LiquidCrystal.h> -> Library für das LCD-Display 
* #include <Wire.h>
* #include <SPI.h> 
* #include "rgb_lcd.h> -> Library für das LCD-Display 
* #include <Arduino.h>

* rgb_lcd lcd; -> Initialisierung des LCD Display
* const int colorR = 120; -> Anpassung der Farbe des Displays
* const int colorG = 70; -> Anpassung der Farbe des Displays
* const int colorB = 70; -> Anpassung der Farbe des Displays
* lcd.begin(16, 2); -> Anpassung der Pixelangabe meines Displays
* lcd.setRGB(colorR, colorG, colorB); 
* initializeGraphics();  

## Schaltplan

<img width="959" alt="Bildschirmfoto 2021-07-28 um 11 44 35" src="https://user-images.githubusercontent.com/35604723/127351544-057f8e14-4711-41e4-888a-a2f53ee6b4ea.png">

![IMG_4350](https://user-images.githubusercontent.com/35604723/127351855-998cec22-c427-4ece-80cd-aefbfef26726.png)


# Verwendete Tutorials

* https://create.arduino.cc/projecthub/muhamd-magdy/arduino-game-by-lcd-9a3bc2?ref=similar&ref_id=169084&offset=0

# First steps:
[Download Code](https://github.com//thepixelence/physical_computing/archive/refs/heads/main.zip)


* 1 - PlattformIO in Visual Studio Code installieren
* 2 - Neues Projekt starten und Microcontroller auswählen (hier Arduino)
* 3 - FastLED Library installieren
* 4 - Daten aus dem download ZIP in die main.cpp Datei kopieren
* 5 - Dateien auf Arduino laden

# Was zu beachten ist:

* Alle Dateien im Repository müssen Lokal gespeichert sein. Die Dateistruktur darf außerdem nicht verändert werden.
* Um den Code zu bearbeiten muss ein Editor wie z.B. Visual Studio Code verwendet werden. ( https://code.visualstudio.com/ )
* Um Code auf das Arduino hochzuladen, wird ein Plugin namens PlattformIO benötigt. Dieses kann über Visual Studio Code Installiert werden.
* Um Code zu verändern, öffnen sie die main.cpp Datei im SRC ordner.
* Die anderen Dateien sollten wenn möglich unverändert bleiben.

# Nächste Schritte 

* Gehäuse bauen (Ich würde gerne ein Gehäuse bauen in dem Ich den Arduiono und die Kabel verstecken kann. Wenn man dann den Arduino mit einer Batterie verbindet könnte man somit einen "Mini-GameBoy" bauen.)

<img width="2560" alt="Bildschirmfoto 2021-07-29 um 18 49 47" src="https://user-images.githubusercontent.com/35604723/127532639-54793a26-45e8-4d90-ac0f-dab1961f1159.png">

Dieses Modell müsste dann noch im 3D Druck Verfahren gefertigt werden und der Mikrocontroller mit einer Batterie verlötet werden. 

* Softwareseitig könnte man das Spiel um ein Menü oder andere Hindernisse erweitern. Eine Highscore Funktion wäre auch eine Interessante Idee.


