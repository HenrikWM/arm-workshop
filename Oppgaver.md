# Oppgaver

Oppgavene er fordelt etter vanskelighetsgrad og det er ikke meningen å fullføre alle. På en 3-timers workshop burde man rekke 1-2 oppgaver, avhengig av tidligere erfaring. Plukk en oppgave som passer med ditt nivå og som vil lære mest av. Siste oppgave er fin hvis man vil ha en lang og komplett walkthough av å bruke ARM-templates.

Alle bør ha gjennomført minst en enkel oppgave
 for å teste at verktøy, Azure-konto og Azure SDKen du har virker. Feilsøking på enkle ARM-templates er n-ganger enklere enn på store templates.

## Vanskelighetsgrad: Enkel

### Publiser et Quickstart 101 prosjekt

Finn et 101-repo på https://github.com/Azure/azure-quickstart-templates og publiser det til Azure. Denne oppgaven gir deg en god innsikt i de grunnleggende begrepene i ARM-templates.

Gjør følgende:

1. Finn et 101-repo.
2. git clone ...
3. Les igjennom json-filene og sett deg inn i strukturen.
4. Klikk på **Deploy to Azure** knappen.
5. Fyll ut feltene. Legg merke til ledetekster, hjelpetekster og inputverdier. Gå tilbake til json-filene og finn ut hvor disse er definert.
6. Publiser og verifiser i Azure-portalen at tjenesten ble publisert.

Gratulerer med vel gjennomført! Du kan velge om du vil prøve deg på et 201- eller 301-prosjekt eller gå videre til en ny oppgave.

### Publiser en Resource Group med en ASP.net Web Application fra Visual Studio

Gå til https://azure.microsoft.com/en-us/documentation/articles/vs-azure-tools-resource-groups-deployment-projects-create-deploy/ og følg artikkelen som guider deg igjennom:

* Opprette en Resource Group i Visual Studio
* Legge til tjenester
* Publisere tjenestene til Azure.

Oppgaven gir deg innsikt i å bruke Visual Studio til å publisere en ARM-template som beskriver infrastrukturen for å kjøre en ASP.Net Web Application.

## Vanskelighetsgrad: Medium

### Publiser Azure Bootcamp 2016 oppgavene

I denne oppgaven skal du publisere tjenestene som dannet grunnlag for oppgaver til [Azure Bootcamp 2016]. Les prosjektets README-fil for å komme igang. Hvis du har brukt Visual Studio i andre oppgaver, prøv med Azure CLI / Powershell denne gangen.

### Eksporter din eksisterende Resource Group som ARM-template

Å eksportere eksisterende tjenester i ditt Azure-abonnement er en fin måte å bli kjent med hvordan ARM-templates virker og kan være et godt utgangspunkt for videre templatebygging.

Gå til [Export an Azure Resource Manager template from existing resources] for å lære hvordan du kan ta utgangspunkt i en allerede eksisterende tjeneste i ditt Azure-abonnement og eksportere ut en ARM-template. 

Gjør følgende:

1. Gå til artikkelen og les.
2. Finn en tjeneste du allerede har satt opp tidligere i Azure og bruk det du lærte i artikkelen til å eksportere ut tjenesten din som en ARM-template.
3. Rediger ARM-templaten og legg til en tjeneste, f.eks. Application Insights eller en Storage Account.
4. Test ARM-templaten hos [http://armviz.io/].
5. Når ARM-templaten er gyldig, bruk Azure CLI / Powershell til å publisere ARM-templaten.
6. Gå i portalen og verifiser at du ser den nye tjenesten og at alle tjenestene du beskrev i templaten er tilgjengelig.

## Vanskelighetsgrad: Utfordring

### Publiser ToDoApp

Gå til [Provision and deploy microservices predictably in Azure] og følg artikkelen. Oppgaven er ikke nødvendigvis vanskelig eller kompleks men noe tidkrevende. Du vil få en grundig gjennomgang av [ToDoApp]-prosjektet, publisering av ARM-templates via Visual Studio og publisering via Azure Powershell. 

Du får et glimrende utgangspukt for senere prosjekter ved å gjenbruke strukturen i ARM-templatene til [ToDoApp]-prosjektet.

### Template Functions

Ta utgangspunkt i en 101-web app fra [https://github.com/Azure/azure-quickstart-templates].

1. git clone ...
2. Legg til en SQL Azure Database tjeneste
3. Opprett en SQL-bruker med passord til din database
4. Bruk databasen i din web app.
5. Inject inn `connectionString` og SQL-brukernavn og -passord. Dette er secrets skal leses fra Azure KeyVault.

[Export an Azure Resource Manager template from existing resources]: <https://azure.microsoft.com/en-us/documentation/articles/resource-manager-export-template/>
[http://armviz.io/]: <http://armviz.io/>
[https://github.com/Azure/azure-quickstart-templates]: <https://github.com/Azure/azure-quickstart-templates>
[Azure Bootcamp 2016]: <https://github.com/HenrikWM/NNUG_GAB2016>
[Provision and deploy microservices predictably in Azure]: <https://azure.microsoft.com/en-gb/documentation/articles/app-service-deploy-complex-application-predictably/>
[ToDoApp]: <https://github.com/azure-appservice-samples/ToDoApp>
