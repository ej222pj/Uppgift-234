# AF1.1 Registrera sig
    En användare vill registrera sig på hemsidan och betala sin medlemsavgift.
    Systemet erbjuder han ett formulär att fylla i för att kunna logga in.
### Primär Aktör
Medlem
### Stödjande Aktör
Klarna betalning: Har hand om betalningen av medlemsavgifterna.
### Offstage Aktör
Webbkonsult: Support om det inte skulle gå att registrera sig eller om avgifts
betalningen inte fungerar.
### Efterkrav
Medlemmen kan börja registrera båtar och se information för medlemmar.
## Huvudscenario
1. Startar när en användare vill registrera sig för att bli medlem.
2. Systemet presenterar ett formulär med information som behövs för att få en profil av användaren.
3. Användaren fyller i formuläret och skickar det.
4. Systemet kontrollerar uppgifterna och svarar att användaren blev godkänd.
5. Användaren väljer att betala medlemsavgiften med mastercard.
6. Klarna betalning presenterar ett formulär att fylla i för betalning.
7. Användaren fyller i uppgifter och skickar det.
8. Klarna betalning kontrollerar uppgifterna och svarar till systemet att betalningen gick igenom.
9. Systemet säger till användaren att han är godkänd och registrerar användaren som medlem.

## Alternativa Scenarios
4a Systemet kontrollerar uppgifterna och svarar att användaren inte blev godkänd.
1. Användaren kontrollerar sina uppgifter och ändrar uppgifterna som blev fel.
2. Systemet kontrollerar uppgifterna och svarar att användaren blev godkänd.
Gå till steg 5.

4b1 Systemet ligger nere och kan inte ta in uppgifterna som skickas mot systemet. Systemet skickar ett felmeddeleande.
1. Användaren försöker en gång till och kan då skicka uppgifterna
Gå till steg 5

4b2 Systemet ligger nere och kan inte ta in uppgifterna som skickas mot systemet. Systemet skickar ett felmeddeleande.
1. Användaren försöker en gång till med samma resultat
    Användningsfallet avslutas

8a Klarna betalning kontrollerar uppgifterna och svarar till systemet att betalningen inte gick igenom.
1. Systemet säger till användaren att betalningen inte gick igenom.
2. Användaren kontrollerar sina uppgifter, ändrar det felaktiga och skickar formuläret igen.
Gå till steg 9.

8b1 Klarna betalning ligger nere och kan inte ta in uppgifterna som skickas av användaren. klarna skickar ett felmeddeleande.
1. Användaren försöker en gång till och kan då skicka uppgifterna
Gå till steg 9

8b2 Klarna betalning ligger nere och kan inte ta in uppgifterna som skickas av användaren. klarna skickar ett felmeddeleande.
1. Användaren försöker en gång till och kan då skicka uppgifterna
    Användningsfallet avslutas 