# Välkommen till Flutter!

Det här är en **interaktiv** guide för dig som inte har någon tidigare erfarenhet av Flutter och är nyfiken på vad det är.

Varje steg har en besktivning på vänster sida och ett kodstycke på höger sida.<br/>En del steg kommer även ha en uppgift som du ska försöka lösa, men om du kör fast så finns en knapp för att visa lösningen.

## Vad är Flutter?
Flutter är en verktygslåda för att bygga gränssnitt för iOS, Android, Webb och Desktop. Allt med samma kodbas.

Vi skriver våra Flutter appar i Dart, ett programmeringspråk från Google.

## Vår första app
Till höger kan vi se en minimal Flutter app som vi ska gå igenom uppifrån och ner.

* Ska vi använda Flutter behöver vi importera något av Flutters bibliotek. Här väljer vi `material`, men det finns även `widgets` & `cupertino`

* Efter det startar appen med att köra `main()` och eftersom det här är en Flutter app så bygger vi vår första widget `MyApp` i `runApp()`

* Allt i Flutter är en `widget`. En widget kan vara allt ifrån väldigt komplicerad till väldigt enkel.<br/> När man skapar en widget så kan man antingen skapa en `Statelesswidget` eller en `Statefulwidget`, den senare kommer vi gå in på lite senare.<br/>
Varje widget har en `build` metod som kommer bygga innehållet i widgeten.<br/>
Eftersom `MyApp` är den widget som vi bygger först så låter vi den först bygga en `MaterialApp`. Den kommer ladda upp vår app med allt den behöver för att vara en app och det enda den behöver veta är vilken widget som kommer sen, här `home: MyFirstScreen()`.

* Nu börjar det roliga! Vi skapar vår första widget som kommer visas på skärmen. Vi kallar den `MyFirstScreen`.<br/>Eftersom den är först ut på skärmen använder vi först en `Scaffold` Widger. Den kommer skapa ett grundutseende för vår vy och skapar bland annat en vit bakgrund och ser till att kommande widgets får ett korrekt utseende.

* Det finns massa widgets att använda sig av. Alla med olika uppgifter och möjligheter. Vi vill visa en text på skärmen, så vi använder en `Text` widget och ger den en text att visa.<br/>
Jippie!!! Vi har nu text på skärmen! 🎉 🎉 🎉<br/>
Men texten är placerad längst upp till vänster och vi vill ju ha den i mitten.<br/>
Om skapar en `Center` widget innan vår text så lyckas vi med att placera texten mitt på skärmen.

### Snyggt jobbat!

Hur ser det ut då?

Under koden till höger så finns det en flik som heter `UI Output`.<br/>Öppna den och tryck på den blå knappen uppe till höger som säger `RUN`

Eftersom Flutter även kan köras på webben så kan vi här se resultatet av vår Flutter app!