# Testfall för AF1.1 Registrera sig
<a href="../Uppgift-3/Use_case/AF1.1_Registrera_sig.md">AF1.1 Registrera sig</a>
## <a href="../Uppgift-3/L03-Krav.md">Kravspecifikation Båtklubben "Den Glade Piraten"</a>
### Testfall 1.1 Huvudscenario
I detta testfall är målet att testa registrerings fasen för medlemmar. 
Det är viktigt att betalningsdelen testas extra noga.
#### Efterkrav
Kontrollera att ett ny användare är registrerad i systemet och även i kassörens lista.
###### Scenario
1. Gå till registreringssidan (www.gladapiraten.se/registrering)
2. Registreringsformulär presenteras
3. <a href="#" name="3"></a>Användarnamn: medlem1, lösenord: pirat123, adress: testaddressgatan 1 123 45, namn: Kapten Krok, klicka på "Skicka"
4. Lyckad informationsregistrering
5. Väljer att betala med mastercard
6. Betalningsformulär presenteras
7. <a href="#" name="7"></a>Kortnummer 1111 2222 3333 4444, giltighetstid 01/18, säkerhetskod 123, klicka på "skicka"
8. Lyckad betalning
9. Användaren lyckades registrera sig och blev registrerad i systemet.

### Testfall 1.2 Alternativt scenario Misslyckad informationsregistrering 
###### Scenario
1. Gå till registreringssidan (www.gladapiraten.se/registrering)
2. Registreringsformulär presenteras
3. Användarnamn: medlem1, lösenord: pir(här ligger felet), adress: testaddressgatan 1 123 45, namn: Kapten Krok, klicka på "Skicka"
4. Felaktig inmatning, registreingsformulär presenteras igen med ett felmeddelande vid lösenordet
5. <a href="#3">Gå till steg 3 i huvudscenario</a>

### Testfall 1.3 Alternativt scenario Systemet ligger nere
###### Scenario
1. Gå till registreringssidan (www.gladapiraten.se/registrering)
2. Registreringsformulär presenteras
3. Användarnamn: medlem1, lösenord: pirat123, adress: testaddressgatan 1 123 45, namn: Kapten Krok, klicka på "Skicka"
4. Systemet kan inte ta in uppgifterna pga att det ligger nere. Spara inmatningen i localstorage
5. Testfallet avslutas

### Testfall 1.4 Alternativt scenario Misslyckad betalning
###### Förkrav 
Informationsregistreringen ska ha lyckats och man börjar betala
###### Scenario
1. Väljer att betala med mastercard
2. Betalningsformulär presenteras
3. Kortnummer 1111 2222 3333 (här ligger felet), giltighetstid 01/18, säkerhetskod 123, klicka på "skicka"
4. Felaktig inmatning, betalningsformuläret presenteras med ett felmeddelande vid kortnummret
5. <a href="#7">Gå till steg 7 i huvudscenario</a>

### Testfall 1.5 Alternativt scenario Klarna betalning ligger nere
###### Förkrav 
Informationsregistreringen ska ha lyckats och man börjar betala
###### Scenario
1. Väljer att betala med mastercard
2. Betalningsformulär presenteras
3. Kortnummer 1111 2222 3333 4444, giltighetstid 01/18, säkerhetskod 123, klicka på "skicka"
4. Klarna betalning kan inte ta in uppgifterna pga att det ligger nere. Spara inte inmatningen i localstorage
5. Testfallet avslutas