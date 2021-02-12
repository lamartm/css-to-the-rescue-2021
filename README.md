# Procesverslag
## Week 1

### Waar ik voor gekozen heb
Ik heb voor de CSS Zen opdracht gekozen waarin ik de restaurant menu zal designen. Qua context heb ik ervoor gekozen om de color scheme te laten veranderen gebasseerd op wat de gebruiker prefereerd. Er zullen alleen twee kleuren gebruikt worden (wel alle tinten van de twee kleuren) en ik zal de site responsive maken zonder media queries te gebruiken.

### Welke CSS technieken ik gelijk aan de slag mee zal gaan
Als eerst zal ik de general layout goed proberen te maken met CSS Grid. Dit doe ik eerst om zeker te zijn dat alles responsive is zonder media queries. Het is beter om het nu alvast te doen in plaats van wanneer ik later bijna klaar ben en wellicht problemen zal krijgen die alles mogelijk kunnen verpesten.

### Waar mijn grootste uitdagingen liggen
Ik ga mezelf uitdagen om buiten mijn comfort zone te gaan en SVG animaties te maken. Ik heb dit nooit eerder echt gedaan en zal me daarom ook meer in verdiepen in de komende weken, zodat dit ook iets wordt dat ik later zelf kan gebruiken.

### Schetsen
Dit zijn de schetsen die ik gemaakt heb na de menu te lezen. Alle figuren die je hierin ziet ga ik proberen te maken in SVG en sommige aspecten hiervan te animeren. 
![schets1](https://github.com/lamartm/css-to-the-rescue-2021/blob/master/schetsen/schets4.jpeg)
![schets2](https://github.com/lamartm/css-to-the-rescue-2021/blob/master/schetsen/schets3.jpeg)
![schets3](https://github.com/lamartm/css-to-the-rescue-2021/blob/master/schetsen/schets2.jpeg)
![schets4](https://github.com/lamartm/css-to-the-rescue-2021/blob/master/schetsen/schets1.jpeg)

## Week 2

### :first-child
Ik heb deze week veel met selectoren gewerkt en gespeeld om ze beter te begrijpen. Zo gebruik ik nu in mijn CSS alleen selectoren. 
```
section:first-child header {
    position: relative;
    display: flex;
}
```
### Sessie vormpjes maken
Bij de sessie vormpjes maken zag ik dat je met CSS meer creatieve kracht heb dan ik had gedacht. Ik wou eerst vooral met SVG's werken om de vormpjes te maken die ik in gedachte had, maar nu zal ik dat met vooral HTML en CSS doen. De meer complexe vormpjes kunnen wel mogelijk met SVG gedaan worden, maar ik zal mezelf proberen uit te dagen en dit niet te doen.

Na de sessie ging ik gelijk het zelf proberen te maken in mijn code. Dit was dan het resultaat:

![noshes](https://github.com/lamartm/css-to-the-rescue-2021/blob/master/schetsen/noshes.PNG)

Door linear-gradients (met een transparent gedeelte) te gebruiken als background images in een before & after kan je de ribbon achtige vorm maken:
```
section:first-child header::after, 
section:first-child header::before {
    content: "";
    position: absolute;
    width: 3.5em;
    height: 2.9em;
    bottom:-.6em;
    background-image: 
    linear-gradient(to left top, transparent 50%, rgb(41, 40, 40) 50%),
    linear-gradient(to left bottom, transparent 50%, rgb(41, 40, 40) 50%);
    z-index: -1;
}
```
### Eerste versie
Dit is dan nu mijn eerste versie:
![v1](https://github.com/lamartm/css-to-the-rescue-2021/blob/master/schetsen/v1.PNG)

Er is nog niet veel, maar ik zat me deze week meer te verdiepen in de verschillende manieren om vormpjes te maken in CSS. 
