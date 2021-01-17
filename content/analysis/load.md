Laddtid
=======================

I denna uppgift skall jag studera och analysera tre olika webbplatser med avseende på färgval och typografi, samt diskutera huruvida dessa designkomponenter stödjer webbplatsens idé på ett bra sätt.

Urval
-----------------------

Jag valde samma tre miljöorganisationers (svenska) hemsidor - WWF, Jordens Vänner, och Naturskyddsföreningen - som i förra uppgiften. Laddtid och prestanda är ju precis som färg intressant i kommunikationssammanhang varför jag tycker att detta urval passar även här.

Metod
-----------------------

Jag använde Googla Pagespeed Insights och Network-fliken i DevTools i Chrome för att analysera tre sidor på dessa webbplatser (se sheet länkat längst ner för mer info)

Resultat
-----------------------

NATURSKYDDSFÖRENINGEN

Naturskyddsföreningens sidor får dåliga poäng i Pagespeed, speciellt på mobilsidan (som belastas av redirects i större utsträckning än desktop-versionen). Sidorna läses in på 3-7 sekunder. Det som framför allt kan göras för att snabba på inläsningen är:

* Minska serverns första svarstid. Jag är dock osäker på vad Pagespeed menar med detta.
* Lägga viktig javascript/CSS inline istället för separat, läsa in sånt som inte kan ligga inline asynkront
* Byta ut JPEG-bilder mot JPEG2000


<br/>
<br/>
![SNF](%assets_url%/img/snf.PNG){.me_start}

WWF

WWF:s sidor får dåliga poäng i Pagespeed, speciellt på mobilsidan. Sidorna läses in på ca 3 sekunder. WWF har dock lite andra problem än Naturskyddsföreningen, vilket är roligt. Förslag på förbättringar:

* Läs in fonten i förväg (via link rel=preload)
* Ta bort javascript som inte används
* Förminska bilderna - de är onödigt stora


<br/>
<br/>
![WWF](%assets_url%/img/wwf.PNG){.me_start}

JORDENS VÄNNER

Jordens Vänner kniper tveklöst jumboplatsen i denna granskning, med usla poäng i Pagespeed och vedervärdiga laddtider. Sidorna läses in på 6-25 sekunder, och på ett sådant sätt att jag som människa reagerar över långsamheten. Saker Jordens Vänner kan göra för att styra upp sin sida:

* Minska serverns första svarstid
* Lägga viktig javascript/CSS inline istället för separat, läsa in sånt som inte kan ligga inline asynkront
* Ta bort javascript som inte används


<br/>
<br/>
![JV](%assets_url%/img/jv.PNG){.me_start}

Analys
-----------------------

De vanligaste problemen i mitt urval av sidor verkar vara att man inte tänkt på laddtid när man byggt sidan. Jag misstänker att alla sidor baseras på nåt CMS i grunden, som sen har anpassats av någon för att få rätt look and feel. Förmodligen har man dock inte rensat ut allt gammalt bös från grund-CMS som inte används i den operationen. Sen har sidorna massa olika spårare, mätare och integrationskod som säkert gör nytta ibland, men ibland bara ligger och skvalpar, och detta tar också mycket resurser. 
<br/>
<br/>
Det här med att lägga css och js inline tror jag inte i praktiken är möjligt för denna typ av sidor, då de som sagt bygger på CMS som, för att funka vettigt, har en modulär uppbyggnad. Men att åtminstone se över storleken på sina bilder är inte för mycket begärt.
<br/>
<br/>
Alla sidor har usla laddtider om man frågar Google, men jag tyckte ändå SNF och WWF var helt ok. Helst hade jag dock sett laddtider som ligger närmare 1 s än 2-3 s, där lägger jag min gräns.
<br/>
<br/>
Jag utser Naturskyddsföreningen till vinnare i detta test, tätt följt av WWF. På jumboplats sätter jag Jordens Vänner som faktiskt behöver skärpa sig. Som användare av deras sida blir jag lite orolig för vad det är för skit som ligger inbäddad där.

Referenser och länkar
-----------------------

https://www.naturskyddsforeningen.se/

https://www.wwf.se/

https://jordensvanner.se/

Google Sheet:

https://docs.google.com/spreadsheets/d/1NMau5KTqGkT_X9Y9PmeuNHFBYAv9SHHPiENwR_VgLss/edit?usp=sharing


Övrigt
-----------------------

Patrik Malvenius tyckte och skrev detta.