---
title: Hvor Tunge og Indtrængende Er Danske Mediers Hjemmesider?
date: 2015-08-11 18:00:00
excerpt: Danske mediers sider og artikler er fyldt med tredjepartsressourcer.

slug: fremtidens-og-fortidens-mediehjemmesider
categories: [da, articles]

layout: post
author: ndarville
---
<style>
    tr td:nth-child(2),
    tr td:nth-child(3),
    tr td:nth-child(4) {
        font-family: "Courier New", Consolata, monospace;
    }
</style>

<!-- Uddybende

1. Reproducér test
    - Sammenlign med oprindelig artikel
    - Prøv i Chrome Canary
    - Spørg forfatter om uoverensstemmelser

-->

<i>(Denne artikel er et publiceret udkast. Frem for at lægge en artikel, der næsten er færdig, ned i skrivebordsskuffen, bliver den i stedet publiceret i sin ufærdige form.)</i>

For nylig kom chefredaktøren for netmagasinet <i>The Verge</i> for skade ved at kritisere Internettets tilstand, hvor især browsere fik med stokken.

Det viste sig nemlig, at [<i>The Verge</i> selv har én af de tungeste og sløveste hjemmesider på internettet][us-test] med artikler, der kan beløbe sig op til 10 MB i størrelse. Heriblandt den pågældende artikel.

En nærmere granskning af andre amerikanske sider viste, at der var plads til forbedring, selv med alle de mange dårlige undskyldninger redaktørerne har.

Det er på sin plads at foretage samme test i dansk regi for at kigge mediebilledet efter i sømmene.

Testen er foretaget i browseren Chrome Canary med mobilsimulationsprofilen:

* 3G-netværk (350 kB/s)
* iPhone 5 (320&times;568)

Der er derfor tale om en lidt anden opsætning end det amerikanske blogindlæg, så tallene skal ikke holdes direkte op imod hinanden.

Der skal tages følgende forbehold:

1. Testen er foretaget med ad-blockers slået fra.
2. Indhold kan variere for abonnenter eller folk med log-in.
    - Testen er foretaget uden log-in-cookies.
3. Nogle sider indlæser mere indhold, hvis man scroller længere ned.
    - Testen er foretaget uden nogen interaktioner.
4. Siderne vil næsten altid hente mere indhold, jo længere testen kører.
    - Testmålingerne er taget fra, når siden når et indlæsningsplateau.

Artiklerne er valgt ved at tage den mest prominente forsideartikel på siden.

Der er målt på tre parametre i testen:

1. **Requests:** Antallet af ressourcer mobilen henter (efterspørger) på siden.
2. **Data:** Hvor meget data mobilen henter på siden målt i megabytes (MB).
3. **Load-tid:** Tiden det tager at indlæse siden.
    - Load-tid er for *hele* siden---ikke bare artikelteksten.

### DR ###

 Sektion         | Requests | Data   | Load-tid
:----------------|---------:|-------:|---------:
 [Forside][dr-f] |       78 | 1,8 MB | 19,74 s
 [Artikel][dr-a] |      112 | 2,4 MB | 25,67 s

DR benytter <i>lazy loading</i>, hvilket gør, at siden kun indlæser de elementer, brugeren kan se på skærmen. Resten af siden indlæses først, når man manuelt bevæger sig længere ned på siden. Dette er én af årsagerne til, at DR har den hurtigste og letteste forside. Denne metode er udgangspunktet for testens ovennævnte tredje forbehold.

Det skal siges, at DR modsat konkurrenterne som statsejet medie ikke er afhængige af reklameindtægter, hvorfor deres side ikke er tilplastret med reklamer, der gør siden sløvere, og som helst skal indlæses med det samme for besøgende.

Dermed ikke sagt at medier er undskyldt for at anvende reklamer og tracking-scripts.

### TV 2 ###

 Sektion          | Requests | Data   | Load-tid
:-----------------|---------:|-------:|---------:
 [Forside][tv2-f] |      312 | 4,6 MB | 52,83 s
 [Artikel][tv2-a] |      178 | 3,0 MB | 15,49 s

### Politiken ###

 Sektion          | Requests | Data   | Load-tid
:-----------------|---------:|-------:|---------:
 [Forside][pol-f] |      554 | 6,3 MB | 50,30 s
 [Artikel][pol-a] |      421 | 4,9 MB | 32,06 s

Testen blev stoppet efter 7,5 minutter, da siderne fortsatte med at sende requests i samme tempo som fem minutter før.

### Berlingske ###

 Sektion        | Requests | Data   | Load-tid
