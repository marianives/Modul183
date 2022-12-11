# Lern-Bericht
Ich habe diesen Auftrag alleine gemacht.

## Einleitung
In diesem Bericht geht es um die SQL-Injections, welche bei einer unsicherer WebApp gemacht werden können, und wie man diese Sicherheitslücke beheben kann. 

## Was habe ich gelernt?

Ich habe gelernt, wie man sich gegen SQL-Injections in einer WebApp sichern kann.

## Beschreibung

![image](https://user-images.githubusercontent.com/100756109/206928815-fff74214-5a43-493d-b181-e765f5e9c7d0.png)

In diesem Code Abschnitt geht es um das insert der News. Zuerst wird ein String mit dem SQL-Statement festgesetzt, in welchem die Values jedoch noch nicht definiert sind "(?)". Als nächstes wird der PreparedStatement deklariert, welcher gegen SQL-Injections schützt. Mit diesem werden dann die fehlenden Angaben deklariert (stmt.set...). Am Schluss wird mit stmt.excecuteUpdate dieser SQL Statement abgeschickt und schon ist man gegen Injection geschützt. Mit catch wird noch im Fall eines Fehlers es gefangen und geloggt.


![image](https://user-images.githubusercontent.com/100756109/206929445-0fae21ff-07a5-416a-ae07-56111d597e72.png)


## Verifikation

Man kann den klaren Code sehen, welcher die Gefahr auf SQL-Injection aufheben und ist funktionsfähig, da eine News mit dem Injection-Inhalt kreiert wird und nicht den SQL-Statement annimmt.

# Reflektion zum Arbeitsprozess

👍 Ich konnte gut mit dieser Problemstellung und mit den Hilfestellungen der Aufgabe den Auftrag lösen.

👎 Ich hatte Probleme mit NetBeans wegen Fehlermeldungen, welche ich übersehen habe.

**VBV**: ✍️ Fehlerbeschreibung besser lesen / analysieren.
