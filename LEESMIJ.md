# Urenregistratie — Android-app

Dit is de complete broncode van de app "Uren". Hij werkt volledig offline. Je klanten en uren worden op je telefoon bewaard.

Je hebt geen programmeerkennis nodig om er een installeerbare app (.apk) van te maken. Kies één van de twee manieren hieronder.

---

## Manier 1: GitHub bouwt de app voor je (gratis, niets installeren)

1. Maak een gratis account op github.com en log in.
2. Klik rechtsboven op **+** en kies **New repository**. Geef hem een naam, bijvoorbeeld `uren-app`. Kies **Private** en klik op **Create repository**.
3. Klik op de link **uploading an existing file**.
4. Pak het zip-bestand uit op je computer. Sleep **de inhoud** van de map `Urenregistratie-android` (dus de mappen `app`, `.github` en de losse bestanden) naar het uploadvak. Klik op **Commit changes**.
5. Open het tabblad **Actions**. Daar start automatisch "Android-app bouwen". Na 3 tot 5 minuten krijgt hij een groen vinkje.
6. Klik op die bouw. Onderaan staat onder **Artifacts** het bestand **Urenregistratie-apk**. Download het en pak het uit: daarin zit `app-debug.apk`.

**Geen bouw te zien bij Actions?** Dan is de verborgen map `.github` niet meegekomen. Dat gebeurt vaak, omdat mappen die met een punt beginnen verborgen zijn. Los het zo op: klik bij Actions op **set up a workflow yourself**. Plak de inhoud van het bestand `.github/workflows/build-apk.yml` en klik op **Commit changes**.

## Manier 2: Android Studio (als je dat al hebt)

1. Open Android Studio, kies **Open** en selecteer de map `Urenregistratie-android`.
2. Wacht tot het project is ingeladen (de eerste keer duurt dat even).
3. Kies in het menu **Build → Build App Bundle(s) / APK(s) → Build APK(s)**.
4. Klik in de melding op **locate**. Daar staat `app-debug.apk`.

---

## Installeren op je telefoon

1. Zet `app-debug.apk` op je telefoon, bijvoorbeeld via Google Drive, een mail aan jezelf of een USB-kabel.
2. Tik op het bestand. Android vraagt of je apps uit deze bron wilt toestaan. Sta het toe voor die app (bijvoorbeeld Bestanden of Drive).
3. Tik op **Installeren**. De app "Uren" staat daarna tussen je apps.

Play Protect kan waarschuwen dat de app onbekend is. Dat komt doordat hij niet uit de Play Store komt. Kies **Toch installeren**.

## Goed om te weten

- **Je gegevens staan alleen op deze telefoon.** Ze worden niet gedeeld met de webversie in Claude. Gebruik dus één van de twee als je vaste plek.
- **Verwijder je de app, dan zijn je gegevens weg.** Exporteer daarom regelmatig je overzicht via **Overzicht → Exporteer (CSV)**. Je kunt het bestand dan mailen, in Drive zetten of via WhatsApp versturen.
- Bij een **nieuwe versie** installeer je de nieuwe .apk gewoon over de oude heen. Je gegevens blijven dan bewaard, mits de nieuwe versie met dezelfde computer of dezelfde GitHub-repository is gebouwd.
- De terugknop van je telefoon sluit eerst een open formulier en gaat daarna terug naar het weekoverzicht.
