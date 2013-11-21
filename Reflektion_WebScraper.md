# Reflektioner

1.  Jag hade tröttnat på att skriva i PHP, och har länge varit sugen på att
    lära mig Python, så jag gav mig på att skriva en Django app. Jag trodde också
    att Python skulle vara ett lämpligt språk att skriva ett sådant här skript
    i och där hade jag rätt! Det var dock lite jobbigt att inte riktigt känna
    sig hemma med grundläggande språkfunktioner från början, men det föll på
    plats utan större hinder.

2.  Små ändringar hos sidan man skrapar kan ge förödande konsekvenser på ens
    applikation, HTML är ett väldigt löst format.

    Vad som är lagligt/etiskt att skrapa kan vara otydligt.

    Om man skickar för täta requests så riskerar man att bli bannad.

3.  Jag ser inga särskilda problem med att skrapa en sida gjord i ASP.NET WebForms,
    dock har jag inte testat. Eftersom man i princip endast handskas med HTML
    så har serverside-tekniker liten inverkan.

    _Efter diskussion_: Man behöver ta hänsyn till ViewState, eventuella klasser
    som ASP.NET får för sig att ändra på osv...

4.  Jag har lagt in en delay i min `get_html()` så att requests inte skickas
    för tätt till servern.

    _Efter diskussion_: Man ska ta hänsyn till `robots.txt` (om den funnits),
    och även vara öppen med att man skrapar genom att sätta sin `useragent` till
    något lämpligt, och hänvisa till sin epost.

5.  Mot förmodan: Att koda i **Python** och en hel del om **Django**. Jag har också lärt
    mig att HTML är ett väldigt löst format som egentligen inte är lämpat att
    användas på det här sättet, koden blir lätt full av fulhack.

    Väldigt rolig uppgift, och ett nyttigt verktyg att kunna använda, dock känns
    det mer som något man kommer använda för eget bruk, skriptet blir lätt ganska
    känsligt för förändring, och man hade fått lägga ner bra mycket mer arbete
    för att rusta programmet för det.

    Många moderna företag som idag _vill_ att man ska dra nytta av deras data
    brukar istället ha ett publikt API.
