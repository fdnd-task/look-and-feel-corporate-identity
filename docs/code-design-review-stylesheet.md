# Look and Feel - Corporate Identity

## Code/Design Review Stylesheet

Deze week heb je geleerd hoe je een styleguide maakt voor een opdrachtgever. Een huisstijl is de visuele identiteit van een organisatie. Hieronder vallen naam, beeldmerk, kleuren, typografie, vormentaal (stramienen/vlakken/curves/opmaak) en fotografiestijl. Jullie hebben de huisstijl van de opdrachtgever geanalyseerd, een interface inventory gemaakt en een styleguide samengesteld. Vervolgens hebben jullie dit omgezet in een gedeelde stylesheet. 

### Aanpak
Vandaag ga je aan de slag met een code-review op de repo 'Look and Feel - Styleguide' van 2 andere groepen. Vervolgens ga je met jouw groepje de ontvangen issues toewijzen (assignen) aan teamleden. Post de link van jullie Look and Feel Styleguide in de Teams channel 'Sprint 4' samen met jullie projectnaam. 

#### Code-review Look and Feel - Styelguide
1. Bekijk in het schema hieronder welke twee groepen jullie gaan reviewen. 

| Groep                         | Reviewt groepen                        | Ontvangt reviews van groepen                  |
|-------------------------------|----------------------------------------|-----------------------------------------------|
| **Drop & Heal**               | Tumi Mundo, Mediahuis                 | Mediahuis, Online Collection Qatar Museums  |
| **Tumi Mundo**                | Oncology Collaboration Platform, Bieb in Bloei | Drop&Heal, Bieb in Bloei      |
| **Oncology Collaboration Platform** | Red Pers Website, Online Collection Qatar Museums | Tumi Mundo            |
| **Red Pers Website**          | Mediahuis, DDA Vacature Site          | Online Collection Qatar Museums, Mediahuis, DDA   |
| **Mediahuis**                 | Drop & Heal, Bieb in Bloei            | Drop&Heal, Red Pers |
| **Bieb in Bloei**             | DDA Vacature Site, Tumi Mundo         | Tumi Mundo, Mediahuis, DDA       |
| **Online Collection Qatar Museums** | Drop & Heal, DDA Vacature Site     | Oncology Collaboration Platform    |
| **DDA Vacature Site**         | Bieb in Bloei, Red Pers Website       | Online Collection Qatar Museums, Red Pers Website, Bieb in Bloei |

_Herhaal onderstaande checklist voor twee groepen. Je voert deze code review uit met de gehele groep. Bepaal met elkaar wie de issues schrijft._

2. Pak samen met jullie mentor de repo erbij van de groep die je gaat reviewen. Lees met elkaar de README. 
   - **Feedback op README**: Controleer of de README voldoende informatie bevat om te begrijpen hoe de stylesheet werkt. Is het duidelijk hoe je de code kunt implementeren? Zou je zelfstandig hiermee kunnen werken? Schrijf je feedback in het “Feedback op README” issue.

3. **Code Review Checklist**: Doorloop de volgende vragen om de kwaliteit van de stylesheet te beoordelen. Schiet waar nodig een issue in.

   - **Indeling van de stylesheet**: Is de structuur van de stylesheet logisch? Zijn secties goed ingedeeld (bijv. kleuren, typografie, knoppen) zodat ze eenvoudig terug te vinden zijn?
   
   - **Consistente naamgeving**: Is de naamgeving consisitent? Kijk of er een consistente schrijfwijze is gekozen (zoals kebab-case voor CSS-variabelen of selectors, bijvoorbeeld `--font-size-large`).
   
   - **Naamgeving en begrijpelijkheid**: Is de naamgeving van variabelen en classes gemakkelijk te volgen? 

   - **Volledigheid van de stylesheet**: Bevat de stylesheet voldoende elementen en states voor een volledige implementatie? Let op states zoals hover, active en focus voor links en knoppen, en controleer of formulieren (inputvelden, foutmeldingen) ook zijn opgenomen.

   - **Custom properties op juiste element**: Worden de custom properties op de juiste plaats toegepast? Bijvoorbeeld, worden custom properties op de :root gedefinieerd? Is dat een bewuste keuze? Of zou het ook op de body kunnen?

   - **Herhaling van code**: Bekijk of er onnodige herhaling van code is. Als er vaak dezelfde stijlen worden herhaald, kijk dan of dit simpeler kan door variabelen of mixins te gebruiken.


---

#### Issues toewijzen
Klaar met de twee code reviews? Ga dan samen aan de slag met de issues die jullie hebben ontvangen.
1. Bekijk samen met jullie mentor de issues die jullie zelf hebben ontvangen. Vraag waar nodig toelichting.
2. Overleg met elkaar wie welke issue gaat oppakken. Assign vervolgens een issue aan het teamlid die deze taak gaat oppakken.
3. Klaar? Je kunt nu individueel de issues die jou zijn toegewezen gaan oplossen. Sluit de issues wanneer opgelost met een duidelijke toelichting wat je hebt gedaan en de bijbehorende commit.  

