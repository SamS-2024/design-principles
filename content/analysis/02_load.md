
Laddningstid och användarbarhet
=================================

Den här uppgiften handlar om att analysera prestandan hos tre olika svenska webbplatser. Analysen inkluderar bland annat att mäta laddningstider, resursanvändning och sidstorlek. Det hjälper till att förstå hur webbplatser kan optimeras för bättre användarupplevelse och högre effektivitet.

#Urval
-----------------------
För att genomföra analysen valdes tre svenska webbplatser med olika syften och målgrupper. Dagens Nyheter (dn.se), en nyhetssida som representerar media. IKEA (ikea.se), en e-handelsplattform. Försäkringskassan (forsakringskassan.se), en offentlig webbsida.

Webbplatserna valdes för att få en variation i typ av innehåll och teknisk implementering, vilket ger möjlighet att jämföra prestanda och optimeringsnivåer inom olika kategorier.


#Metod
-----------------------
För att analysera webbplatsens användarbarhet och laddningstider användes två verktyg. Google PageSpeed Insights för att bland annat mäta webbplatsens prestanda, största synliga innehåll (Largest Contentful Paint), interaktivitet (Total Blocking Time) och hur snabbt innehåll visas (Speed Index). DevTools Network i Firefox för att mäta laddningstid, antal resurser och sidstorlek. Mätningarna dokumenterades i ett kalkylark.

Det första steget var att kopiera länkarna till webbplatserna och klistra in dem i PageSpeed Insights, en i taget. Varje webbplats undersöktes först i mobilt läge och sedan i desktop-läge. Från varje webbplats valdes tre olika sidor att analysera: en huvudsida och två andra sidor, exempelvis en kontaktsida eller en inloggningssida.

För att använda DevTools högerklickades på webbplatsen och "Inspect" valdes. Därefter valdes fliken "Network". I slutet av sidan visades olika resultat, som laddningstid, antal resurser och storlek. Sidan laddades om efter att cachen rensats för att hämta nya värden. Totalt genomfördes tre mätningar per sida och medelvärden beräknades.

De uppmätta värdena, tillsammans med övriga data från PageSpeed Insights, dokumenterades i ett Google Kalkylark. Där finns det även länkar till alla sidor som har undersökts.

#Resultat
-----------------------

<h2 class="website-title">Dagens nyheter</h2>

![Dagens nyheter](%base_url%/image/DN.png?w=800&h=800&q=70){.snapshot}

Mätningarna från Dagens Nyheter visar att mobilversionerna av huvudsidan, ekonomi och sport har sämre prestanda än desktopversionerna. Largest Contentful Paint (LCP) är långsam i mobilversionen också, särskilt på huvudsidan (6,5 sekunder), vilket innebär att stora innehållselement tar tid att ladda. 

Dessutom är Total Blocking Time (TBT) högre på mobilen (1 490 ms), vilket kan påverka interaktiviteten negativt.

Desktopversionerna presterar bättre, med LCP under 1,5 sekunder och TBT under 200 ms, vilket ger en snabbare och mer interaktiv användarupplevelse. Samtliga sidor presterar dock högt inom bästa metoder, tillgänglighet och SEO.

I DevTools visade mätningarna att laddningstiden för sidan varierade mellan 1,01 och 1,15 sekunder, med ett genomsnitt på 1,09 sekunder. Antalet resurser som laddades varierade mellan 182 och 282. Den totala storleken på sidan låg mellan 7,02 MB och 8,78 MB, med ett genomsnitt på 7,91 MB. Detta innebär att sidan laddade en ganska stor mängd data, vilket kan påverka visningstiden för användarna.

Dagens Nyheter kan förbättra prestandan på sina mobilsidor genom att optimera stora innehållselement för att minska Largest Contentful Paint (LCP) och reducera Total Blocking Time (TBT), samt minska antalet och storleken på resurser som laddas för att förbättra laddningstiderna.

<h2 class="website-title">IKEA</h2>

![IKEA](%base_url%/image/IKEA.png?w=800&h=800&q=70){.snapshot}

Mätningarna för IKEA visar att mobilversionerna har betydligt lägre prestanda än desktopversionerna. På mobilversionen av huvudsidan är Largest Contentful Paint (LCP) mycket lång, med 16,2 sekunder, vilket innebär att stora synliga innehållselement tar lång tid att laddas. Total Blocking Time (TBT) är också hög, särskilt på huvudsidan (6 670 ms), vilket kan fördröja interaktiviteten. Den totala laddningstiden är även hög, 9,2 sekunder för huvudsidan.

Desktopversionerna av huvudsidan, "Följ min order" och kontaktsidan har bättre prestanda. LCP är mycket snabbare, under 3,5 sekunder på alla sidor, och TBT är lägre, vilket gör att sidorna laddas snabbare och blir interaktiva på en kortare tid. 

Tillgängligheten och SEO-poängen är generellt bra, men det finns utrymme för att förbättra dessa för vissa sidor samt hastigheten på mobilversionerna.

Från DevTools visade mätningarna att sidan laddade på ungefär samma sätt under de tre testerna. Den totala laddningstiden varierade mellan 1,77 och 2,22 sekunder. Antalet resurser som laddades varierade mellan 149 och 156, och den totala storleken på de nedladdade resurserna var mellan 6,11 MB och 6,38 MB. Detta tyder på att IKEA:s huvudsida laddar flera resurser och att dessa kan vara relativt stora, vilket kan påverka användarupplevelsen, särskilt på mobila enheter. Med ett genomsnitt på 6,26 MB, visar detta att sidan använder en stor mängd data vid varje besök.

