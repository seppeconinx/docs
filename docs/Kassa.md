# Kassa
[azure](https://dev.azure.com/anyvent/Kassa)

#### [Odoo](https://www.odoo.com) is een business management software-packet met alle nodige modules om een bedrijf te kunnen beheren.

Wij gebruiken enkel de module Point-of-Sales voor onze applicatie en hosten deze in een docker container op een ubuntu VM.

## Talen
- Python
- Javascript

## Database
PostgreSQL

### Toegang tot de database met [pgadmin](10.3.56.5:5050/browser/)
- 10.3.56.5:5050/browser/
- Username: `pgadmin4@pgadmin.org`
- Wachtwoord: `admin`

### Toegang tot [Odoo](http://10.3.56.5:8071/web/login) webinterface
- http://10.3.56.5:8071/web/login
- Username: `ehb@ehb`
- Wachtwoord: `ehb`

Toegang tot Odoo VM
ssh anyvent@10.3.56.5
Wachtwoord: `waterval`

[Github](https://github.com/Ashot-ton/anyvent-kassa): https://github.com/Ashot-ton/anyvent-kassa

### Data nodig voor aanmaak Kassa

#### Bedrijf
- Btwnummer
- Naam

#### Users (toegang tot kassa):
- Email
- Voornaam
- Achternaam
- Wachtwoord


#### Producten (beschikbare producten op event)
- Prijs
- ProductId

#### Bezoekers:
- Voornaam
- Achternaam
- Adres(straat, plaats, postcode, land)
- Email
- Telefoon
- Bedrijf
