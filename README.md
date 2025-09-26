# Oppgave: Containerisering av en Spring Boot-applikasjon med Docker

**Mål:** Opprett en enkel Spring Boot-applikasjon, pakk den i et Docker-image, og kjør den i en container.
**Tid:** ca. 20 minutter
**Arbeidssted:** Din egen maskin eller i et CloudShell-miljø

---

## Trinn 1 – Lag applikasjonen

* Bruk [Spring Initializr](https://start.spring.io/) til å generere et prosjekt.
* Ta med minst én avhengighet (for eksempel *Spring Web*).
* Last ned prosjektet og bygg applikasjonen slik at du får en kjørbar `.jar`-fil.

---

## Trinn 2 – Opprett en Dockerfile

* Lag en fil kalt **Dockerfile** i prosjektmappen.
* Velg et passende base-image (f.eks. en lettvekts OpenJDK).
* Forslag: Bruk en "Multi stage" dockerfil som også kompilerer koden
* Husk Entrypoint - hvordan applikasjonen skal startes når containeren kjører.


## Trinn 3 – Bygg Docker-imaget

* Bruk Docker CLI til å bygge et image basert på Dockerfile-en din.
* Gi imaget et navn du selv velger.

## Trinn 4 – Kjør applikasjonen i en container

* Start en container basert på imaget du har laget.
* Eksponer porten applikasjonen kjører på, og sjekk at applikasjonen fungerer.

💡 **Tips:**

* Hold Dockerfile enkel.
* Diskuter med sidemannen før du ber om hjelp.

---

## 📄 Cheat Sheet

### Vanlige Docker-kommandoer

**Bygg image fra Dockerfile:**

```bash
docker build -t <image-navn> .
```

**Se hvilke images du har:**

```bash
docker images
```

**Kjør en container fra et image:**

```bash
docker run -p <lokal-port>:<container-port> <image-navn>
```

**Se hvilke containere som kjører:**

```bash
docker ps
```

**Stoppe en container:**

```bash
docker stop <container-id>
```

**Slette en container:**

```bash
docker rm <container-id>
```

**Slette et image:**

```bash
docker rmi <image-id>
```

# Bonus 

* Lag en multi-stage dockerfile 