IKEA kan förbättra prestandan på sina mobilsidor genom att minska Largest Contentful Paint (LCP) och Total Blocking Time (TBT) samt optimera resursstorlekar och antalet filer som laddas, för att korta ned laddningstiderna och förbättra användarupplevelsen.


<h2 class="website-title">Försäkringskassan</h2>

![Försäkringskassan](%base_url%/image/FK.png?w=800&h=800&q=70){.snapshot}

Mätningarna för Försäkringskassan visar att desktopversionerna har bra prestanda med höga poäng för både prestanda och användarupplevelse. På dessa sidor laddas innehållet snabbt och blir interaktivt inom en kort tidsperiod. Mobilversionerna, å andra sidan, har lägre poäng och längre laddningstider, särskilt på inloggningssidan där LCP och Total Blocking Time är högre. 

Trots detta uppnår samtliga sidor höga poäng i Tillgänglighet och Bästa metoder. SEO-poängen är också bra, även om förbättringar kan göras för mobilversionerna, särskilt på inloggningssidan.

Mätningarna från DevTools visade att sidan hade en relativt stabil laddningstid under de tre testerna, med ett genomsnitt på cirka 2,08 sekunder. Antalet resurser som laddades var mellan 90 och 94, och den totala storleken på resurserna varierade mellan 3,79 MB och 4,41 MB. Detta tyder på att sidan är effektiv när det gäller att hantera resurser och data, vilket kan bidra till en bättre användarupplevelse, särskilt för användare med långsammare internetanslutningar.

Försäkringskassan kan förbättra sina mobilversioner genom att optimera laddningstiderna, särskilt för inloggningssidan, och minska Total Blocking Time (TBT) och Largest Contentful Paint (LCP) för att förbättra användarupplevelsen ytterligare.

#Analys
-----------------------

Sammanfattningsvis visar resultaten att mobilversionerna av webbplatser generellt har sämre prestanda än desktopversionerna. De vanligaste problemen inkluderar långa laddningstider, särskilt för stora innehållselement (Largest Contentful Paint, LCP), samt höga värden för Total Blocking Time (TBT), vilket påverkar hur snabbt sidorna blir interaktiva. För vissa sidor, bidrar stora resurser och hög dataanvändning till dessa problem.

Gemensamma förbättringsåtgärder för de analyserade webbplatserna innefattar:

Optimering av resurser för mobila enheter: Bilder och andra stora filer kan komprimeras för att minska laddningstiderna.

Förbättrad kodoptimering: Genom att minska Total Blocking Time kan interaktiviteten på webbplatserna förbättras.

Effektiv hantering av resurser: Att minska mängden data som laddas per besök kan förbättra prestandan och upplevelsen, särskilt på mobila enheter.

Webbplatsernas styrkor ligger i tillgänglighet och bästa metoder, där samtliga sidor presterade väl. Därför bör fokus främst ligga på att förbättra laddningshastighet och interaktivitet, särskilt för mobila användare, för att skapa en mer balanserad användarupplevelse.


#Rangordning och vinnare i testet
-----------------------------------

Baserat på mätvärdena kan webbplatserna rangordnas som följer:

1- Försäkringskassan – Trots att mobilversionen speciellt för inloggningssidan har brister i prestanda, har Försäkringskassan överlag de bästa resultaten. Desktopversionerna presterar mycket bra med snabb laddningstid, låg Total Blocking Time (TBT), och höga poäng för tillgänglighet.

2- Dagens Nyheter (DN) – DN:s desktopversioner presterar väl med snabba laddningstider och höga SEO-poäng. Mobilversionerna har dock lägre prestanda, särskilt när det gäller LCP och TBT, vilket påverkar användarupplevelsen negativt. DN har dock en fördel i att dess sidor är innehållsrika och visuellt stabila, med höga poäng för tillgänglighet och bästa metoder.

3- IKEA – IKEA:s mobilversioner presterar sämst i testet, med långa laddningstider, högt LCP och mycket hög TBT, särskilt på huvudsidan. Desktopversionerna är däremot relativt bra, men jämfört med de andra webbplatserna är deras genomsnittliga prestanda lägre. Dessutom bidrar stora resursfiler och höga datamängder till längre laddningstider.

Försäkringskassan utses som vinnare i testet tack vare dess konsekvent höga poäng på desktopversionerna och goda resultat för tillgänglighet. DN kommer på andra plats tack vare bra desktopprestanda, SEO poäng, bästa metoder och tillgänglighet. Men förlorar på prestanda och total blocking time. DN:s 'First Contentful Paint' och 'Largest Contentful Paint' siffror var bättre än försäkringskassan i mobilversioner överlag så beslutet var inte enkelt i den punkten men generell prestanda fick avgöra till slut.

IKEA hamnar sist på grund av de stora bristerna i mobilprestanda, vilket är särskilt kritiskt eftersom mobila användare ofta förväntar sig snabb och smidig tillgång till information och tjänster. Också hade IKEA högre siffror i 'Largest Contentful Paint' och i 'Total Blocking Time' överlag samt lägre siffror i prestanda.

#Vilken laddningstid uppfattas som snabb eller långsam för webbplatserna?
--------------------------------------------------------------------------

En gräns på 2 sekunder för absolut laddningstid upplevs som snabb, medan över 3 sekunder anses långsam. För desktopversionerna klarar alla webbsidor gränsen. DN ligger i topp med medelvärde på 1.09 sekunder.<br><br>


<iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQI36m3gPvtLJh2Mmz4gyPgCVRC9fGwFFV-apYawRY1kQnR5PG-AjsJ7aAzEry3I6i09PY1grH7ERqn/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" class="spread-sheet"></iframe>