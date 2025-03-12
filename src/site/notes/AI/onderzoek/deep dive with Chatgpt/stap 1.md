---
{"dg-publish":true,"permalink":"/ai/onderzoek/deep-dive-with-chatgpt/stap-1/","created":"2025-02-15T22:21:13.516+01:00","updated":"2025-03-12T14:44:30.536+01:00"}
---


## downloaden en voorbewerken van het "internet"


Een bedrijf genaamd HuggingFace heeft een dataset gemaakt / verzameld genaamd FineWeb

Al de grote LLM's leveranciers zoals Anthropic(Claude), Google(Gemini) en OpenAI(ChatGPT) hebben een gelijkaardige interne dataset zoals deze FineWeb Dataset.

Wat men hiermee probeert te bereiken is om zoveel mogelijk tekst van zoveel mogelijk
 verschillende openbare bronnen te verzamelen.
We willen een enorme hoeveelheid documenten van hoge kwaliteit en we willen een enorme diversiteit van documenten omdat we een grote hoeveelheid kennis willen in deze modellen.

## URL filtering
### ruwe data vinden
Een veel gestelde vraag is dan natuurlijk waar halen ze al die data vandaan?
Er zijn algemeen gezien 2 opties:

-Je crawlt het zelf , zoals bedrijven als OpenAI en Anthropic doen.
-Je gebruikt een openbare opslagplaats van gecrawlde webpagina's zoals bv CommonCrawl

Om Fineweb te bouwen heeft men CommonCrawl als een startpunt genomen , en als voorbeeld nemen we de laatste CC crawl(Januari 2025) bevat 3 miljard webpagina's (goed voor een 460TiB aan ongecomprimeerde inhoud)

#### zwarte lijsten
Men maakt ook een lijst van welke soort websites niet mogen worden opgenomen in een dataset , bv racistische websites , malware of virus websites ,...
## tekst extractie

Dan gaat men proberen om enkel de tekst van een webpagina te crawlen , men heeft namelijk geen nood aan bv navigatie of afbeeldingen dus deze dingen laat men achterwege

## taalfiltering

Men beslist ook welke kwaliteit van taal men wilt van bv Engels . Hier beslist men ook welke talen ze allemaal willen in de dataset.

Als men ervoor kiest om bv Spaans uit de dataset te laten , zal het model niet echt sterk kunnen handelen in het Spaans.

FineWeb heeft een focus gelegd op het Engels , dus dus zal het AI model ook het beste werkte in het Engels.


## Andere stappen

na taalfiltering gebeuren er nog een heleboel stappen namelijk vooral filteren , op specifieke dingen.

Nog een belangrijke stap , de laatste dan van stap 1 is het verwijderen van persoonlijke gegevens zoals adressen rijksregisternummers enzovoort.
Deze gegevens worden allemaal uit de dataset verwijderd.