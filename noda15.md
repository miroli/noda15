##Noda15 – Anteckningar

__Innehåll__

* 1. Aron Pilhofer
* 2. Kristoffer Örstadius
* 3. VG's do's and don'ts
* 4. Interactive featuremaking (The Guardian)
* 5. What should we expect the readers to know? (Helsingin Sanomat)
* 6. Hur vi byggde #SMPlab? (Sunnmørsposten)
* 7. Live the story, through technology (Immersive Journalism)
* 8. Security matters (Runa Sandvik)

####1. Aron Pilhofer

Inspirerande grejer: [Guantanamo Diary](http://www.theguardian.com/world/guantanamo-diary) av The Guardian, gjordes av deras multimedia-team och deras grafik-team. [Tesco map](http://www.theguardian.com/business/ng-interactive/2015/jan/28/tescos-store-closures-and-abandoned-developments-interactive), de ville inte bara placera ut prickar på en karta, så bestämde sig för att göra en mer innehållsrik variant.

Det fanns förut en princip på NYT om att man skulle byta ut huvudbilden på ettan varje timme, oklart varför. De ifrågasatte och bestämde sig för att mäta hur många besökare som återkommer med och utan bilduppdatering. Ingen skillnad. Viktigt att mäta beteende och sluta påstå saker utan belägg.

Artiklar kan kategoriseras som "givers" och "receivers". Vissa artiklar ökar trafiken till övriga sajten, medan andra är "dead ends". Behöver göras mer sofistikerade analyser av hur besökarna rör sig vidare från ens artiklar.

Varför är just antal klick och antal unika besökare intressant? Se t.ex. Medium som istället mäter lästid. Våra vanliga mätparametrar är anpassade för annonsmakarna.

####2. Kristoffer Örstadius

Dragning om att vara journalist och programmerare. En del om grundläggande kodsyntax, men även om tillvägagångssätt i konkreta projekt.

#####[Myndigheter censurear Wikipediatexter](http://www.dn.se/ekonomi/myndigheter-censurerar-wikipediatexter/):

Byggde först upp en lista över IP-adresser.
[Ripe.net](Ripe.net) användes för att söka på IP-nummer. Free database search. Full text search. Sökte manuellt igenom stora myndigheter som han tyckte var intressanta. Där fick han upp en rad olika IP-nummer som tillhörde t.ex. Försäkringskassan. Sen sökte han på de IP-numrena i Wikipedias sökfunktion. Men eftersom det var miljontals IP-nummer skrev han ett PHP-skript för att kolla resultaten.

Tog 4 månaders att samla in datan. Visade sig sen att Dan Eliasson hade varit inne och redigerat i egen hög person.

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
En journalist lyssnade på Aron Pilhofer på en konferens i Bergen och fick en idé om kreditskulder. Frågade om de kunde göra en interaktiv grej av det. Svaret: Kanske, vad finns det för data? Visade sig att journalisten med idén hade en stor Excelfil med välstrukturerad data på ämnet. Känn till datasituationen innan du går vidare.

_När det blir skarpt nyhetsläge är det bara att släppa allt och jobba med de verktyg man är bekväm med. T.ex. interaktiv karta under terrorattackerna i Paris._

Vidare: Journalisten ville ha en counter på förstasidan med antalet skuldsatta norrmän. Hon ville även ha ett nytt kommentarssystem där folk anonymt kunde kommentera projektet. De byggde systemet. Moderatorna fick bara godkänna kommentarer som var konstruktiva och hade något nytt att säga. Publicerade 40 av över 200.

En annan journalist (i teamet) fick en idé om en guide där besökarna själva kunde se om de var i farozonen för att hamna i en skuldsituation. Blev "Ut av inkasso-fella".

Det hela blev storytellingprojektet [Gjeldskrisen](http://www.vg.no/spesial/2014/inkassokrisen/). Det viktiga för dem var att inte publicera alla siffror, utan aktivt tänka på vad folk är intresserade av. Resulterade i sökfunktionen som filtrerar fram den data som är intressant för besökaren i fråga.

#####Flera typer av storytelling
Tre kategorier de jobbar med:

- "Visual storytelling" (kräver mycket finess, se t.ex. [Laerdal](http://www.vg.no/spesial/2015/laerdal/) som var 50k tecken i tidningen, där den digitala versionen till viss del översattes till visuella element)
- "Longreads" som är mer Snowfall-aktiga (kan bara berättas med text, t.ex. om pojke som begick självmord)
- "The hybrid" (se t.ex. [Mysteriet – Scandinavian Star](http://scandinavian-star.vg.no/)) som inte har en klar storyline, där du snarare försöker berätta en del "substories" som t.ex. Estoniaprojekten.

#####Viktigt att veta om storytelling:

- You need a good storyline
- It's time consuming
- You need some tech to make it work
- You need training to make it great
- Involves tech changes, reusability is at the time is pretty low
- Evaluate

Viktigt att träna sig i digital storytelling. Läsarna älskar det när det blir rätt. Ibland måste du slänga dina bra idéer eller ny teknik du precis har lärt dig, och välja den enkla vägen (men spara dem någonstans, du behöver dem senare).

#####Principer för interaktiva projekt:

- Aim high,
- Go for simplicity and quality if time is short,
- Use common tools (e.g. CartoDB, Tableau, R)
- Make a publishing plan
- Ensure a life on social media
- Always think about the mobile device
- Track your data
- Kill some darlings
- Remember your errors
- HAVE FUN!

####4. Interactive featuremaking (The Guardian)

Med Francesa Panetta, Special Projects Editor. En genomgång av deras digitala projekt.

#####[Bangladesh – The Shirt on Your Back](http://www.theguardian.com/world/ng-interactive/2014/apr/bangladesh-shirt-on-your-back)

Text över film-projekt om klädindustrin i Bangladesh. Följde en fabriksarbetare. Det är en icke-linjär berättelse med grafiska element insprängda i texten.

#####[The view from the Shard](http://www.theguardian.com/artanddesign/interactive/2013/feb/01/view-from-top-shard-london-interactive)

Experiment med ljud i en kartmiljö.

#####[Streetstories – King's Cross](http://www.theguardian.com/mobile/interactive/streetstories-sample-map-with-audio)

En interaktiv guide i stadsmiljö. Känner av ens position och berättar historier om platsen.

#####[Digital Deadly Sins](http://www.theguardian.com/technology/ng-interactive/2014/jun/06/-sp-digital-deadly-sins)

En interaktiv berättelse om människors "synder" i den digitala världen.

#####[First World War](http://www.theguardian.com/world/ng-interactive/2014/jul/23/a-global-guide-to-the-first-world-war-interactive-documentary)

En interaktiv dokumentär om första världskriget med videomaterial från den tiden. Avsikten var att sammanfatta kriget för läsarna, utan att förenkla det alltför mycket. Det var viktigt att göra det till en global berättelse, vilket språkvalet i början vittnar om.

Projektet involverade många personer med olika kompetenser, både internt och externt, t.ex. historiker, programmerare, designers, videoredigerare och representanter från museer.

######Arbetsprocessen

- December 2013: research
- December 2013: hitta vinkeln (som blev det globala kriget)
- December 2013: Koncept (wireframing). Här föddes idén om parallella berättelser.
- December 2013: Ljud, idé om historiker från runtom i världen. Förintervjuer på telefon. Sammanställde deras berättelser i Excel.
- Januari 2014: Inspelningar, experterna kom till Guardians studio och spelade in sina berättelser.
- Januari-februari 2014: Redigering av berättelserna.
- Mars 2014: Interaktiv design, konceptutveckling (Vad är det vi gör?, En eller flera filmer? Interaktion i eller utanför filmerna?). Skisser på papper och wireframing. Designen skulle vara modern, global och inspirerande. Topografin viktig för känslan, därav bakgrundskartan. Navigering bestämdes.
- Januari-juni 2014: Video- och bildresearch. Man gick igenom Imperial War Museums arkiv.
- Mars-juni 2014: Interaktiv media, jobbade med datateamet, museet, praktikanter etc. Började skriva texterna, jobbade med ljuddesignen, skapade gifar, gick igenom Guardians eget arkiv.
- Mars-juni 2014: Byggandet börjar, iterativ process.
- Mars-juni 2014: Översättningar. All text matades in i ett översättningskalkylark. En researcher jobbade heltid med detta.
- Juli 2014: Tester av översättningar och funktionalitet.
- Juli 2014: Marknadsstrategi, social media, pressrelease, intervjuer, Guardians blogg, Superpixie.
- Juli 2014: Lansering, samarbete med andra europeiska tidningar, t.ex. El Pais.
- Juli-december 2014: Nya översättningar med hjälp av crowdsourcing. Kommer snart att lanseras på holländska och indonesiska.

######Utmaningar

- Tidsåtgången
- Att beskriva projektet (utan att veta hur det blir i slutet)
- Personalhantering (många involverade, internt och externt)
- Kostnad (t.ex. billigare att spela in historikernas röster istället för att spela in dem på video)

####5. What should we expect the readers to know?

[Esa Mäkinen](http://www.esamakinen.fi/e/) från Helsingin Sanomat. Om att designa UI för läsarförståelse. De har ett eget verktyg för in-app analytics. Se [denna länk](http://www.hs.fi/aihe/datajournalismi/) för en översikt av tidningens interaktiva projekt.

#####Exempel 1: [The Dress Machine](http://www.hs.fi/kotimaa/a1305901177538)
82k användare, 15k återvändande användare (19%). 1,4 miljoner actions, 17 per användare (högt relativt till deras andra projekt).

37,1% valde år, 21,7% öppnade och stängde klänningar, 8,4% valde färg, 4% valde en annan skärning. Esa besviken på att så få valde färg. De hade hoppats att projektet hade blivit viralt, men det tog aldrig riktigt fart.

#####Exempel 2: [Get yourself a Swedish name](http://www.hs.fi/kotimaa/a1305742444299)
714k öppnade appen. 95,5% klickade på knappen (mycket bra). 4,2% delade på Facebook, vilket är hyfsat bra.

#####Exempel 3: [Check when your name will be popular again](http://www.hs.fi/elama/a1305801877641)
1,3 miljoner besök, varav 343k (26,1%) var siduppdateringar. Endast 1 miljon använde appen (78,5%). 87,7% av de som sökte på sitt namn hittade det i databasen. 3,4% av de som hittade sitt namn delade på Facebook.

#####Exempel 4: [Where to buy a house](http://dynamic.hs.fi/2014/mistaostaa/)
App där man anger sin budget och får en karta över vilka områden man har råd med. 44k användare, 3,9 sökningar per användare, totalt 173k sökningar.

#####"Misslyckade" appar

- [Hockey name generator](http://www.hs.fi/urheilu/a1305821795460): Färre än 10k besökare.
- [Vote for your favorite chocolate](http://www.hs.fi/koti/a1305763184004): Ungefär 10k besökare. Ej värt arbetsinsatsen. Hypotes om oklar röstningsfunktion. Även tajmingproblem, publicerades två dagar före jul.
- [Tensions in the Middle East](http://www.hs.fi/ulkomaat/a1412996026673): Få besök och kort besökstid. Huvudproblem antagligen att den är baserad på musrörelser. Hoverevent anpassade för desktop. Litet typsnitt på mobil.
- [Life of Edward Munch](http://dynamic.hs.fi/2014/munch/): Färre än 10k besökare. Svårt att förstå varför det inte gick hem. Vissa saker fungerar inte lika bra på iOS, kan vara en anledning.

#####Oväntat "lyckade" appar
- [What's your new retirement age](http://www.hs.fi/kotimaa/a1411956233937): Tog ungefär en timme att göra, och blev väldigt populärt, en hel vecka. Konkurrenterna hade vanliga tabeller, och blev inte alls lika populära. Folk gillar att klicka.
- [How lonely are you](http://dynamic.hs.fi/2014/yksinaisyyskysely/index.html): Besökarna svarar på frågor och får respons direkt. Emotionellt ämne.

#####Vad ska man förvänta sig av läsarna?
Ingenting.

#####Saker att akta sig för
Hoverevents är det nya blink, undvik. Sliders är oprecisa på mobil, men svåra att ersätta ibland. Även klick kan vara oprecisa på mobil. Se upp för små klickytor.

3G är det nya [14400](https://en.wikipedia.org/wiki/SupraFAXModem_14400). Se till att mobilanpassa bilder och annat innehåll som kan vara segladdat på mobila nätverk.

WOW! är dött. De flesta wow-effekter bygger på stora bilder och videoklipp, men det ger inte samma intryck på mobil. Dessutom ingen autoplay på mobil.

Endast skroll är universellt.

Var tydlig med vilken slags applikation besökarna har framför sig. Ha gärna med "quiz" i rubriken om det är ett quiz. Små hjälpdetaljer som skyltar, popups etc är underskattat. Behöver inte vara tecken på dålig design.

####6. Sunnmørsposten: Hvordan bygget vi [#SMPlab](https://smpno.wordpress.com/tag/smplab/)?

Om hur Sunmörsposten byggde upp en datajournalistik redaktion.

__Vad är datajournalistik för oss?__ Tre kriterier: ett bra dataunderlag, datafiltrering och digital storytelling.

__Exempelprojekt (namn?):__
Data: 937 domar, lagavsnitt.
Filtrering: Ta fram Sunmörspostens distrikt.
Digital storytelling: Visualisera datan på sajten.

__Hur kom vi igång?__
Under startfasen började vi med att bygga och dela med oss av kompetensen på tidningen. Vi kartlade olika verktyg som fanns tillgängliga, vi körde workshops i huset, och vi gjorde försöksprojekt (i syfte att lära).

Något av det allra första vi gjorde var att skapa Google Fusion-kartor. Steg två var att lägga till lite grafik i kartorna (popups och ikoner).

__Den heliga treenigheten:__ journalistik, webbdesign och programmering. När vi hade detta på plats på redaktionen kunde vi börja jobba.

__Organisering:__ Vi började i en mörk hörna och gick till nyhetsdesken. Det är viktigt att jobba i samspel med resten av redaktionen. Vi sitter två meter från webbredaktionen.

För attt skapa en innovationskultur: Skapa rum för lekfullhet och experiment. Var inte rädd för att misslyckas. Men styr leken i strategiskt viktiga riktningar. Växla mellan datatunga projekt till mer lekfulla storytellingprojekt.

Viktigt med samarbeten på tre områden: andra medieorganisationer, teknologiskt kunniga organisationer och människor, samt universitetsvärlden.

Bygg en öppenhetsfilosofi! Kodkulturen är minst lika viktig som journalistkulturen. Dela med er av kod och idéer och var inte hemlighetsfull om det inte behövs. Blogga! Datajournalistik för oss är en verklig omställning, och alla ska med. Ett projekt med GPS-data för mobiltelefoner involverade exempelvis 17 personer på redaktionen.

Vissa har ifrågasatt varför man ska lägga så mycket resurser på en så smal nisch. Detta behöver motarbetas. Skapa innehåll för hela mediehuset.

__Publikfråga från svenska Stampen:__ _Vad hade programmeraren för bakgrund?_

Svar: Han hade tidigare drivit ett eget företag och hade inte haft med media att göra. Det var dock ett minimalt problem. Kom in i arbetssättet så småningom, och ett nytt perspektiv var nyttigt.

####7. Live the story, through technology

Av programmeraren bakom [Immersive Journalism](http://www.immersivejournalism.com/).

Virtual Reality används i dag mest för spel och simuleringar, men hittar nya användningsområden hela tiden. Immersive Journalism använder den senaste gamingteknologin för att förmedla känslor, väcka besökarens uppmärksamhet, och ge en förstahandsupplevelse av händelser.

Några projekt: Hunger in Los Angeles (2012), Use of Force (2014), Project Syria (2014).

För Project Syria dokumenterade teamet allting, återskapade gator från video och foton och använde autentiska ljudklipp från platserna.

Resten av dragningen går mest ut på att visa exempel och fruktansvärda klipp från Syrien.

####8. Security matters (Runa Sandvik)

Om digital säkerhet, hot och mjukvara.
hgf
[Securedrop](https://freedom.press/securedrop), anonymous whistleblowing platform.

GCHQ har listat "undersökande journalister" på samma hotnivå som terrorister och (illasinnade) hackers (The Guardian, 19 jan).

Använd samma säkerhetstänkande online som offline. Du håller alltid ögonen öppna när du korsar en väg, på samma sätt bör man som journalist även ha ett grundläggande säkerhetstänkande även för helt harmlösa jobb. Viktigt att jobba in säkerhetsrutiner.

Fyra frågor att ställa sig:

- 1. Vilken information vill du låta vara privat?
- 2. Vem vill ha reda på informationen?
- 3. Vad kan de göra för att ta reda på informationen?
- 4. Vad händer om de lyckas?

Efter Snowden har antalet tjänster som kallar sig "NSA-säkra" skjutit i höjden. De flesta är skräp. Runa Sandvik rekommenderar verktyg som är gratis, open source och transparenta. Ingen vits med stängda system som tekniskt kunniga människor inte har försökt att knäcka. Tor är ett exempel på ett system som är fortsatt säkert trots många försök att knäcka den öppna källkoden.

I Europa finns något som heter Key Disclosure Law. Finns exempel på personer som har behövt avkryptera sina hårddiskar innan de går ombord på plan. Finns personer i Storbritannien som avtjänar tvååriga fängelsestraff för att ha vägrat lämna ut sina krypteringslösenord.

Viktigaste för medelstora mediaredaktioner vad gäller säkerhet är att kryptera sina laptops. NRK kommer att tillhandahålla krypterade datorer åt alla sina anställda nästa år.

[Surveillance self-defense](https://ssd.eff.org/) är en uttömmande guide för digital säkerhet.

Tips för att använda Tor:

- 1. Använd inte Tor för att ladda ner torrents.
- 2. Installera inte plugins eller tillägg
- 3. Logga inte in på sidor utan HTTPS
- 4. Din identitet kan avslöjas om du laddar ner filer (t.ex. en Wordfil som kan laddas ner anonymt, men i sin tur innehåller bilder som den inte laddar ner genom Tor)

RedPhone (Android) & Signal (iOS) utvecklas av Open WhisperSystems, och är ett verktyg för att kryptera kommunikation och innehåll på telefoner. Båda parter behöver ha appen installerad.