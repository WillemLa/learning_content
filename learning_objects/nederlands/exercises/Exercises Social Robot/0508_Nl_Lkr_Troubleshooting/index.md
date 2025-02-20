---
hruid: sr_TroubleshootingSimulator
version: 3
language: nl
title: "Troubleshooting"
description: "Troubleshooting"
keywords: ["Sociale robot"]
educational_goals: [
    {source: Source, id: id}, 
    {source: Source2, id: id2}
]
copyright: dwengo
licence: dwengo
content_type: text/markdown
available: true
target_ages: [12, 13, 14]
difficulty: 3
return_value: {
    callback_url: callback-url-example,
    callback_schema: {
        att: test,
        att2: test2
    }
}
content_location: example-location
estimated_time: 5
skos_concepts: [
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-computers-en-systemen'
]
teacher_exclusive: true
---

# Programmeren van de robot
## Code testen

Telkens je aanpassingen doet aan een programma of als je een nieuw programma hebt geschreven, voer je het uit in de simulator. Zo kijk je wat het resultaat zal zijn op de dwenguino, en test je uit of het programma goed werkt. De simulatie kan bediend worden met de knoppen uit het simulatormenu. Zo kan je de simulator starten met ![](embed/Playknop.png "Play") en stoppen met ![](embed/Stopknop.png "Stop").

![](@youtube/https://www.youtube.com/embed/hmr5smg7l8Y "voorbeeld")

Het ‘sociale robot’-scenario bevat geen dwenguino in het simulatieveld. Daar zal je enkel code kunnen uitvoeren op de robotonderdelen die je zelf aan het simulatieveld hebt toegevoegd.


## Debuggen

Doet je code niet wat je verwacht, dan kan je de code debuggen met ![](embed/Stapknop.png "Stap"): je spoort fouten op door de code blok per blok uit te voeren. Telkens je op de debug-knop klikt, wordt het volgende blok uit je programma uitgevoerd en gesimuleerd. Je kan dan op je eigen tempo ontdekken waar er een foute blok in het programma zit.  
Wil je niet vanaf het eerste blok debuggen? Dan kan je de simulatie eerst starten en pauzeren met ![](embed/Pauzeknop.png "Pauze") waar je wil starten met debuggen.

![](@youtube/https://www.youtube.com/embed/PhblfDjUXPQ&list=PLHRY06NDfDXlBpLm5J3BK26Ul6GxGykDu&index=2 "Lijst simulatortutorials")


## Code uploaden naar de dwenguino

In het hoofdmenu (en dus niet in het simulatormenu) kan je de knop ![](embed/Upload.png "Upload") vinden om je programma te uploaden naar de fysieke robot. Zorg ervoor dat de dwenguino verbonden is met de computer m.b.v. de bijgeleverde USB-kabel.


Tijdens het uploaden verandert het robot-icoontje ![](embed/RobotIcoon.png "Robot icoon") in een draaiend tandwieltje ![](embed/Settings.png "Bezig"). Op het lcd-scherm van de dwenguino verschijnt een boodschap om aan te geven dat de microcontroller in gebruik is. Wanneer het robot-icoontje terug verschijnt, is het programma succesvol geüpload naar de dwenguino

Krijg je een pop-up te zien met de boodschap *'Sorry, het is niet gelukt om de code te uploaden naar het bord'*? Dan is het uploaden mislukt. Hiervoor kunnen er verschillende redenen zijn:


1. **Het bord is niet of fout aangesloten**

Volg deze stappen om het dwenguino-bord te herstarten:

* Maak de USB-kabel los;

* Verbind de computer en het dwenguino-bord met de USB-kabel;

* Druk tegelijkertijd de RESET-knop en de ZUID-knop in van het dwenguino-bord;

* Los dan eerstde RESET-knop;

* Los daarna de ZUID-knop;

* Upload het programma opnieuw via de ![](embed/Upload.png "Upload") in het hoofdmenu.


2. **Er zit een fout in je programma**

Controleer nogmaals of je programma correct is. Je kan ook kijken naar foutmeldingen in het zwarte consolevenster in de pop-up om uit te zoeken water mis is. Lukt her niet om de fout op te lossen? Download je Blockly-programma en laad het opnieuw in. Probeer het dan nogmaals te uploaden naar de dwenguino.


## FAQs

**Het lcd-scherm toont geen tekst of is bijna zwart**

* Pas het contrast van het lcd-scherm aan via het gele schroefje op de dwenguino (zie **Elektronica**)

**De sonar-sensor werkt niet**

* Het gebeurt af en toe dat een sensor kapot is. Probeer na te gaan of dit het geval is door de aansluitingen van de sonar-sensor na te kijken en de gemeten waarde van de sensor weer te geven op het lcd-scherm.
* Is de bedrading correct aangesloten? Zit er geen fout in de bedrading zelf (bv. een verwisseling van de dragen)?