# DayZ-Standalone-Server
DayZ Standalone Serverfiles - Ideal für Coop (enthält nützliche Funktionen)

#### :: Informationen zu den Servereinstellungen
⋅⋅* Bis zu 10 spieler können beitreten (kann geändert werden in der ServerDZ.cfg)  
⋅⋅* Schwierigkeit: Einfach (Es ist immer Tag, kein Tag/Nacht Zyklus, meistens Warm, man findet häufiger Essen/Trinken)  
⋅⋅* Schraubenzieher als Startgegenstand (Praktisch zum Dosenöffnen).  
⋅⋅* Es wurden hilfreiche Befehle hinzugefügt.  Ich habe hierzu die init.c von https://github.com/Heinrich19800 gebugfixt und aufs wesentliche gekürzt.  
Bekannte Fehler: Aktuell kann die Befehle jeder auf dem Server ausführen (wird später noch gefixt).  

#### :: Admin Befehle
```!Regen         - Es wird aufhören zu Regnen  
!Nebel         - Der Nebel entfernt sich  
!Gewitter      - Das Gewitter zieht vorüber  
!Tag           - Es wird Tag (12 Uhr)  
!Nacht         - Es wird Nacht (0 Uhr)  
!goto Name     - Du wirst zu dem Spieler 'Name' Teleportiert. Name duch Spielernamen ersetzen. Standard Spielername ist "Survivor".  
!here Name     - Der Spieler 'Name' wird zu dir Teleportiert. Name duch Spielernamen ersetzen. Standard Spielername ist "Survivor".  
!tppos X Y     - Teleportiert dich an die eingegebene Koordinate. Die Webseite https://dayz.ginfo.gg ist hier sehr hilfreich.  
!pos           - Gibt deinen aktuellen Koordinaten aus. Diese kann man dann auf der Webseite eingeben.
!hilfe         - Gibt eine Übersicht über alle Befehle aus  
```  



#### :: Installation
Die Dateien herunterladen und im DayZ Server Ordner (\Steam\steamapps\common\DayZServer) einfügen.  
Bestehende Dateien dabei überschreiben.  
 
 
#### :: Start.bat - Startet den Server
Startet die 64Bit version des DayZ Standalone Servers, lädt die Konfigurationsdateien und erstellt einen Ordner für Logfiles unter "C:\Users\\%USERNAME%\Documents\DayZServer_SERVERNAME".
 
 
 
#### :: serverDZ.cfg - Die Konfigurationsdatei für den Server
Bitte in der ersten Zeile "EXAMPLE NAME" durch den gewünschen Servernamen ersetzen andernfalls startet der Server nicht.  
WICHTIG: Bitte unbedingt unter passwordAdmin = ""; ein Admin Kennwort setzen!  
Hier kann man den Tag/Nacht zyklus oder die Startzeit auf seine eigenen wünsche anpassen. Beschreibung ist in der Datei enthalten.  
 
 
 
#### :: init.c - Beinhaltet die Wetterkontrolle und die hilfreichen Befehle
Falls man englische Sprache nutzen möchte löscht man die init.c und ändert die "init.c_en" in "init.c".  
Keine änderungen in dieser Datei vornehmen! Andernfalls führt das zu einem Absturz, Datenverlust oder einem instabilem Server!  
 
 
 
#### :: types.xml - Beinhaltet die verteilungsrate von Essen, Waffen, etc.
Es wurde nur die häufigkeit von Nahrung erhöht da man sonst permanent den Hungertod stirbt.  
 
 
 
#### :: messages.xml - Nachrichten des Servers
Beinhaltet eine Willkommensnachricht für jeden Spieler der Beitritt. Bitte hier den Text anpassen/ändern.  
 
 
 
#### :: globals.xml - Globale Servereinstellungen
Hier wurde die 15 Sekündige Login Wartezeit entfernt. Spart Zeit und ist im Coop sonst besonders nervig.  
