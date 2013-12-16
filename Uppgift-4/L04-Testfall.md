# Testfall AF1.1 Registrera sig
## <a href="../Uppgift-3/L03-Krav.md>AF 1.1 Registrera sig</a>
### Testfall
I detta testfall är målet att testa registrerings fasen för medlemmar. 
Det är viktigt att betalningsdelen testas extra noga.
#### Efterkrav
Kontrollera att ett ny användare är registrerad i systemet och även i kassörens lista.
#### Testfall 1.1 Huvudscenario
1. Gå till registreringssidan (www.gladapiraten.se/registrering)
2. Registreringsformulär presenteras
3. Användarnamn: medlem1, lösenord: pirat123, adress: testaddressgatan 1 123 45, namn: Kapten Krok, klicka på "Skicka"
4. Lyckad informationsregistrering
5. Väljer att betala med mastercard
6. Betalningsformulär presenteras
7. Kortnummer 1111 2222 3333 4444, giltighetstid 01/18, säkerhetskod 123, klicka på "skicka"
8. Lyckad betalning
9. Användaren lyckades registrera sig och blev registrerad i systemet.

#### Testfall 1.2 Alternativt scenario Misslyckad informationsregistrering 
1. Gå till registreringssidan (www.gladapiraten.se/registrering)
2. Registreringsformulär presenteras
3. Användarnamn: medlem1, lösenord: pir(här ligger felet), adress: testaddressgatan 1 123 45, namn: Kapten Krok, klicka på "Skicka"
4. Felaktig inmatning, registreingsformulär presenteras igen med ett felmeddelande vid lösenordet
5. Gå till steg 3 i huvudscenario

###### Testfall 1.3 Alternativt scenario Systemet ligger nere
1. Gå till registreringssidan (www.gladapiraten.se/registrering)
2. Registreringsformulär presenteras
3. Användarnamn: medlem1, lösenord: pirat123, adress: testaddressgatan 1 123 45, namn: Kapten Krok, klicka på "Skicka"
4. 

Användningsfallet avslutas




1. Startar när en användare vill registrera sig för att bli medlem.
2. Systemet presenterar ett formulär med information som behövs för att få en profil av användaren.
3. Användaren fyller i formuläret och skickar det.
4. Systemet kontrollerar uppgifterna och svarar att användaren blev godkänd.
5. Användaren väljer att betala medlemsavgiften med mastercard.
6. Klarna checkout presenterar ett formulär att fylla i för betalning.
7. Användaren fyller i uppgifter och skickar det.
8. Klarna checkout kontrollerar uppgifterna och svarar till systemet att betalningen gick igenom.
9. Systemet säger till användaren att han är godkänd och registrerar användaren som medlem.

TF 1.1 Huvudscenario aut. som admin
Gå till inloggninssidan (www.exempel.test/login);
Inloggningsformulär presenteras
Användarnamn: admin, Lösenord: nimda
Lyckad inloggning som admin
TF 1.2 Huvudscenario; aut. som sturelsemedlem
Gå till inloggninssidan (www.exempel.test/login)
Inloggningsformulär presenteras
Användarnamn: user, Lösenord: resu
Lyckad inloggning som styrelsemedlem
TF 1.3 Alt. Scenario 4a; misslyckad aut
Gå till inloggninssidan (www.exempel.test/login)
Inloggningsformulär presenteras