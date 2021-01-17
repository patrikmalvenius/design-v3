---
Title: Designprojekt
Description: Rapport för kmom 10
Template: kmom
---

Design - Projekt
==================

Jag har gjort en sida åt min fru, som är designer. Kunden inom ramen för detta projekt är alltså Art Ist. Min fru behöver en sida som framför allt kan användas som referenssida, eller showroom, för de saker hon har gjort, varför fokus ligger på att dels visa ett print som "hero image" på startsidan, och dels bygga ett litet galleri med mer bilder i. Footern är instoppad i sidan, där loggan (som i detta fallet bara är min frus namn) och navigeringen håller footern sällskap. I footern finns endast det mest centrala, nämligen länkar till Instagram + en mail-knapp. När man klickar på galleri-bilderna kommer man till en gömd sida som innehåller bilden i originalstorlet. Där har min fru också möjlighet att skriva nåt om varje enskild bild. Det har hon dock inte gjort :(. Klickar man på den gömda undersidans bild kommer man tillbaka till samma div man klickade på i galleriet. Det är lite skit samma när man kollar på en bred skärm, men på mobilen, när listan blir lång och enfilig, kändes det viktigt.

Jag hade säkert kunnat lösa detta med de gömda undersidorna programmatiskt, vilket hade varit ca 10000% snyggare, men ibland går det fortare att köra copy-paste än att tänka. Tänker man på framtida underhåll av denna sidan hade det dock varit smart att bygga det lite käckare och intelligentare.

Temat är avskalat, men ändå genomtänkt för att synka med de färger som återfinns i bilderna. Tanken med temat är att det ska platsa på den tunna linjen mellan lekfullt och stilrent, för att på så sätt lyckas vara både och. Fokus på sidan ligger främst på bilderna, varför temat bara skall rama in och lyfta dessa, utan att göra för mycket väsen av sig. Sidan behöver inte särskilt mycket lull-lull för att funka. Därför är bara det nödvändigaste där. Jag har dock valt att tydligt separera navigation/kontakt från resten av sidan, för att göra det enkelt för användaren att både navigera och kontakta min fru.

Det viktigaste på sidan är själva galleriet. Jag ville gärna få till en struktur för detta där bilderna kunde vara olika långa men ändå ligga i ett grid. Det hade säkert gått att lösa detta med en grid också, men det kändes mest intuitivt att lösa det med nästlade flexboxar, både vertikala och horistonella. Utöver denna basdesign innehåller css också media queries, dels för att fälla ihop navigeringen, och dels för att trycka ihop sidofältet. Galleriet blir "enfiligt" helt automatiskt. Jag hade dock kunnat lägga lite mer tid på att få bilderna att skala i fler nivåer beroende på skärmbredd. Som det är nu är det två nivåer, vilket gör att det blir OK på den dator jag testat, samt i "virtuellt iPad-läge", men på en mobil blir bilderna lite onödigt smala i galleriet. Jag har också kört lite cimage och srcset, dels för att skala ner jpeg-bilderna i galleriet med cimage, och dels för att klippa bilderna i olika bredd beroende på skärmbredd. Fonten blev en "Poppins", som kändes lite stram men ändå lite kul.

Tillgängligheten har jag försökt tänka på genom att ha tillräcklig kontrast samt stoppa in maskinläsbar text i alla länkar och visuella element.

Jag började bygga denna sida baserat på min portfolio, pga kändes enklast. Det var dock också lärorikt att dekonstruera den CSS som låg till grund för portfolion, så av den anledningen kan jag tycka att det var ett bra val. Jag kan väl också konstatera att det jag lämnat in nu innehåller ett par onödiga filer, som ni hade sluppit om jag gjort allt från scratch, så ur den synvinkeln kan man säga att det var ett dåligt val. Det viktigaste här är väl dock min läroresa, så med det i bakhuvudet kan vi konstatera att det allt som allt var ett bra val!

Jag tycker att denna kursen varit rolig, trots att man var tvungen att skriva analyser. Det roligaste är att jag känner att jag börjar få lite grepp om CSS, äntligen. Vad gäller design i övrigt har vi dock sedan länge en uppdelning hemma hos oss där min fru står för det mesta av den biten. Projektet var precis lagom utmanande. Jag lärde mig en hel del på det, samtidigt som det inte åt upp vare sig mitt, min fru eller mina barns liv. Det lämnar ju också utrymme för mer ambitiösa studenter att jobba ännu mer, med de valfria uppgifterna som jag valt att inte göra. Det är också så, som jag nog skrivit nåt om i alla mina kurser hos er, att det är bra att återvända till saker man gjort innan, fast i en lite annan kontext, så att man utmanas at verkligen tänka efter och förstå vad man gjort tidigare för att kunna utnyttja det till att göra något nytt.

Bra också att ni introducerat Git. Tack.

Tack för en fin kurs!

Patrik
