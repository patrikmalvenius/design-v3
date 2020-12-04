---
Title: Kmom 2
Description: Rapport för kmom 2
Template: kmom
---

Kmom 2
==================

SASS känns ganska lätt att komma in i, och jag tror att när jag väl får ordentlig kläm på CSS kommer jag kunna ha nytta av att preprocessa stilar. Just nu är det dock fortfarande CSS som känns omfattande att greppa, SASS känns väldigt enkelt jämförelsevis.

Jag har grejat lite med Node och npm tidigare, när jag testat att installera Hajk (https://github.com/hajkmap/Hajk), en plattform för kommunalt GIS byggt på öppen källkod. Men då var det i princip bara copy paste av nån annans förslag på kommandon. Vilket det väl iofs har varit i detta kmom också :).

Komplieringen gick bra, förutom första gången då det inte gick bra. Tror det beror på att jag precis hade installerat lite grejer men inte startat om cygwin. 

Mitt tema är väldigt basalt, vilket mest beror på att jag inte riktigt vet vart denna kurs tar vägen och därför inte har någon klar bild av hur en design som bäst motsvarar slutproduktens krav ser ut. Har därför i princp kopierat det tema som jag gjorde i förra kmomet, vilket i sin tur är tungt inspirerat av dbwebb- och aurora-temana i sin grundkonstruktion. Det jag ändrat lite är flashbilden och färger, samt lagt till lite mer stilregler för små skärmar. 

All min SCSS-kod ligger i inkluderade filer i "shared". Olika filer beroende på om det är övergripande layout, navbar, variabler. Men längre fram kanske jag får tillfälle att lägga verkliga grundkomponenter i stilen i "shared", och temaspecifika stilregler i style.scss. Som det är upplagt nu delar ju alla teman som hämtar stil från shared på samma stil. 

Min TIL från detta kmom är att SCSS är enkelt. CSS är svårt.