:---------------|---------:|-------:|---------:
 [Forside][b-f] |      386 | 4,0 MB | 48,86 s
 [Artikel][b-a] |      181 | 2,0 MB | 23,40 s

Da førstehistorien linkede til **Politiko.dk** i stedet for **b.dk**, blev artiklen nedenunder valgt i stedet.

Forsidetesten blev stoppet efter 7,5 minutter af samme grund som Politiken-testen. Artiklen havde ikke samme problem, og testen blev afsluttet tidligere.

### Jyllands-Posten ###

 Sektion         | Requests | Data   | Load-tid
:----------------|---------:|-------:|---------:
 [Forside][jp-f] |      172 | 2,7 MB | 30,65 s
 [Artikel][jp-a] |      111 | 1,1 MB | 15,19 s

### Børsen ###

 Sektion          | Requests | Data   | Load-tid
:-----------------|---------:|-------:|---------:
 [Forside][boe-f] |      313 | 2,5 MB | 30,01 s
 [Artikel][boe-a] |      152 | 2,5 MB | 24,80 s

Forsidetesten blev stoppet efter 7,5 minutter af samme grund som Politiken-testen. Artiklen havde ikke samme problem, og testen blev afsluttet tidligere.

### Information ###

 Sektion          | Requests | Data   | Load-tid
:-----------------|---------:|-------:|---------:
 [Forside][inf-f] |      207 | 5,2 MB | 43,74 s
 [Artikel][inf-a] |      154 | 2,9 MB | 24,03 s

### Hafnia Times ###

Ret skal være ret; tid til selvransagelse.

 Sektion          | Requests | Data       | Load-tid
:-----------------|---------:|-----------:|---------:
 [Forside][ht-f]  |       10 |  57 **k**B | 1,02 s
 [Artikel][ht-a]  |       16 | 264 **k**B | 2,71 s

Det kunne godt gøres lidt hurtigere. For eksempel indlæses skribentbilledet tre gange, hvilket giver et spild på hele 32,2 kB.

Bemærk, at der er tale om **kB**; det vil sige, at forsiden og artiklen fylder henholdsvist 0,057 og 0,264 MB[^mb] sammenlignet med de andre sider.

[^mb]: Forsiden og artiklen fylder endnu mindre, hvis man opgør 1 MB som 1.024 kB.

### Sammenfatning ###

#### Forsider ####

 Medie        | Requests | Data   | Load-tid
:-------------|---------:|-------:|---------:
 DR           |       78 | 1,8 MB | 19,74 s
 TV 2         |      312 | 4,6 MB | 52,83 s
 Politiken    |      554 | 6,3 MB | 50,30 s
 Berlingske   |      386 | 4,0 MB | 48,86 s
 JP           |      172 | 2,7 MB | 30,65 s
 Børsen       |      313 | 2,5 MB | 30,01 s
 Information  |      207 | 5,2 MB | 43,74 s

 Medie        | Requests | Data      | Load-tid
:-------------|---------:|----------:|---------:
 Hafnia Times |       10 | 57 **k**B | 1,02 s

#### Artikler ####

 Medie        | Requests | Data   | Load-tid
:-------------|---------:|-------:|---------:
 DR           |      112 | 2,4 MB | 25,67 s
 TV 2         |      178 | 3,0 MB | 15,49 s
 Politiken    |      421 | 4,9 MB | 32,06 s
 Berlingske   |      181 | 2,0 MB | 23,40 s
 JP           |      111 | 1,1 MB | 15,19 s
 Børsen       |      152 | 2,5 MB | 24,80 s
 Information  |      154 | 2,9 MB | 24,03 s

 Medie        | Requests | Data       | Load-tid
:-------------|---------:|-----------:|---------:
 Hafnia Times |       16 | 264 **k**B | 2,71 s

#### Forskel Mellem Forside og Artikel ####

 Medie        | Requests | Data | Load-tid
:-------------|---------:|-----:|---------:
 DR           |      70% |  80% |      80%
 TV 2         |     180% | 150% |     340%
 Politiken    |     130% | 130% |     160%
 Berlingske   |     210% | 200% |     210%
 JP           |     150% | 250% |     200%
 Børsen       |     200% | 100% |     120%
 Information  |     130% | 180% |     180%

 Medie        | Requests | Data | Load-tid
:-------------|---------:|-----:|---------:
 Hafnia Times |     160% |  20% |     380%

Man kan eventuelt selv prøve at slå wifi fra på sin mobiltelefon og selv tilgå siderne med 3G-dækning for at se, hvordan oplevelsen er for mobile brugere. 4G/LTE er for hurtigt og EDGE for langsomt til at teste, men derfor kan man selvfølgelig alligevel prøve.

