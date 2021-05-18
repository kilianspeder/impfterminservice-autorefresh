# impfterminservice-autorefresh
 
*English version below*

### Allgemeine Hinweise

- Dieses Skript wurde entwickelt für die Plattform *imptferminservice.de* zur automatischen Suche nach Impfterminen 
- Dieses Skript wurde getestet in Firefox und Google Chrome, müsste aber prinzipiell in allen modernen Browsern funktionieren
- Das Skript funktioniert erst, wenn man einen Vermittlungscode hat. Es sucht nicht nach den Codes

### Benutzung

1. JavaScript-Konsole mit <kbd>Cmd/Strg</kbd> + <kbd>Alt</kbd> + <kbd>C</kbd> des Browsers im Tab mit *impftermineservice.de* öffnen. \
(In Safari muss dafür in den Einstellungen unter *Erweitert* der Punkt *Menü "Entwickler" in der Menüleiste anzeigen* aktiviert werden)
2. Den Inhalt von [imptermineservice-autorefresh.js](./impfterminservice-autorefresh.js) in die Eingabe der Konsole kopieren und mit <kbd>Enter</kbd> ausführen
3. Einmal auf die Eingabefläche "*Termine suchen*" klicken.
4. Das Popup öffnet und schließt sich jetzt automatisch, bis ein Termin gefunden wurde. Jede Öffnung stößt eine erneute Suche an
5. Sobald ein Termin gefunden wurde, ertönt ein Ton und der Hintergrund der Webseite wird rot.
6. Um den Hintergrund wieder weiß zu machen, muss man die ```resetBackground()``` in die Konsole eingeben und ausführen.
7. Das Skript lässt sich mit dem Befehl ```toggleOnOff()*``` über die Konsole ein- und ausschalten.


### Fortgeschrittenes

Falls man die Wartezeit bevor das Popup nach Terminen geprüft und wieder geschlossen wird, ändern will, muss man die 
Variable ```timeToWaitForAPI``` über die Konsole ändern. Der Wert wird in Millisekunden angegeben.

---

## English Version:

### General information
- This script was developed to automate the search for vaccinations appointments on *impfterminservice.de*
- This script was tested in Google Chrome and Firefox but should also work in every other modern browser
- This script only works after already receiving a so called "Vermittlungscode" (referral code). 
  It does not automatically search for these codes.
  
### Usage
1. Open the JavaSript-console on the browser tab with *impfterminservice.de* with <kbd>Cmd/Strg</kbd> + <kbd>Alt</kbd> + <kbd>C</kbd>\
   (In Safari you have to activate the developer options in the settings tab *Advanced*)
2. Copy the contents of [imptermineservice-autorefresh.js](./impfterminservice-autorefresh.js) into the console and execute it with <kbd>Enter</kbd>
3. Click on "*Termine suchen*" once to start the script
4. The popup will now automatically open and close until an appointment is found. Each opening will start a search for appointments.
5. Once an appointment is found, a sound will be played and the background of the website will turn red.
6. To turn the background white again execute ```resetBackground()``` in the console.
7. Using ```toggleOnOff()``` you can turn the script on and off

### Advanced
If you want to change the time before the Popup will be checked for appointments and closed again, you have to change 
the variable ```timeToWaitForAPI``` via the console. The value is given in milliseconds.
