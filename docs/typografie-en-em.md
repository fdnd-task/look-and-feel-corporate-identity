# Look and Feel - Corporate Identity

## Typografie en EM

<!-- Over fonts, regellengte en responsive layouts coderen met EM, en andere CSS units  -->

In deze sprint *Look & Feel* leer je meer CSS technieken voor typografie.

In sprint 2 heb je geleerd de basis regels voor goede leesbare teksten op het web geleerd:
De font size is minimaal `16px`, een goede regellengte is 10-12 woorden en niet langer dan `40em` en de regellafstand is `140%`.

```css
body{
    font-family: "Open Sans", Helvetica, sans-serif;
    font-size: 16px;
    line-height: 1.4;
}
```

### Aanpak

Eerst ga je websites analyseren om te leren hoe websites typografie toepassen. Daarna ga je onderzoek wat micro- en macro-typografie is en hoe je dat in CSS kan toepasen. 
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

Onderzoek de [artikelpagina van de Correspondent](https://decorrespondent.nl/15628/alarm-slaan-of-beter-bewijs-zoeken-de-wetenschappelijke-strijd-achter-kantelpunten-in-het-klimaat/babb3b1e-e017-0dcf-24e7-044ff58251d1) en een [artikel van Pixel Ambacht](https://pixelambacht.nl/2021/optical-size-hidden-superpower/) de *properties* en *values* die de websites gebruiken voor goed leesbare teksten.

Schrijf op het whiteboard de
- font-family
- font-size
- line-height 
- Breedte van het tekst element
- Andere interessante CSS properties voor typografie?

### Bronnen

- [Fundamental text and font styling - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)
- [Font properties en shorthand](https://css-tricks.com/almanac/properties/f/font/)



## Font-family en lettertypes

Met de *property* `font-family` kan je de browser 'vertellen' welke fonts gebruikt mag worden. 
Dat ziet er zo uit: 
```css
body{
    font-family: "Open Sans", Arial, sans-serif;
}
```
Hier probeert de browser eerst een extern font te gebruiken. Als dat font niet lukt mag de browser een systeem-font gebruiken. 
Als dat font niet bestaat dan mag de browser zelf een`sans-serif` font gebruiken om de website te renderen. Dit wordt *Fallback* genoemd, zo zorg je ervoor dat de website altijd zo goed mogelijk gerenderd zal worden.

Er bestaan verschillende soorten font-familie soorten, zoals `serif`, `sans-serif` en `monospace`. Zorg ervoor dat je bij de font-family altijd een generiek font naam meegeeft zodat de browser als fallback zelf een passend font gebruikt. 

'Serif' of schreef-letters hebben kleine uitsteeksels aan de stokken en staarten. 
Die zorgen ervoor dat letters beter van elkaar te onderscheiden zijn, en dus zijn ze beter leesbaar. Zo wordt de leesbaarheid van een tekst verbeterd, dit was vooral van belang toen de drukpersen nog niet zo goed waren. 'Sans'serif' of schreefloze-letters hebben geen schreef. 
![](serif-sans-serif.jpg) 
*Het verschil tussen schreef  (Serif) en schreef-loze (Sans-Serif) lettertypes.*

`Monospace' letters zijn allemaal even breed. Voordeel hiervan is dat ze goed uitlijnt. Dit kan je daarom goed gebruiken voor het presenteren van getallen. 

![](monospaced.png) 
*Monospaced letters zijn allemaal even breed.*

### Fonts laden

Het is mogelijk om voor jouw website een extern font in te laden. Hiervoor gebruik je `@font-face`. Je roept hiervoor een extern font bestand aan, nadat het geladen is kan je het gebruiken voor je styling. 
```css
@font-face{
    font-family: "Open Sans";
    src: url('opensan.woff2') format('woff2'),
}
body{
    font-family: "Open Sans", Arial, sans-serif;
}
```
Op deze manier kan je lettertypes gebruiken die niet standaard door een browser gebruikt kunnen worden. 

### Bronnen
- [Web Fonts](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Web_fonts)
- [Font Family - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family)
- [How to use @font-face in CSS](https://css-tricks.com/snippets/css/using-font-face-in-css/)
- [A complete collection of web safe CSS font stacks](https://www.cssfontstack.com)




## Micro- en macro-typografie

In typografie is er onderscheid tussen micro- en macro-typografie. Micro-typografie gaat over de details, zoals letters, spatiering, kerning en woordspatiering.
Macro-typogorafie is meer gericht op het font en de layout.

Bijna al deze typografische settings kun je met CSS (en HTML) aanpassen.

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
- [Typography properties - CSS Reference](https://cssreference.io/typography)
- [Wrapping and Breaking text - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_text/Wrapping_breaking_text)





## CSS Units

In CSS bestaan er heel veel *units* die je kan gebruiken. 

Er bestaan *absolute length units*, zoals de px (pixel). *Font-relative length units*, zoals de EM en REM. *Viewport relative units* zoals de vw en vh die afhaneklijk zijn can de breedtje of hoogte van de viewpoort. En nog veel meer ...

De EM is een *Font-relative length units*. 
In oorsprong is het de breedthe van de hoofdletter "M" van het lettertype. De EM is een 'relative unit', het is afhankelijk van het font, de font-size en de DPI settings. Het wordt vaak gebruikt voor `font-size` en regellengte omdat je in verhouding tot het font de typografische waardes kan bepaken. 

### opdracht
Om te leren wat je zoal kan doen met al die verschillende CSS units ga je de lengte van een zin op verschillende manieren bouwen. 

De beroemde grafisch ontwerper Robert Bringhurst komt tot het uitgangspunten: een goede regellengte heeft 45-75 karakters, oftwel 10–12 woorden. 

Gebruik verschillende CSS units om ervoor te zorgen dat de regellengte van onderstaande zin op 10-12 woorden komt. Raadpleeg het artikel "CSS values and units" van MDN. Leg uit in je Learning log wat er gebeurt. 
- Behalve pixels zijn de *Absolute length units* voor het web niet geschikt, lukt het je toch om met `cm` of `mm` een regel van zo'n 10-12 woorden te maken? Hoeveel `px` is dat? 
- Gebruik daarna de *Font-relative length units*. Hoeveel `em` heb je nodig voor een goede regellengte? En in `ch` dan? Wat is het verschil als je `rem` gebruikt? 
- Experimenteer tot slot met *Viewport relative units* en *Container units*, zoals `vw` en `cqw`. En wat doen`dvw` of `vmax`?

Open je code editor en maak een blanco HTML pagina, noem het file `typography.html` en sla deze op in de repo van je leertaak. 
Maak een leeg CSS file, noem het `typography.css`, sla het op in dezelfde map als het HTML file.  Voeg het CSS file toe aan het HTML file. 

Gebruik onderstaande HTML *snippet* voor de experimenten: 

```html
<article>
  <blockquote cite="http://webtypography.net/2.1.2">
    <p>Anything from 45 to 75 characters is widely regarded as a satisfactory line length for a single-column page set in a serifed text face in a text size. The 66-character line (counting both letters and spaces) is widely regarded as ideal. For multiple column work, a better average is 40 to 50 characters.</p>
  </blockquote>
  <p>—Robert Bringhurst</p>
  </article>
```




### Bronnen

- [CSS values and units - MDN](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)
- [The amazing em unit and other best practices](https://www.w3.org/Style/LieBos3e/em)
- [Em (typography) - Wikipedia](https://en.wikipedia.org/wiki/Em_(typography))



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