#Oppgave: Containerisering av en Spring Boot-applikasjon med Docker

## Mål:
Lag en Docker-fil som containeriserer en enkel Spring Boot-applikasjon, opprettet ved hjelp av Spring Initializr.

##Beskrivelse:
Du har 20 minutter på deg til å containerisere en Spring Boot-applikasjon som du vil opprette ved hjelp av Spring Initializr og deretter pakke den som et Docker-image. Følg trinnene nedenfor for å fullføre oppgaven:

##Trinn 1: Opprett Spring Boot-applikasjon med Spring Initializr
Bruk Spring Initializr (https://start.spring.io/) til å opprette en enkel Spring Boot-applikasjon. Velg en passende konfigurasjon og avhengigheter for din applikasjon. Last ned prosjektfilen når du er ferdig.

##Trinn 2: Lag en Docker-fil
Opprett en Docker-fil som beskriver hvordan Spring Boot-applikasjonen skal pakkes inn i en Docker-container. Du må velge et passende baseimage og inkludere alle nødvendige trinn for å kopiere og kjøre applikasjonen i containeren.

##Trinn 3: Bygg Docker-image
Bruk Docker CLI til å bygge Docker-imaget basert på Docker-filen du har opprettet. Sørg for at byggeprosessen går knirkefritt uten feil.

##Trinn 4: Kjør Docker-containeren
Start Docker-containeren basert på det opprettede Docker-imaget. Sjekk at Spring Boot-applikasjonen kjører som forventet i containermiljø