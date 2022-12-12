---
Title: Analysis
Description: Reports
Template: analysis
---

Laddningstid och användarbarhet
=======================

Denna rapport bygger på observeringar jag gjort utav tre olika sidors laddningstid och användarbarhet. Rapporten tittar på tre webbsidor tillhörande verksamheter inom samma område men med olika inriktning.<br><br>

Urval
-----------------------

Jag valde att fortsätta kolla på samma hemsidor som i föregående rapport då jag tänkte att det kunde vara spännande att fortsätta utvärdera dessa inom andra aspekter. Jag har alltså tittat på tre museum/kulturverksamheter i Norrköping.
<h3>Arbetets museum</h3>
<a href="https://www.arbetetsmuseum.se">Följande länk användes i undersökningen: https://www.arbetetsmuseum.se</a>

<h3>Norrköping Konstmuseum</h3>
<a href="https://www.norrkopingskonstmuseum.se">Följande länk användes i undersökningen: https://www.norrkopingskonstmuseum.se</a>

<h3>Visualiseringscenter</h3>
<a href="https://visualiseringscenter.se">Följande länk användes i undersökningen: https://visualiseringscenter.se</a><br><br>

Metod
-----------------------

Jag använde mig utav två metoder för att analysera webbplatsernas laddningstid och användarbarhet. Först la jag in länkar till hemsidorna på PageSpeed Insights och sammanställde information jag fick fram rörande mobil och desktop i mitt excel-ark. Jag gick sedan in på hemsidorna och kollade i devtools fliken under network. Här fick jag ytterligare information som jag antecknade i mitt excel-ark. Jag kollade sedan lite närmare på informationen i devtools samt på PageSpeed Insight för att försöka utvärdera resultaten och hitta eventuella förbättringsområden.<br><br>

Resultat
-----------------------

Följande excel-ark innehåller all den insamlade datan.
<iframe class="excel-results" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTgpEuLSxpNE2FgUnnmpBgFOr-kszAcZZHcDwtDbteRwD-Qp4IA07cQtjtG2kBqfnS3oixmu1IUddVp/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

<br>
<h3>Arbetets museum</h3>
<div class="container-rapport">
<div><img src="%base_url%/content/analysis/img/arbetsmuseet.png" alt="Arbetets museums webbplats"></div>
<div class="text-rapport">På mobil och desktop framkommer det att Arbetets museum främst border arbeta med sina bilder för att få ned svarstiden på sin webbplats. Enligt PageSpeed Insight kan de bland annat kolla över vilka bildformat som används i nuläget och i fall dessa kan bytas ut mot andra format som ger bättre komprimering. Även sättet som bilderna är kodade på bör ses över och förändras för att de ska kunna läsas in snabbare och förbruka mindre mobildata, ett exempel är att integrera responsiva bildformat eller moduler som automatiskt optimerar och minskar bildstorleken. Utöver att jobba med bilder kan de även reducera ned mängden CSS och javascript genom att ta bort de delar som inte används på sidan. På desktop är det huvudsakligen javascripten som bör ses över och inte lika mycket CSS. När jag kollar i devtools fliken ser jag tydligt att fonts och bilder är det som tar mest minne, så kan dessa reduceras hade det varit positivt.</div>
</div>

<h3>Norrköping Konstmuseum</h3>
<div class="container-rapport">
<div class="text-rapport">Konstmuseum bör se över hur de kan minska serverns svarstid för både mobil och desktop, detta är den förändringen som skulle göra störst skillnad på webbplatsen enligt PageSpeed Insight. Men de bör även på mobil se över bildformaten som används och välja modernare alternativ som komprimerar bilderna. Även Konstmuseet, likt Arbetets museum bör se över CSS och javascript för att reducera bort de delar som inte används. I devtools ser det ut som att de delar som tar mest minne är kopplade till javascript, så ifall dessa kan reduceras ned och rensas hade det antagligen gjort laddningstiden kortare.</div>
<div><img class="hoger-skugga" src="%base_url%/content/analysis/img/konstmuseet.png" alt="Norrköpings Konstmuseum webbplats"></div>
</div>

<h3>Visualiseringscenter</h3>
<div class="container-rapport">
<div><img src="%base_url%/content/analysis/img/visualiseringsc.png" alt="Visualiserings Centrum webbplats"></div>
<div class="text-rapport">Visualiseringscenter bör främst se över deras användning av bilder, på mobil och desktop. De kan få ned sin svarstid avsevärt genom att kolla över sina bildformat samt hur deras bilder är kodade, precis som de andra sidorna jag undersökt. För visualiseringscenter rekommenderas även reducering samt minifiering av deras javascript på mobil och desktop. Detta hade gjort att färre byte behövde skickas via nätverket. Tittar jag i devtools fliken under network syns det även tydligt att de delar som tar upp mest minne är bilderna och de är med stor marginal, så detta är absolut något de bör titta på.</div>
</div>

Analys
-----------------------

Det jag tydligt kan se i min undersökning är att alla tre hemsidor har problem med ungefär samma saker, bilder och mängden oanvänd javascript och CSS. Överlag känns det som ganska enkla saker att ta tag i och förändra, med enkla medel. Bland annat som tidigare nämnt att se över vilka bildformat man använder sig av och istället välja modernare alternativ som bättre komprimerar bilderna. Men även att se över hur bilderna är kodade och utan att tumma på kvaliten justera detta för att få ned mängden data. Då alla tre webbplatser enligt mig visar ganska dåliga resultat när man titar på laddningstiden så känns det högst relevant att både ur ett användar- men också ett miljöperspektiv titta över dessa delar och göra de enkla förändringar som krävs.<br>
Om jag ska rangordna resultaten som jag fått fram så tolkar jag de som att Konstmuseum är bäst, trots att de laddar in flest filer. Tvåa är visualiseringscenter och trea Arbetets museum. Men som sagt anser jag inte att någon av de presterade speciellt bra. Jag skulle säga att man bör komma under 1 sekunds laddningstid (load) för att det för användaren ska vara trevligt att besöka webbplatsen. På flera av de webbplatserna jag undersökt upplever jag det som störande att webbplatsen fortsätter att laddade en tid efter att jag kommit in på hemsidan, då det blir hackigt. Men även om laddningstiden är okej är det ändå viktigt att ha i åtanke vilken mängd data som skickas och om all data faktiskt behöver skickas etc, ur ett miljöperspektiv.<br><br>

Referenser
-----------------------

https://www.norrkopingskonstmuseum.se<br>
https://visualiseringscenter.se<br>
https://www.arbetetsmuseum.se<br><br>

Övrigt
-----------------------

Författare av rapport: Julia Nilsson