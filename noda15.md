##Noda15 – Anteckningar


####1. Aron Pilhofer

Inspirerande grejer: [Guantanamo Diary](http://www.theguardian.com/world/guantanamo-diary) av The Guardian, gjordes av deras multimedia-team och deras grafik-team. [Tesco map](http://www.theguardian.com/business/ng-interactive/2015/jan/28/tescos-store-closures-and-abandoned-developments-interactive), de ville inte bara placera ut prickar på en karta, så bestämde sig för att göra en mer innehållsrik variant.

Det fanns förut en princip på NYT om att man skulle byta ut huvudbilden på ettan varje timme, oklart varför. De ifrågasatte och bestämde sig för att mäta hur många besökare som återkommer med och utan bilduppdatering. Ingen skillnad. Viktigt att mäta beteende och sluta påstå saker utan belägg.

Artiklar kan kategoriseras som "givers" och "receivers". Vissa artiklar ökar trafiken till övriga sajten, medan andra är "dead ends". Behöver göras mer sofistikerade analyser av hur besökarna rör sig vidare från ens artiklar.

Varför är just antal klick och antal unika besökare intressant? Se t.ex. Medium som istället mäter lästid. Våra vanliga mätparametrar är anpassade för annonsmakarna.

####2. Kristoffer Örstadius

#####[Myndigheter censurear Wikipediatexter](http://www.dn.se/ekonomi/myndigheter-censurerar-wikipediatexter/):
Dan Eliasson.

Byggde först upp en lista över IP-adresser.
[Ripe.net](Ripe.net) användes för att söka på IP-nummer. Free database search. Full text search. Sökte manuellt igenom stora myndigheter som han tyckte var intressanta. Där fick han upp en rad olika IP-nummer som tillhörde t.ex. Försäkringskassan. Sen sökte han på de IP-numrena i Wikipedias sökfunktion. Men eftersom det var miljontals IP-nummer skrev han ett PHP-skript för att kolla resultaten.

Tog 4 månaders att samla in datan.

#####Oddsen för litteraturpriset:
Skript som en gång i timmen gick in på de fem största bettingsajterna och kollade oddsen före utdelningen. Hade historiskt tenderat att sjunka timmarna före utdelning. Visade sig stämma även den här gången. Antagligen läcka i kommittén.

#####Skolgranskningen:
Undersökte vilka som kom in på lärarprogrammet. Hittade en programmerare på högskoleverket. Sa att han inte hade fått hjälp från pressjouren. Frågade om hur deras databas såg ut och byggde upp ett förtroende därifrån. Visade sig i slutändan att 123 personer kom in på programmet med 0.1 i betyg på högskoleprovet.

#####Polisgräv:
Granska officiell statistik (BRÅ). Kan man se om det fuskades med siffror i inrapporteringen? Tankade ner Excelfiler etc, om t.ex. uppklaringssiffror. Mellan 2010 och 2011 löste polisen fler brott än de gjort tidigare, och skröt om detta. Men det visade sig att ett brott blev 10 990 uppklarade brott. En liga i Skåne som smugglat grejer, polisen hade kodat varje tablett som ett brott.

#####Vädergranskning:
Tankade hem data om vädret dagen efter, och jämförde sen hur bra de stämmer överens. Stämde bara vid hälften av tillfällena.

####3. VG's do's and don'ts (lärdomar 2014)

VG:s datajournalistikteam: en programmerare/datajournalist, två designers, och en "journalist in a new way". En ny anställd börjar i april.

#####Dålig process
Bli kontaktad av printreporter som har en färdigskriven artikel och som vill att man gör något med relaterad data "som säkert finns där", och publicera något NYT-mässigt tre dagar före publicering.

#####En bättre process
En journalist lyssnade på Aron Pilhofer på en konferens i Bergen och fick en idé om kreditskulder. Frågade om de kunde göra en interaktiv grej av det. Svaret: Kanske, vad finns det för data? Visade sig att journalisten med idén hade en stor Excelfil med välstrukturerad data på ämnet. __Första poängen__: Känn till datasituationen innan du går vidare.

_När det blir skarpt nyhetsläge är det bara att släppa allt och jobba med de verktyg man är bekväm med. T.ex. interaktiv karta under terrorattackerna i Paris._

Vidare: Journalisten ville ha en counter på förstasidan med antalet skuldsatta norrmän. Hon ville även ha ett nytt kommentarssystem där folk anonymt kunde kommentera projektet. De byggde systemet. Moderatorna fick bara godkänna kommentarer som var konstruktiva och hade något nytt att säga. Publicerade 40 av över 200.

En annan journalist (i teamet) fick en idé om en guide där besökarna själva kunde se om de var i farozonen för att hamna i en skuldsituation. Blev "Ut av inkasso-fella".

Det hela blev storytellingprojektet [Gjeldskrisen](http://www.vg.no/spesial/2014/inkassokrisen/). Det viktiga för dem var att inte publicera alla siffror, utan aktivt tänka på vad folk är intresserade av. Resulterade i sökfunktionen som filtrerar fram den data som är intressant för besökaren i fråga.

#####Flera typer av storytelling
Tre kategorier de jobbar med: "Visual storytelling" (kräver mycket finess, se t.ex. [Laerdal](http://www.vg.no/spesial/2015/laerdal/) som var 50k tecken i tidningen, där den digitala versionen till viss del översattes till visuella element), "longreads" som är mer Snowfall-aktiga (kan bara berättas med text, t.ex. om pojke som begick självmord), och "the hybrid" (se t.ex. [Mysteriet – Scandinavian Star](http://scandinavian-star.vg.no/)) som inte har en klar storyline, där du snarare försöker berätta en del "substories" som t.ex. Estoniaprojekten.

######Viktigt att veta:

- You need a good storyline
- It's time consuming
- You need some tech to make it work
- You need training to make i great
- Involves tech changes, reusability is at the time is pretty low
- Evaluate

Viktigt att träna sig i digital storytelling. Läsarna älskar det när det blir rätt.