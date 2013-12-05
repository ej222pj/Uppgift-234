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
2. Systemet presenterar ett formulär med information som behövs för att får en profil av användaren.
3. Användaren fyller i formuläret och sparar det.
4. Systemet kontrollerar uppgifterna och svarar att användaren blev godkänd.
5. Användaren väljer att betala medlemsavgiften med mastercard.
6. Klarna betalning presenterar ett formulär att fylla i för betalning.
7. Användaren fyller i uppgifter och skickar det.
8. Klarna betalning kontrollerar uppgifterna och svarar till systemet som säger till användaren att
han är godkänd och registrerar användaren som medlem.