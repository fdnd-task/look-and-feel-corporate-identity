# Look and Feel - Corporate Identity

## Code/Design Review

Deze week heb je geleerd hoe je een gezamenlijke styleguide toepast op jouw eigen leertaak. Daarnaast hebben jullie meer geleerd over typografie en formulieren. 

<!-- Als er 40 studenten zijn, groepen van 3 maken. 14 groepen maken we dan. -->

### Aanpak

Jullie gaan elkaars werk één voor één reviewen binnen de groep. Gebruik één laptop om de code te bekijken en een andere laptop om issues in te schieten. De onderstaande code- en design review voer je uit voor elk lid van jullie groep. 

#### Code review

Een doel van deze sprint is om in de HTML van de leertaak de gedeelde styleguide te gebruiken, dus daar gaat deze code review over. Zorg dat de laatste versie van de gedeelde styleguide live staat op GitHub en beschikbaar is via GitHub Pages.

We gaan kijken of zowel de gedeelde stylesheet, als je eigen stylesheet, gebruikt wordt in de leertaak. Controleer dit gezamenlijk, en schiet issues in waar nodig.

-   Stap 1: Controleer of de gedeelde stylesheet correct is gelinkt in de repository, via een `<link>` tag naar de stylesheet op GitHub Pages van de gedeelde repository. Zo niet, maak dan een issue aan op de leertaak, en laat de ander dit meteen oplossen (en dat issue sluiten).
-   Stap 2: Controleer of de styles uit de gedeelde stylesheet conflicteren met die uit de leertaak, en zoek uit hoe dit komt. Waarschijnlijk door de _specificity_ van de selectors: het kan goed zijn dat er te algemene selectors in de gedeelde stylesheet staan. Maak in dat geval issues aan in de _gedeelde repository_. Voorbeeld: “De font styling op de `body` is te algemeen, en conflicteert met de styling van mijn eigen `header`. De selector voor font styling in onze gedeelde stylesheet moet minder algemeen.” Deze issues kunnen komende week opgepakt worden.
-   Stap 3: Doe een code review op de HTML uit de leertaak, en controleer of er inderdaad ook gebruik wordt gemaakt van `classes` uit de gedeelde stylesheet. Zo niet, maak dan een issue aan op de leertaak. Voorbeeld: “Je gebruikt voor het stylen van je alinea's nog geen CSS uit de gedeelde stylesheet; gebruik hiervoor `class="font-xl"`.”
-   Stap 4: Bekijk het individueel gemaakte CSS-bestand uit de leertaak. Loop alle regels in de CSS door, en kijk of er styling in staat die ook al in de gedeelde stylesheet staat. Schiet issues in op de leertaak als dit het geval is. Voorbeeld: “Je eigen stylesheet gebruikt nog font styles, die ook al in de gedeelde stylesheet staan. Deze kun je weghalen, want je maakt gebruik van `class="font-xl"`.”

#### Design review

Ga met elkaar na of de styleguide navolgbaar toegepast is in de leertaak. Pak hiervoor de live link van de leertaak en de live link van de styleguide repository erbij. Schiet issues in waar nodig:

-   Komen de kleuren, typografie en fonts overeen met die in de styleguide? Zijn er extra kleuren, fonts of andere font-sizes toegevoegd? Moeten die opgenomen worden in de styleguide?
-   Zijn de kleuren op de juiste manier toegepast? Hoe hebben jullie dat gecontroleerd? Is dit terug te vinden in de styleguide?
-   Zijn de componenten vormgegeven zoals aangegeven in de styleguide? Kijk vooral ook naar de details, denk aan afgeronde hoeken, schaduwen en spacing. Zijn hier afspraken over gemaakt?
-   Is er consistentie te zien in de uitgewerkte versie?
-   Zijn alle elementen die op de website staan ook terug te vinden in de styleguide? Zo nee, waar zou dit onder kunnen worden opgenomen?