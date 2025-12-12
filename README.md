# Grupp 3

Arash, Simon N, Anette, Kasper, Andreas H, Martin E, Christoffer.

---

Vi har ändrat i en YAML-fil, deployment/backend.yaml. Det vi ändrade var storage till lvms-vg1. Vi fick göra det eftersom vår förra storage class inte kunde binda. Vi behöver endast köra oc apply på den fil vi ändrat.

Vi har skapat en action secret i GitHub som är för workflow-filen. I vår build and deploy-fil pekar vi på dessa secrets för autentisering. Genom att göra detta blir våra containers privata.

Eftersom vi hade gjort vår Guestbook i Red Hat Sandbox-miljön var vårt första steg att skapa Guestbooken i din labbmiljö, du (Jonas). Efter att vi har konfigurerat detta och skrivit klart vår workflow-fil kommer vi att testa att det fungerar genom att köra GitHub Actions.

Innan vi såg att det fungerade stötte vi på ett problem där vi pekade på fel folder när vi skulle deploya på OpenShift. Det löste vi genom att skriva oc apply -f deployment/. Vi hade också skrivit fel i vår oc login, där vi skrev fel string så att vi inte pekade på våra tokens. Efter att vi löst dessa problem såg vi att allt fungerade i GitHub Actions. 


