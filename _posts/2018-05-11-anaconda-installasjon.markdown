---
layout: post
title:  "Installasjon av anaconda for MacOS"
date:   2018-05-11 10:25:43 +0200
categories: anaconda python
---

## Last ned anaconda distribusjonen fra 
Last ned anaconda fra [anaconda][anaconda] sitt nettsted. (![Download]({{ "/assets/img/download_button.png" | absolute_url }})-knapp øverst i høyre hjørne)
Vanligvis vil nettstedet se hvilket operativsystem du har. Dersom den ikke gjør det velger du manuelt mellom MacOS, Windows eller Linux. 
![My helpful screenshot]({{ "/assets/img/download_site_small.jpg" | absolute_url }})
Velg Python 3.6-versjonen. Før nedlasting kan det hende du blir bedt om å registrere deg, da er det bare å klikke på {% include button.html button_name="No Thanks" button_class="primary" %}. 


## Installer anaconda
Knapper å trykke riktig på underveis. 

## Sjekk at anaconda-installasjonen fungerer som den skal 
I det følgende vil `>>` brukes som *python-prompt*, altså at man gir en instruksjon til python-interpreteren på maskinen. Dette svarer til det stedet i anaconda der man kan skrive inn kommandoer direkte (se bilde). 

Den første sjekken er `>> print("Hello World")`

### Er anaconda installert med nødvendige pakker?
Kopier innholdet i kodesnutten under, og legg det inn i et nytt script i anaconda. Kjør deretter scriptet. 

{% highlight python %}
from pylab import *
print("Hello, World")
t = linspace(0, 3, 100)
A = x**2
plot(t, A)
xlabel("tid")
ylabel("amplitude")
show()
{% endhighlight %}

Dersom alt har gått bra skal du nå få opp en figure som viser $math$x^2$/math$-funksjonen. Dersom dette ikke fungerer bør du ha fått opp en feilmelding.  

### Innstillinger i Anaconda
Det er mange innstillinger i Anaconda, og mange ting er smak og behag. For at alle skal ha samme oppsett når vi er på kurs, slik at vi unngår unødig feilsøking, har vi følgende forslag til innstillinger: 

La anaconda slette variable mellom kjøringer. Dette hindrer masse uventet oppførsel.


[anaconda]: https://www.anaconda.com/
