# Oppgaver til OWASP Top 10 - OWASP WebGoat

## Kom i gang
1. Last ned WebGoat med docker: `docker pull webgoat/webgoat`
2. `docker run -p 8080:8080 -p 9090:9090 -p 80:8888 -e TZ=Europe/Amsterdam webgoat/webgoat:latest`
3. Gå til `http://localhost:8080/WebGoat`

## Oppgaver - Hint
### Broken Access Control
#### Insecure direct object reference
- Bruk nettverksfanen eller et verktøy for å inspisere og endre requester - Firefox har god støtte for endring
- Gjør kall med forskjellige id-er for å finne en annen profil
- Bruk `PUT` for å endre en annen profil (husk `content-type`)
  
#### Missing function level access control
- Inspiser skjulte elementer
- Gjør et `GET`-kall mot `/access-control/users`
  
#### Spoofing an authentication code

### Injection
#### Cross Site Scripting
- Målet er å få siden til å gjøre noe den ikke vil
#### Injection (intro)
- Hopp rett til oppgave 6 hvis du vet hvordan man skriver SQL

### Identification and authentication failures
#### Authentication Bypasses
#### JWT Tokens
#### Password reset

### Software and data integrity
#### Insecure Deserialization

### Security logging and monitoring failures
#### Logging security

### Server side request forgery (SSRF)
#### Cross-Site Request Forgeries
#### Server-Side Request Forgery
