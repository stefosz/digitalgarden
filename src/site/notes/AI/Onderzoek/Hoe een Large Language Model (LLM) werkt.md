---
{"dg-publish":true,"permalink":"/ai/onderzoek/hoe-een-large-language-model-llm-werkt/","created":"2025-03-14T22:04:00.760+01:00","updated":"2025-03-14T22:08:47.118+01:00"}
---


# Intro Van neurale netwerken tot maatschappelijke impact


In de afgelopen jaren hebben Large Language Models (LLM's) zoals GPT-4 een revolutie teweeggebracht in artificiële intelligentie. Deze modellen, gebouwd op neurale netwerken en geavanceerde architecturen zoals de transformer, combineren grootschalige dataverwerking met innovatieve mechanismen zoals self-attention om menselijke taal te begrijpen en te genereren. Dit artikel biedt een diepgaande analyse van hun werking, van fundamentele principes tot maatschappelijke gevolgen, ondersteund door recente inzichten uit onderzoek en praktijktoepassingen

---

# Neurale netwerken ,Het brein achter AI

Een Large Language Model is een specifieke toepassing van **kunstmatige neurale netwerken**, geïnspireerd op de structuur van het menselijk brein. Net zoals neuronen in de hersenen via synapsen communiceren, bestaan neurale netwerken uit lagen van kunstmatige "neuronen" die informatie verwerken via gewichten en biases. Een eenvoudig neuraal netwerk bevat:

- Een **inputlaag** die ruwe data ontvangt (bijvoorbeeld tekst).
    
- Verborgen **middelste lagen** die patronen extraheren.
    
- Een **outputlaag** die het resultaat produceert (zoals een voorspeld woord).
    

Bij LLM's werken deze netwerken op een **diepgaande schaal**, met honderden miljoenen tot biljoenen parameters. Een analogie: stel je een vertaler voor die eerst individuele letters leert herkennen, dan woorden, vervolgens zinsstructuren, en uiteindelijk hele verhalen kan interpreteren. Elk "neuron" in het netwerk draagt bij aan dit cumulatieve leerproces door statistische relaties tussen taalonderdelen te identificeren

---

# De transformer-architectuur , Een paradigmaverschuiving

De doorbraak van LLM's is ondenkbaar zonder de **transformer-architectuur**, geïntroduceerd in 2017. Traditionele modellen zoals RNN's (Recurrent Neural Networks) verwerkten tekst sequentieel, wat traag en inefficiënt was voor lange zinnen. Transformers omzeilen dit via **parallelle verwerking** en een innovatief **self-attention-mechanisme**.

---

# Zelfaandacht, De kunst van contextueel begrip

Stel je een literaire kring voor waar elke deelnemer (woord) luistert naar anderen om de betekenis van een zin te bepalen. Het self-attention-mechanisme werkt vergelijkbaar: het berekent voor elk woord (token) hoe sterk het gerelateerd is aan andere woorden in de zin. Wiskundig gezien gebeurt dit via **dot-productberekeningen** tussen **query-**, **key-**, en **value-vectoren**, die het model leert tijdens training.



---

# Positionele codering, Orde in de chaos

Omdat transformers geen inherent besef van woordvolgorde hebben, voegen ze **positionele coderingen** toe aan de invoer-embeddings. Dit is vergelijkbaar met het nummeren van woorden in een zin om hun relatieve positie te behouden.

---

# Tokenization en embeddings, Van tekst naar wiskunde



---

## Tokenization, Het opbreken van taal

Voordat een LLM tekst kan verwerken, splitst het deze in **tokens**—kleine eenheden zoals woorden, subwoorden of karakters. Bijvoorbeeld: "voorbeeldzin" wordt mogelijk opgesplitst in "voor", "beeld", "zin". Dit proces optimaliseert de balans tussen semantische betekenis en rekenefficiëntie.

---

## Embeddings, Taal in vectorruimte

Elke token wordt omgezet in een **embedding**, een dichtbevolkte vector van getallen (bijvoorbeeld 768 dimensies) die semantische en syntactische relaties vastlegt. Een analogie: net zoals een GPS-coördinaat een locatie in 3D-ruimte beschrijft, plaatst een embedding een woord in een multidimensionale "betekenissenruimte".

---

# Training, Het leerproces van een LLM



---

## Pre-training op gigantische datasets

LLM's leren eerst algemene taalpatronen via **zelfsupervisie** op datasets zoals The Pile (886GB tekst). Een veelgebruikte taak is **masked language modeling**, waarbij het model ontbrekende woorden in een zin voorspelt. Bijvoorbeeld:  
"De kat zat op de (MASK)" → "mat".


---

# Fine-tuning, Specialisatie voor specifieke taken

Na pre-training wordt het model verfijnd op smallere datasets voor taken zoals vertaling of vraagbeantwoording. Dit proces vereist slechts 1-10% van de oorspronkelijke rekenkracht maar verbetert de prestatie aanzienlijk.

---

# Voor- en nadelen van LLM's

## Voordelen

- **Schaalbaarheid**: Modellen zoals GPT-4 kunnen duizenden taken aan dankzij brede training.
    
- **Efficiëntie**: Automatisering van tekstgeneratie, vertaling en code schrijven.
    
- **Innovatie**: Toepassingen in klimaatmodellering en medisch onderzoek.
    

## Uitdagingen

- **Energieverbruik**: Training van GPT-3 verbruikte ~1.287 MWh, vergelijkbaar met het jaarlijkse verbruik van 120 huishoudens.
    
- **Bias en ethiek**: Modellen kunnen vooroordelen in trainingsdata reproduceren, zoals genderstereotypen.
    
- **Black box-probleem**: Zelfs ontwikkelaars begrijpen niet volledig hoe LLM's bepaalde beslissingen nemen.

---

# Maatschappelijke impact en toekomstperspectief

LLM's hebben al sectoren zoals gezondheidszorg, onderwijs en softwareontwikkeling getransformeerd. Zo helpen ze artsen bij het analyseren van medische literatuur en studenten bij het leren van talen) Echter, hun groeiende invloed roept vragen op over privacy, arbeidsmarktverstoring en ecologische voetafdruk. Innovaties zoals **groene AI** (energiezuinige algoritmen) en **ethische richtlijnen** zijn cruciaal om deze uitdagingen het hoofd te bieden.

De toekomst van LLM's ligt in **multimodaliteit** (combinatie van tekst, beeld en geluid) en **persoonlijke aanpassing**, waarbij modellen zich in realtime aanpassen aan individuele gebruikers. Zoals een kind leert door interactie, zullen toekomstige LLM's continu evolueren via interactie met de echte wereld.

---

# bronnen

Hier vindt u enkele bronnen die ik gebruikt heb voor dit onderzoek.

Wu, L., et al. (2023). The Impact of Large Language Models on Scientific Discovery: a Preliminary Study using GPT-4. arXiv. [https://arxiv.org/abs/2311.07361](https://arxiv.org/abs/2311.07361)

Raschka, S. (2023, 9 februari). Understanding and Coding the Self-Attention Mechanism of Large Language Models from Scratch. [https://sebastianraschka.com/blog/2023/self-attention-from-scratch.html](https://sebastianraschka.com/blog/2023/self-attention-from-scratch.html)

Jain, A. (2024, 30 mei). Understanding the Core Components of LLMs: Vectors, Tokens, and Embeddings. LinkedIn. [https://www.linkedin.com/pulse/understanding-core-components-llms-vectors-tokens-embeddings-jain-dlv6e](https://www.linkedin.com/pulse/understanding-core-components-llms-vectors-tokens-embeddings-jain-dlv6e)

DataHacker. (2024, 26 november). Understanding Large Language Models (LLMs) like LLaMa by Meta - Part 1. [https://datahacker.rs/understanding-large-language-models-llms-like-llama-by-meta-part-1/](https://datahacker.rs/understanding-large-language-models-llms-like-llama-by-meta-part-1/)

AiThority. (2024, 19 juni). Benefits And Limitations Of LLM. [https://aithority.com/machine-learning/benefits-and-limitations-of-llm/](https://aithority.com/machine-learning/benefits-and-limitations-of-llm/)

Nusocia. (2023, 3 november). Leveraging Large Language Models for Social Impact. LinkedIn. [https://www.linkedin.com/pulse/leveraging-large-language-models-social-impact-nusocia-b4pzc](https://www.linkedin.com/pulse/leveraging-large-language-models-social-impact-nusocia-b4pzc)

OpenAI. (2023, 14 maart). GPT-4. [https://openai.com/index/gpt-4-research/](https://openai.com/index/gpt-4-research/)