### Fortiden og Fremtidens Mediehjemmesider ###

Det er fristende at sortere rækkefølgen af resultaterne, men der er næppe nogen dukse i denne test. Der er ingen, er siger, at en side skal fylde en MB at hente---det kan fint opgøres i kB. I dette tilfælde er det bare nemmere at læse resultaterne i MB---når der nu alligevel ikke er nogen, der ligger under 1 MB.

Mange har prøvet at sidde i toget og forsøge at læse dagens nyheder på den sporadiske 3G-forbindelse, man lejlighedsvist kan tiltuske sig. Dårligt og dovent hjemmesidedesign gør det til et langtrukkent forløb for ikke at tale om et dyrt bekendtskab for folk med abonnementer, der giver et dataloft på 100 MB om måneden.

Der er flere elementer, der gør, at de fleste hjemmesider er så dårlige i dag:

1. Dårlig programmering og manglende optimering
2. Tabloidlayout
    - Billeder
3. Alt skal med og vises på én gang
4. Reklamer og tracking

#### Tabloidlayout ####

Der er ved at være nogle år, siden aviserne kapitulerede og gik over til det såkaldte tabloidformat. Det blev ikke sidste gang, idet der også skete en digital overgang til tabloidformatet, der bedst kan demonstreres ved tv2.dk's udvikling fra 2007 til 2013[^tv2-layouts]:

[^tv2-layouts]: Se flere websidelayouts i den mellemliggende periode for [2008][tv2dk-2008], [2010][tv2dk-2010], [2011][tv2dk-2011], [2012][tv2dk-2012].

