# Look and Feel - Corporate Identity

## Stylesheet

Je hebt in Figma een styleguide gemaakt, nu ga je een gestructureerd CSS file maken met als doel dat jullie één stylesheet kunnen gebruiken in je individuele project voor veelvoorkomende CSS selectoren en properties.

## Opdrachten

- CSS strategie
- Custom properties
- CSS inladen

### CSS strategie
Naarmate er meer CSS in je project komt, bijvoorbeeld als je gaat samenwerken aan een project, wordt het steeds belangrijker om een CSS strategie (met elkaar) te bepalen.

**Opdracht**  
Bekijk, voor onderstaande websites, in de inspector, hoe de css is gemaakt voor een `h2` element en een `button` element.

Beantwoord deze vragen voor onderstaande websites en schrijf op het whiteboard:  
- Welke element selectoren en class selectoren zijn gebruikt?
- Welke properties staan er in welke selectoren?
- Wat valt op aan de naamgeving van classes en custom properties?

Websites:  
- https://css-tricks.com/  
- https://www.smashingmagazine.com/  
- https://fdnd.nl/

### Custom Properties
Met Custom Properties kun je een css value opslaan en op meerdere plekken gebruiken. Hiermee zorg je voor _DRY code_, wat de code beter leesbaar, makkelijker onderhoudbaar en sneller maakt. Dit is fijn voor de developers én de gebruikers.

**Opdracht**  
Gebruik voor values die in de generieke stylesheet vaker voorkomen _Custom Properties_.

Tip: Zet een Custom Property nooit op de _:root_ selector, maar zo diep mogelijk in de _DOM Tree_!

Bronnen:
- [A strategy Guide To CSS Custom Properties](https://www.smashingmagazine.com/2018/05/css-custom-properties-strategy-guide/)
- [Breaking CSS Custom Properties out of :root Might Be a Good Idea](https://css-tricks.com/breaking-css-custom-properties-out-of-root-might-be-a-good-idea/)

**Opdracht (advanced)**  
Een Light en Dark mode op de website helpt gebruikers om de website beter te kunnen bekijken in verschillende omstandigheden. 
Implementeer een Dark Theme, die in ieder geval werkt op basis van de voorkeuren van de gebruiker. Custom Properties kunnen hierbij helpen om onnodige herhaling van bijvoorbeeld CSS values voor kleuren te voorkomen. 

Bron:  
- [Dark Mode in 3 Lines of CSS and Other Adventures](https://dev.to/madsstoumann/dark-mode-in-3-lines-of-css-and-other-adventures-1ljj)

### CSS inladen
Nu je met je team een gemeenschappelijke, generieke stylesheet hebt gemaakt, kan je deze gebruiken in jouw eigen project (leertaak).

**Opdracht**  
Koppel de gemeenschappelijke, generieke stylesheet in de HTML van jouw project (gebruik hiervoor de live link naar de stylesheet op GitHub pages) 
Refactor jouw reeds bestaande lokale stylesheets. Hieruit kan alle overbodige CSS, die nu in de generieke stylesheet staat, worden verwijderd.

