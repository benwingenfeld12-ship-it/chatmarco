Chat Macro (Fabric, clientseitig)

1. Projekt mit dem Fabric-Template-Generator (fabricmc.net/develop/template) erzeugen,
   "Split client and common sources" aktivieren. Das liefert gradlew + gradle/wrapper.
2. Die Ordner src/ aus diesem ZIP ins Template kopieren (vorhandene Dateien ersetzen).
   Alternativ: gradlew + gradle/ aus dem Template in diesen Ordner kopieren.
3. In gradle.properties die Versionen pruefen (stehen auf 1.21.11).
4. ./gradlew build  ->  fertige .jar in build/libs/ (ohne -sources).
5. Im Spiel: Optionen > Steuerung > Chat Macro. Standard: H = "Hallo zusammen!", G = "gg".

Texte aendern: in ChatMacroClient.java die Strings bei send(...).
Ein Text mit "/" am Anfang wird als Befehl gesendet.
