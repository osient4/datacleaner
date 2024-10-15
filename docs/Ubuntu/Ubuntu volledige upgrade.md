# Ubuntu volledige update en upgrade (handmatig)

Zorg ervoor dat je Ubuntu-systeem altijd up-to-date is. In dit artikel bespreek ik kort de stappen om je systeem volledig te updaten, zodat je profiteert van de laatste beveiligingspatches en verbeteringen.

## TL;DR

- sudo apt-get update
- sudo apt-get upgrade -y 
- sudo apt-get dist-upgrade -y
- sudo apt-get autoremove -y 
- sudo apt-get autoclean -y

## Handmatige volledige upgrade in 5 stappen
### 1. sudo apt-get update
Dit commando ververst de lijst van beschikbare software en updates op je systeem. Het zorgt ervoor dat je computer weet wat de nieuwste versies zijn van de programma's die je via apt kunt installeren. Dit commando zelf installeert nog niets, het verzamelt alleen informatie.

### 2. sudo apt-get upgrade -y
Dit commando installeert de nieuwste versies van alle geïnstalleerde software op je systeem, zolang deze updates geen bestaande instellingen of andere softwarepakketten wijzigen. De -y zorgt ervoor dat je niet telkens op 'ja' hoeft te drukken om de updates te bevestigen.

### 3. sudo apt-get dist-upgrade -y
Dit commando doet hetzelfde als upgrade, maar het kan ook pakketten verwijderen of nieuwe pakketten installeren als dat nodig is om de updates te voltooien. Dit is nuttig bij grotere systeemupdates. De -y bevestigt wederom alles automatisch.

### 4. sudo apt-get autoremove -y
Hiermee worden overbodige softwarepakketten automatisch verwijderd, zoals oude afhankelijkheden die niet meer nodig zijn. Dit houdt het systeem schoon en bespaart ruimte.

### 5. sudo apt-get autoclean -y
Dit verwijdert gedownloade installatiebestanden van oude softwareversies die niet meer nodig zijn, waardoor je opslagruimte vrijmaakt.

## Aanbevolen routine
Het is aan te raden om wekelijks `sudo apt-get update` en `sudo apt-get upgrade -y` uit te voeren. Maandelijks kun je `sudo apt-get dist-upgrade -y`, `autoremove` en `autoclean` doen.