[![tv2.dk's hjemmeside 1/7-2007][tv2dk-20070701-i]][tv2dk-20070701-u]

[![tv2.dk's hjemmeside 2/3-2013][tv2dk-20130302-i]][tv2dk-20130302-u]

(Sidste layout har langt flere billeder, hvis man bevæger sig længere ned på siden. Klik på billederne for at se det fulde oprindelige hjemmesidelayout.)

Layoutsene giver mindelser om **annoncemosaikken** i de gamle tabloidaviser, hvor alt er tilplastret med så meget indhold som muligt. Dertil kommer de store bogstaver, enorme billeder og skrigende farver, der kendes fra de såkaldte "kulørte" tabloidaviser og sladderblade.

tv2.dk har mere end nogen mediehjemmesider taget denne (anti-)æstetik til sig, så der tale om et mere ekstremt tilfælde, der hjælper med at påpege inspirationen.

En anden motivation for den generelle designomstilling blandt alle medier er en lille ting fra 2008 ved navn **iPhone**.

Al udvikling går så hurtigt, så det er svært at følge med, og alle nye opfindelser tages efterhånden for givet, men det er værd at huske på, at der var engang for ikke så længe siden, hvor det ikke var til at fatte, at størstedelen af fremtidens internettrafik ville komme udelukkende fra mobile computer, inklusive tablets.

Vi skal ikke længere tilbage end tre år til 2012, hvor Facebook [i deres børsnotering][facebook-s-1] skriver, at de vurderer deres største eksistentielle trussel til at være en manglende omstilling til mobile computere. *Facebook viste ikke engang reklamer på mobile computere før marts 2012.*[^facebook-mobile]

[^facebook-mobile]: Siden udgjorde reklamer på mobile enheder [90% af Facebooks vækst og pt. 72% af omsætningen][mobile-revenue].

Senere er mange gået over til en såkaldt <i>mobile first</i>-strategi, hvor man fokuserer på udvikling til mobile computere, fordi det simpelthen er der, størstedelen af trafikken kommer fra. Læg dertil at der findes folk---på verdensplan---der *udelukkende* anvender tjenester som Facebook via en mobil computer.

Med udgivelsen af iPhones og senere iPads måtte vi gentænke hele vores websidedesign, idet tastatur og mus var smidt ud til fordel for **<i>touch</i>-baseret navigation**. For at kunne navigere på en webside og interagere med links---og reklamer, forstås---måtte vi som det første sikre, at elementer var tilpas store nok til at pege på <i>(tappe)</i> uden at ramme noget forkert ved siden af. Desuden er der nogle, hvis syn ikke må siges at være godt nok til at kunne læse alt med småt.

Den *anden* konsekvens af udbredelsen af iPhones blev, at folk pludselig begyndte at **surfe mobilt** i et omfang, som det aldrig var set før. Og når man surfer fra en mobil, er forbindelsen væsentligt langsommere uden adgang til bredbåndwifi.

Desværre har mange kun omstillet sig til den *første* revolution.

##### Billeder #####

Webdesignere skulle nu omstille sig til en ny virkelighed, hvor brugere:

1. Anvender <i>touch</i>-baseret navigation.
2. Surfer fra mobilnetværk med langsomt net som EDGE og 3G.

For at brugere kunne mobiltappe på artikler uden at ramme ved siden af, blev mange sider inddelt i et kasselayout, hvor artiklerne blev repræsenteret af enorme billeder, der var umulige at tappe ved siden af. For eksempel ville det oprindelige tv2.dk-layout være svært at navigere på for mobile bruger grundet de små artikellinks.

Dette mosaiklayout, som danske tabloidmedier som eb.dk og bt.dk især tog til sig, medfører en *<i>touch</i>-konflikt*, idet siderne bruger flere og større billeder for at bistå <i>touch</i>-mobile brugere, på samme tid som de burde sikre, at deres sider indlæses så hurtigt som muligt på brugernes langsomme forbindelser.

Oven i hatten annoncerede Apple ved introduktionen af iPhone 4 deres [Retina][]-display, der betød en fordobling af skærmens pixeltæthed og derved et firdoblet pixel- og billedareal. Billeder, der hidtil havde været rettet imod almindelige skærme, tog sig nu grumsede ud på den nye iPhone, så nu var man nødt til at firdoble opløsningen på sine billeder for at imødekomme besøgende med en iPhone 4.

* * * *

Nye udfordringer skal imødekommes, men det må ske ved at favne dem uden betingelsesløst at stable flere og flere nye ting sammen på bekostning af den samlede oplevelse.

Fremtiden er ikke hestevogne med forbrændingsmotor.

* * * *

#### Reklamer og Tracking ####

Ved brug af [Lightbeam][] til Firefox kan man se hvor mange tredjepartssider, du indlæser ved at besøge en side. Hvis vi indlæser vores artikler igen:

 Medie                   | TPS
:------------------------|----:
 [DR][dr-json][^json]    | 14
 [TV 2][tv2-json]        | 35
 [Politiken][pol-json]   | 30
 [Berlingske][b-json]    | 25
 [JP][jp-json]           | 33
 [Børsen][boe-json]      | 38
 [Information][inf-json] | 30

[^json]: Du kan se den fulde liste med resultater ved at klikke på linksene i tabellen.

Her er et eksempel på tredjepartssiderne **(TPS)** i Politikens artikel:

![Visualisering af tredjepartsindlæsninger via Politikens artikel][tv2-viz]

Sidst, men ikke mindst:

 Medie        | TPS
:-------------|----:
 Hafnia Times | 2

Hvis du ikke er glad for at blive sporet, kan jeg anbefale følgende browserprogrammer, i prioriteret rækkefølge:

Mod trackere:

* [Privacy Badger][privacy-badger] (Chrome, Firefox)
* [Ghostery][]
* [Disconnect][]

Mod reklamer:

* uBlock ([Chrome][ub-c], [Safari][ub-s], [Firefox][ub-ffx])
* [Ad Muncher][ad-muncher] (Windows)

Lad være med at bruge AdBlock.

### Ad-blockerne Kommer ###

Afslutningsvist er det værd at påpege, at man i næste iOS 9-softwareopdatering til iPhones og iPads om et par uger kan installere en ad-blocker, som blokerer for tracking og reklamer. Du kan se [et videoeksempel her][ios-adblock-video].

Med udsigt til en mobil genvej til at indlæse artikler hurtigere og sikrere ved at gå uden om trackere og reklamer må medierne spørge sig selv, om de er skråsikre om en fremtid, hvor deres hjemmesider stadig er fyldt med billeder, reklamer og tracking, som skal tilgås fra en tarvelig 3G-forbindelse på mobilen i toget på vej til arbejde.[^battery]

[^battery]: Og så har vi ikke engang kigget på, hvordan de pågældende hjemmesider dræner mobilbatteriet.

Nogle vil undersøge muligheden for at gå appvejen, som Facebook med <i>Paper</i> og Apple med <i>News</i> prøver at presse medierne til. Men Internettet forsvinder ikke foreløbigt, og vi kommer ikke til at løbe fra, at mange finder deres læsning via sociale netværk med links til artiklerne på nettet---i stedet for en digital morgenavis.

Det er også værd at spørge, om betalende abonnenter skal døje med samme reklamer, tredjepartsindhold og tracking online som forbipasserende gratislæsere. Hvilken læseoplevelse har man krav på som læser? Og hvor meget kan medierne slippe afsted med, før tålmodigheden og tilliden er væk?

### Relateret Læsning ###

* ["The Verge's web sucks"][us-test]
* ["Medier blæser til kamp mod adblockers"][adblockers]
* ["The adblocking revolution is months away"][ios-adblock]
* [Hjemmesiders vækst i forhold til computerspil][doom]
* [Hjemmesidestørrelser med og uden adblockers][adblock-difference]
* <i>[Web Design: The First 100 Years][idle-words]</i>
* [Malvertising][]
* <i>New York Times</i>: ["Study of Ad-Blocking Software Suggests Wide Use"][nyt-adblocking]


[us-test]: http://blog.lmorchard.com/2015/07/22/the-verge-web-sucks/

[dr-f]: http://dr.dk
[dr-a]: http://www.dr.dk/nyheder/politik/sf-opraab-fra-f16-mekanikere-er-et-wake-call
[tv2-f]: http://tv2.dk
[tv2-a]: http://nyhederne.tv2.dk/2015-07-28-politiet-det-er-ikke-hver-dag-at-vi-finder-to-slanger
[pol-f]: http://pol.dk
[pol-a]: http://politiken.dk/indland/politik/ECE2772577/radikale-vil-fortsaette-kamp-mod-is-trods-slidte-fly-og-mekaniker-noedraab/
[b-f]: http://b.dk
[b-a]: http://m.b.dk/nationalt/f16-mekanikere-stop-fly-aktionen-mod-islamisk-stat
[jp-f]: http://jp.dk
[jp-a]: http://jyllands-posten.dk/international/europa/ECE7894151/Nato-bakker-Tyrkiet-op-i-kampen-mod-Islamisk-Stat/
[boe-f]: http://børsen.dk
[boe-a]: http://investor.borsen.dk/artikel/1/308123/usa_positive_amerikanske_aktier_efter_flotte_regnskaber.html
[inf-f]: http://information.dk
[inf-a]: http://www.information.dk/540474
[ht-f]: https://hafniatimes.com
[ht-a]: https://hafniatimes.com/articles/2014/09/14/danish-polls/

[tv2dk-20070701-u]: https://web.archive.org/web/20070701155638/http://tv2.dk/
[tv2dk-20070701-i]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/tv2dk-20070701.png
[tv2dk-20130302-u]: https://web.archive.org/web/20130302030436/http://tv2.dk/
[tv2dk-20130302-i]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/tv2dk-20130302.png
[tv2dk-2008]: https://web.archive.org/web/20080924024814/http://tv2.dk/
[tv2dk-2010]: https://web.archive.org/web/20100603031753/http://tv2.dk/
[tv2dk-2011]: https://web.archive.org/web/20110923163834/http://tv2.dk/
[tv2dk-2012]: https://web.archive.org/web/20121206074034/http://tv2.dk/

[facebook-s-1]: http://modrenman.com/2012/04/24/facebook-instagram-and-mobile
[mobile-revenue]: http://www.statista.com/chart/2496/facebook-revenue-by-segment/
[retina]: https://en.wikipedia.org/wiki/Retina_Display

[lightbeam]: https://www.mozilla.org/en-US/lightbeam/

[dr-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/dr.json
[tv2-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/tv2.json
[pol-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/pol.json
[b-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/b.json
[jp-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/jp.json
[boe-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/boe.json
[inf-json]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/inf.json
[tv2-viz]: /da/assets/fremtidens-og-fortidens-mediehjemmesider/pol.png

[privacy-badger]: https://www.eff.org/privacybadger
[ghostery]: https://www.ghostery.com/en/our-solutions/ghostery-add-on/
[disconnect]: https://disconnect.me/
[ub-c]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm
[ub-s]: https://www.ublock.org/
[ub-ffx]: https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/
[ad-muncher]: https://www.admuncher.com/

[ios-adblock-video]: https://theoverspill.wordpress.com/2015/07/30/the-adblocking-revolution-is-months-away-with-ios-9-with-trouble-for-advertisers-publishers-and-google/
[adblockers]: https://politiken.dk/kultur/medier/ECE2771183/medier-blaeser-til-kamp-mod-adblockers/
[ios-adblock]: https://theoverspill.wordpress.com/2015/07/30/the-adblocking-revolution-is-months-away-with-ios-9-with-trouble-for-advertisers-publishers-and-google/
[doom]: https://twitter.com/xbs/status/626781529054834688
[adblock-difference]: https://twitter.com/jbscript/status/624535428620791808/photo/1
[idle-words]: http://idlewords.com/talks/web_design_first_100_years.htm
[malvertising]: https://en.wikipedia.org/wiki/Malvertising
[nyt-adblocking]: http://bits.blogs.nytimes.com/2015/08/10/study-of-ad-blocking-software-suggests-wide-use
