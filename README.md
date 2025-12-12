# Grupp 3

Arash, Simon N, Anette, Kasper, Andreas H, Martin E, Christoffer.

---

Vi har ändrat i en yaml fil, deployment->backend.yaml. Det vi ändrade var storage, till lvms-vg1. Vi fick göra det för att vår förra storage class inte kunde binda. Vi behöver endast oc apply på den vi ändrat. 

Vi har skapat en action secrets i github som är för workflow filen. I vår build and deploy fil pekar vi på dessa secrets för authenticering. Genom att göra detta blir våra containers privata. 

Eftersom vi hade gjort vår Guestbook i Redhat sandbox miljö var vårt första steg att skapa Guestbooken i din labbmiljö Du (Jonas). Efter vi har konfigurerat detta och skrivit klart vår workflowfil så kommer vi att testa att de fungerar, testar i github actions. 

Innan vi såg att de fungerade ås stöttre vi på ett problem där vi pekade på fel folder när vi skulle deploya på openshioft det löste vi igenom att skriva ”oc apply -f deployment/. Vi hade också skrivit fel på våran ”oc login” där vi skrev fel string så vi pekade inte på våra tokens. Efter vi löst dessa problem såg vi att allt fungerade i github actions. 


