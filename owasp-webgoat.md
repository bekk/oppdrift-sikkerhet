# Oppgaver til OWASP Top 10 - OWASP WebGoat

## Kom i gang
1. Last ned WebGoat med docker: `docker pull webgoat/webgoat`
2. `docker run -p 8080:8080 -p 9090:9090 -p 80:8888 -e TZ=Europe/Amsterdam webgoat/webgoat:latest`
3. Gå til `http://localhost:8080/WebGoat`

## Oppgaver - Hint💡
### A01 - Broken Access Control
#### Insecure direct object reference
- Bruk nettverksfanen eller et verktøy for å inspisere og endre requester - Firefox har god støtte for endring
- Gjør kall med forskjellige id-er for å finne en annen profil
- Bruk `PUT` for å endre en annen profil (husk `content-type`)
  
#### Missing function level access control
- Inspiser skjulte elementer
- Gjør et `GET`-kall mot `/access-control/users`
  
#### Spoofing an authentication code

### A03 - Injection
#### Cross Site Scripting
- Målet er å få siden til å gjøre noe den ikke vil
- Oppgave 3-6 er bare tekst, så du kan hoppe rett til oppgave 7
#### Injection (intro)
- Hopp rett til oppgave 6 hvis du vet hvordan man skriver SQL
- Prøv noen vanlige [SQL-injection payloads](https://github.com/payloadbox/sql-injection-payload-list?tab=readme-ov-file#generic-sql-injection-payloads)

### A07 - Identification and authentication failures
#### Authentication Bypasses
#### JWT Tokens
#### Password reset

### A08 - Software and data integrity
#### Insecure Deserialization

### A09 - Security logging and monitoring failures
#### Logging security

### A10 - Server side request forgery (SSRF)
#### Cross-Site Request Forgeries
#### Server-Side Request Forgery
