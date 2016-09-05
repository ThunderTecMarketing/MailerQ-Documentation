Als je e-mails verstuurt, wil je natuurlijk wel dat deze allemaal worden
afgeleverd, en niet ergens in een spambox eindigen. Copernica biedt een
groot aantal hulpmiddelen om de afleverkwaliteit te optimaliseren. Ook
vind je hier algemene tips voor het verbeteren van je deliverability.

1. E-mail authenticatie {#1.-e-mail-authenticatie}
-----------------------

Om de niet-aflatende stroom van spamberichten te kunnen onderscheiden
van bonafiede e-mails hebben grote e-mail service providers (ESP's),
waaronder Google, Microsoft en Yahoo technische hulpmiddelen ontwikkeld
waarmee jij je kunt identificeren als een betrouwbare verzender.

### DKIM (DomainKey Identified Mail) {#dkim-(domainkey-identified-mail)}

DKIM staat voor DomainKey Identified Mail en is een stukje code in de
DNS. Hiermee zet je een unieke digitale handtekening in de header van je
e-mail die jou bestempelt als veilige afzender. Ontvangende mailservers
zien of de e-mail echt door jou is verstuurd en niet vervalst of
geforward door een andere partij. 

-   [E-mails versleutelen met
    DKIM](https://www.copernica.com/nl/blog/e-mails-versleutelen-met-dkim)

### SPF1

Je gebruikt je eigen domein als afzenderadres voor je bulkmailings. De
mails worden echter door onze mailsender verstuurd. SPF1 controleert of
het onzichtbare afzenderadres (envelope adress) gebruikt mag worden om
emails te versturen vanaf jouw domein. Als je dus Copernica toevoegt aan
je spf record, weet de ontvangende partij dat jouw mail verstuurd is
door een andere partij die daar toestemming voor heeft. Je hoeft SPF1
alleen in te stellen als je gebruik wilt maken van een eigen envelope
adres. Bij de meeste gebruikers is dit **niet** het geval, en staat de
SPF automatisch goed ingesteld.

-   [Eigen envelope domein gebruiken en instellen SPF voor dit
    domein](https://www.copernica.com/nl/blog/eigen-envelope-domein-gebruiken-en-instellen-spf-voor-dit-domein)

### Versterk je e-mail authenticatie verder met DMARC

DMARC is een policy die je kunt opnemen in het [DNS
record](https://en.wikipedia.org/wiki/Domain_Name_System) van het
afzenderdomein van je e-mails. Met deze policy geef je bij de
ontvangende mailboxprovider aan dat je SPF en/of DKIM gebruikt. Maar wat
DMARC vooral krachtig maakt, is het feit dat het aangeeft wat de
ontvanger moet doen met e-mail die niet door de SPF- of DKIM-test komt.
Het is zelfs mogelijk om dagelijks rapportages te ontvangen van ESP's
over de e-mails die wegens een niet-geaccepteerde DKIM en/of SPF zijn
geweigerd.

-   [Zorg dat je e-mails niet in de spambox terecht komen met
    DMARC!](https://www.copernica.com/nl/blog/zorg-dat-je-e-mails-niet-in-de-spambox-terecht-komen-met-dmarc)
-   [Bij de bron zelf: dmarc.org](https://dmarc.org/)
-   [Google handleiding voor het opmaken van een DMARC entry in je
    DNS](https://support.google.com/a/answer/2466563?hl=en)

2. Optimaliseer je database {#2.-optimaliseer-je-database}
---------------------------

ESP's houden er niet van als je e-mails blijft sturen naar adressen
onder hun domein die niet meer bestaan, zich hebben afgemeld of
resulteren in bepaalde foutmeldingen.

### Maak gebruik van dubbele optin

Een dubbele opt-in geeft je de garantie dat aanmelders zichzelf
daadwerkelijk hebben aangemeld en met een bestaand e-mailadres. Je
database blijft dus schoon van grappenmakers die een niet-bestaand
e-mailadres of dat van een ander invullen.

-   [Nieuwbriefinschrijvingen laten verlopen via dubbele
    optin](https://www.copernica.com/nl/blog/single-opt-in-of-double-opt-in-wat-is-het-en-hoe-werkt-het)

Houd je database schoon, verwerk bounces Het kan altijd gebeuren dat een
e-mailadres wordt opgeheven, of om een andere reden ophoudt te bestaan.
Wanneer een afleverpoging resulteert in een foutmelding, wordt dit voor
jou door Copernica geregistreerd. Hierop kan je selecties maken en
verdere actie ondernemen.

-   [Automatisch verwerken van e-mail
    bounces](https://www.copernica.com/nl/blog/automatisch-verwerken-bounces)

3. Optimaliseer je e-maildocumenten {#3.-optimaliseer-je-e-maildocumenten}
-----------------------------------

Iedereen die wel eens spam heeft ontvangen weet dat spam meestal ook de
uiterlijke en inhoudelijke kenmerken hiervan heeft. Copernica beschikt
over een aantal tools om jouw document te controleren op spamgevoelige
materie en eigenschappen. - Document controleren op spamgevoeligheid

-   [Verlaag je spamrating: enkele
    aandachtspunten](https://www.copernica.com/nl/blog/verlaag-je-spamrating-enkele-aandachtspunten)
-   [Veelvoorkomende HTML-fouten
    oplossen](https://www.copernica.com/nl/blog/veelvoorkomende-html-fouten)

4. Ontvangers kunnen zich uitschrijven {#4.-ontvangers-kunnen-zich-uitschrijven}
--------------------------------------

Je bent volgens Nederlandse wet verplicht een duidelijke
afmeldmogelijkheid te bieden bij elke bulkmailing die je verzendt.
Copernica biedt verschillende methodes aan om zo'n uitschrijving te
faciliteren.

-   [Afmeldingen automatisch
    verwerken](https://www.copernica.com/nl/blog/afmeldingen-automatisch-verwerken)

5. Controleer alles nog eens voordat je een bulkmailing verstuurt {#5.-controleer-alles-nog-eens-voordat-je-een-bulkmailing-verstuurt}
-----------------------------------------------------------------

Staat alles goed ingesteld? Is er geen hoge spamscore? Copernica loopt
vlak voordat je een document gaat versturen alles nog even na. Mocht je
onverhoopt een melding krijgen, dan vind je hier mogelijk de oplossing.

-   [Extra controles voor het versturen van een
    bulkmailing](https://www.copernica.com/nl/blog/extra-controles-voor-het-versturen-van-een-bulkmailing)
