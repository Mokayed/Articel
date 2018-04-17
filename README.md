# Articel
Googlemap with Android/Java
Google Maps i Android
Introduktion
Jeg vil snakke om hvordan man kan bruge google maps i android and garneret en google map api, med 7 trins som man kan får google map på din mobile Application.9
Man bruge google maps til mange forskelle ting (Navigation, får en location, din location,etc…

-Trin 1
 
 Installer SDK for Google Play-tjenester
Tilføj Google Play-tjenester til Android Studio.


-Trin 2
 Opret et Google Maps-projekt
 
Følg disse trin for at oprette et nyt app-projekt, herunder en kortaktivitet:
Start Android Studio.
Opret et nyt projekt som følger:

Hvis du ser dialogen Velkommen til Android Studio, skal du vælge Start et nyt Android Studio-projekt, der er tilgængeligt under 'Hurtigt start' til højre for dialogboksen.
Ellers skal du klikke på Filer i menulinjen i Android Studio og derefter på Ny, nyt projekt.
Indtast dit appnavn, firma domæne og projekt placering, som bedt om det. Klik derefter på Næste.

Vælg de formfaktorer, du har brug for til din app. Hvis du ikke er sikker på hvad du har brug for, skal du bare vælge Telefon og tablet. Klik derefter på Næste.
Vælg Google Maps Aktivitet i dialogboksen "Tilføj en aktivitet til mobil". Klik derefter på Næste.
Indtast aktivitetsnavnet, layoutnavnet og titlen som bedt om det. Standardværdierne er fine. Klik derefter på Udfør.
Android Studio starter Gradle og bygger dit projekt. Det kan tage et par sekunder. Yderligere oplysninger om oprettelse af et projekt i Android Studio finder du i dokumentationen til Android Studio.

Når bygningen er færdig åbner Android Studio google_maps_api.xml og MapsActivity.java-filer i editoren. (Bemærk, at din aktivitet kan have et andet navn, men det er det, du konfigurerede under opsætningen.) Bemærk, at filen google_maps_api.xml indeholder instruktioner om at få en Google Maps API-nøgle, før du forsøger at køre programmet. Det næste afsnit beskriver, hvordan du får API-nøglen mere detaljeret.

-Trin 3.
 Få en Google Maps API-nøgle
 
Din ansøgning har brug for en API-nøgle for at få adgang til Google Maps-serverne. Den type nøgle, du har brug for, er en API-nøgle med begrænsning for Android-apps. Nøglen er gratis. Du kan bruge det med alle dine programmer, der kalder Google Maps Android API, og det understøtter et ubegrænset antal brugere.

Vælg en af følgende måder at få din API-nøgle fra Android Studio:

Den hurtige og nemme måde: Brug linket i den google_maps_api.xml-fil, som Android Studio har oprettet til dig:
Kopier linket i filen google_maps_api.xml og indsæt det i din browser. Linket fører dig til Google API-konsollen og leverer de nødvendige oplysninger til Google API-konsollen via URL-parametre, hvilket reducerer den manuelle indgang, der kræves af dig.
Følg vejledningen for at oprette et nyt projekt i Google API-konsollen eller vælg et eksisterende projekt.
Opret en Android-begrænset API-nøgle til dit projekt.
Kopier den resulterende API-nøgle, gå tilbage til Android Studio, og indsæt API-nøglen i elementet <string> i filen google_maps_api.xml.
En lidt mindre hurtig måde: Brug legitimationsoplysningerne i den google_maps_api.xml-fil, som Android Studio har oprettet til dig:
Kopier de legitimationsoplysninger, der er angivet i filen google_maps_api.xml.
Gå til Google API Console i din browser.
Brug de kopierede legitimationsoplysninger til at tilføje din app til en eksisterende API-nøgle eller for at oprette en ny API-nøgle.
 (https://console.developers.google.com/apis/dashboard?project=reflected-song-186909&duration=PT1H)
Den fulde proces til at få en API-nøgle: Hvis ingen af ovenstående valgmuligheder virker for din situation, skal du følge hele processen.












Trin 4.
 Tag kig på koden
Undersøg koden, der leveres af skabelonen. Se især på følgende filer i dit Android Studio-projekt.

XML layoutfilen
Som standard er XML-filen, der definerer appens layout, reset / layout / activity_maps.xml. Den indeholder følgende kode:
 

Kortaktiviteten Java-filen
Java-filen, der definerer kortaktiviteten, er som standard navngivet MapsActivity.java. Det skal indeholde følgende kode efter dit pakkenavn:
 
-Trin 5
Til Slut en Android-enhed
Den enkleste måde at se din app på, er at slutte en Android-enhed til din computer. Følg vejledningen for at aktivere udviklerindstillinger på din Android-enhed og konfigurér din applikation og system for at registrere enheden.

Alternativt kan du bruge Android-emulatoren til at køre din app. Brug Android Virtual Device (AVD) Manager til at konfigurere en eller flere virtuelle enheder, som du kan bruge sammen med Android-emulatoren, når du opbygger og kører din app. Når du vælger din emulator, skal du sørge for, at du bruger Android 4.2.2 eller nyere, og pas på at vælge et billede, der indeholder Googles API'er, eller programmet har ikke de nødvendige runtime-API'er for at kunne udføres. Bemærk også instruktionerne til konfiguration af virtuel maskinacceleration, som du skal bruge med en x86-mål-AVD som beskrevet i vejledningen. Dette vil forbedre din oplevelse med emulatoren.





Trin 7.
Build og kør din app
I Android Studio skal du klikke på menuen Kør menuen (eller ikonet for afspilningsknappen) for at køre din app.

Når du bliver bedt om at vælge en enhed, skal du vælge en af følgende muligheder:

Vælg den Android-enhed, der er sluttet til din computer.
Alternativt skal du vælge knappen Start emulator og vælge den virtuelle enhed, som du tidligere har konfigureret.
Klik på OK. Android Studio vil påberåbe Gradle til at opbygge din app, og derefter vise resultaterne på enheden eller på emulatoren. Det kan tage et par minutter, før appen åbnes.

Du skal se et kort med en markør placeret over Sydney, Australien. Hvis du ikke kan se et kort, skal du bekræfte, at du har gennemført alle de trin, der er beskrevet på denne side. Kontroller især, at du har tilføjet en API-nøgle som beskrevet ovenfor.

Konklusion
De trin har jeg selv brugt og jeg synes det gik meget fint og jeg fik google map på min telefone.
Dvs. det gik meget godt og jeg fik det jeg har forventet, jeg vil også anbefale at går efter de trin hvis man skal bruge google map på din application for første gang.
