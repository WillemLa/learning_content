---
hruid: aiz_voorbeeld
version: 3
language: nl
title: "Voorbeeldnotebook"
description: "Voorbeeldnotebook"
keywords: [""]
educational_goals: [
    {source: Source, id: id}, 
    {source: Source2, id: id2}
]
copyright: dwengo
licence: dwengo
content_type: text/markdown
available: true
target_ages: [14, 15, 16, 17, 18]
difficulty: 3
return_value: {
    callback_url: callback-url-example,
    callback_schema: {
        att: test,
        att2: test2
    }
}
content_location: example-location
estimated_time: 1
skos_concepts: [
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-computers-en-systemen'
]
teacher_exclusive: false
---

# Voorbeeldnotebook
Je kan enkele lichaamsparameters in rekening brengen om te proberen te voorspellen of een patiënt risico loopt op een hartaanval. Van gekende
patiënten zijn bepaalde parameters terug te vinden in het patiëntendossier.
De volgende tabel toont zulke parameters voor zes patiënten waarvan  geweten is of ze al dan niet een hartaanval kregen (Shoemaker et al., 2001).
Aan de hand van deze (te beperkte) dataset wordt getoond hoe je het verdeel-en-heersalgoritme in de praktijk toepast om een beslissingsboom
aan te maken. Deze beslissingsboom kan dan gebruikt worden om voor nieuwe patiënten na te gaan of ze risico lopen op het krijgen van een hartaanval.

|**Patiëntnummer**|**Pijn in de borststreek**|**Man**|**Rookt**|**Voldoende lichaamsbeweging**|**Hartaanval**|
|---------------|------------------------|-----|-------|----------------------------|------------|
|1|ja|ja|nee|ja|ja|
|2|ja|ja|ja|nee|ja|
|3|nee|nee|ja|nee|ja|
|4|nee|ja|nee|ja|nee|
|5|ja|nee|ja|ja|ja|
|6|nee|ja|ja|ja|nee|

<figure>
    <figcaption align = "center"><b>Tabel: Parameters van belang voor risico op hartaanval</b></figcaption>
</figure>

Het algoritme om een beslissingsboom te construeren, kan ook geprogrammeerd worden in een computer. Om een computer dit algoritme te laten uitvoeren, moet je de verschillende stappen op een ondubbelzinnige manier in een computerprogramma gieten. Dat is reeds voor jou gedaan en bereikbaar via Python-modules.
Je zal deze gebruiken en je zal dus a.d.h.v. een regelgebaseerd AI-systeem automatisch een beslissingsboom laten genereren.

In de notebook vertrek je van dezelfde tabel met de parameters die worden gebruikt om te proberen voorspellen of een patiënt risico loopt op een
hartaanval. Om dit te implementeren in Python, zal je dus deze beperkte dataset in Python moeten ingeven. Dat gebeurt door een matrix in te voeren. Zo’n matrix is niet anders dan een tabel van getallen. 

Merk op dat de waarden van de variabelen in de tabel categorisch zijn en dat deze voor de computer omgezet zullen moeten worden naar numerieke of kwantitatieve
variabelen. In de notebook worden de waarden van de variabelen ingegeven als numerieke waarden. Voor ‘nee’ wordt een ‘0’ gebruikt en voor ‘ja’ een ‘1’.

[![](embed/Knop.png "Knop")](https://kiks.ilabt.imec.be/jupyterhub/?id=3010 "Voorbeeldnotebook")

Extra uitleg vind je in hoofdstuk 8 van de handleiding.
