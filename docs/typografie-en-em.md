# Look and Feel - Corporate Identity

## Typografie en EM

<!-- Over fonts, regellengte en responsive layouts coderen met EM, en andere CSS units  -->

In de sprint *Look & Feel* leer je meer technieken over hoe je goede typografie kan ontwerpen en bouwen.

In sprint 2 is typografie en leesbaarheid al een keer behandeld.
De basis regels voor goede leesbare teksten op het web zijn:
De font size is minimaal `16px`, een goede regellengte is 10-12 woorden en niet langer dan `40em` en de regellafstand is `140%`.

```css
body{
    font-family: "Open Sans", Helvetica, sans-serif;
    font-size: 16px;
    line-height: 1.4;
}
```

### Aanpak

Eerst ga je websites analyseren om te leren hoe andere websites typografie toepassen. Daarna onderzoek wat micro- en macro-typografie is en hoe je dat in CSS kan toepasen. 
Daarna ga je oefenen met verschillende CSS units. 

## Typografie en CSS properties

"Web Design is 95% typography"

Dit schrijft het designbureau IA.net. Een website bestaat niet alleen uit titels en de teksten, maar ook uitleg bij foto's, button, en bijvoorbeeld labels van formulier-elementen bevatten tekst. 

In CSS bestaan veel *properties* om fonts goed vorm te geven, zoals `font-family`, `font-weight`, `font-stretch`, `font-variant`, `font-size`.
```css
body{
    font-family: "Open Sans", Arial, sans-serif;
    line-height: 1.4;
    font-weight: normal; 
    font-stretch: normal;
    font-variant: small-caps;
    font-size: 16px;
}
```
Deze *properties* kan je ook met de font *shorthand* schrijven, dat ziet er zo uit: 
```css
body{
    font: normal small-caps normal 16px/1.5 "Open Sans", Arial, sans-serif;
}
```

CSS heeft veel meer mogelijkheden om teksten goed leesbaar te maken zoals de `line-height`, `word-break`, `word-spacing`, `letter-spacing` en `hyphens`. 

### Opdracht

Onderzoek op CSS-Tricks en Github welke CSS *properties* en *values* deze websites gebruiken voor goed leesbare teksten.

Schrijf op het whiteboard de
- font-family
- font-size
- line-height 
- Breedte van het tekst element
- Andere interessante CSS properties voor typografie?

### Bronnen

- [Fundamental text and font styling - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)
- [Font properties en shorthand](https://css-tricks.com/almanac/properties/f/font/)


## Micro- en macro typografie

Je kan onderscheid maken tussen micro- en macro-typografie. Micro-typografie gaat over de details, zoals letters, spatiering, kerning en woordspatiering.
Macro-typogorafie is meer gericht op het font en de layout.

Bijna al deze typografische settings kun je met CSS instellen.

> Micro typography deals with detailed aspects of type and spacing, focusing on the readability of text:
> - Tracking and Glyph-width
> - Protrusion, margin kerning, or hanging punctuation
> - Punctually increasing or decreasing word space
> - Chunking words through word spacing or other white space
>
> Macro typography covers many aspects of what we nowadays call Web design:
> - The Format: The basic dimensions within which we set type
> - The Grid: Type size, proportion of columns
> - The Hierarchy: How the different type sizes and the formatting relate to each other
> 
> [Web Design is 95% Typography](https://ia.net/topics/the-web-is-all-about-typography-period) - Ia.net


### Opdracht

Lees het artikel "Web Design is 95% Typography" en onderzoek met welke CSS properties je micro- en macro-typografie kan toepassen. 
Gebruik hiervoor de lijst op CSS Reference *Typography properties* en *Wrapping and breaking text* van MDN. 


### Bronnen
- [Web Design is 95% Typography](https://web.archive.org/web/20191218153545/https://ia.net/topics/the-web-is-all-about-typography-period)
- https://cssreference.io/typography
- https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_text/Wrapping_breaking_text



## Font-family en lettertypes

Aan de *property* `font-family` kan je de browser 'vertellen' dat verschillende fonts gebruikt mogen worden. 
De browser probeert dan het eerste font te gebruiken, lukt dat niet omdat een font niet beschikbaar is, dan wordt de volgende gebruikt. 
Dat ziet er zo uit: 
```css
body{
    font-family: "Open Sans", Arial, sans-serif;
}
```
Hier probeert de browser eerst een extern font te laden. 
Daarna mag de browser een systeem-font gebruiken. 
Als dat font niet bestaat dan mag de browser zelf een`sans-serif` font gebruiken om de website te renderen. Dit wordt *Fallback* genoemd, zo zorg je ervoor dat de website altijd zo goed mogelijk gerenderd zal worden.

Er bestaan verschillende soorten font-familie soorten, zoals `serif`, `sans-serif` en `monospace`. Zorg ervoor dat je bij de font-family altijd een generiek font naam meegeeft zodat de browser als fallback zelf een passend font gebruikt. 

'Serif' of schreef-letters hebben kleine uitstekels aan de stokken en staarten. 
Die zorgen ervoor dat letters beter van elkaar te onderscheiden zijn, en dus zijn ze beter leesbaar. Zo wordt de leesbaarheid van een tekst verbeterd, dit was vooral van belang toen de drukpersen nog niet zo goed waren. 'Sans'serif' of schreefloze-letters hebben geen schreef. 
![](serif-sans-serif.jpg) 
*Serif letters hebben schreven, sans-serif niet.*

`Monospace' letters zijn allemaal even breed. Voordeel hiervan is dat dat goed uitlijnt. Dit kan je daarom goed gebruiken voor het presenteren van getallen. 

![](monospaced.png) 
*Monospaced letters zijn allemaal even breed*

#### Fonts laden met fallback

Hier (korte) uitleg over @font-face


### Bronnen
- [Web Fonts](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Web_fonts)
- [How to use @font-face in CSS](https://css-tricks.com/snippets/css/using-font-face-in-css/)
- [Font Family - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)


## CSS Units
Font sizes en regellengte met verschillende units
Font size en regellengte met (R)EM


<!-->
Tot slot ga je leren hoe je op basis van de regellengte een responsive layout kan ontwerpen en bouwen. 


## Responsive layout
Responsive desing op bais van regellengt met EM
Wat is beter, pizels of em?
Uitdaging: Grid layout responsive zonder medie queries

Er zijn verschillende manieren(strategieen) om sizes te definieren in CSS. Ook nieuwe manieren > laten zien

Vandaag typografische verhoudingen bepalen aan de hand van EM.
Je kan dan ook de responsive layout hierop baseren, met de regellengte als uitganspunt. Hoe breed is minimaal? Hoe reken je dat uit? En dan een media query, met min width voor een vloeiende opvulling.

Er zijn ook andere manieren om responsive layouts te maken. Op een component. In grid zonder media queries. En in pixels. Kan allemaal ...
-->