 # Landingspagina – Maison Ambrose

Statische one-page site (HTML + CSS + een beetje JS), gebouwd met Claude ("vibe coded"), klaar voor GitHub Pages.

## Inhoud
| Sectie | Wat |
|---|---|
| Hero | "One scent. After dark." + campagnefilm (Firefly, 12 s, autoplay zonder geluid) + 2 CTA-knoppen |
| Verhaal | merkverhaal "Less choosing. More you." + groepsfoto van de vier geuren + 3 pijlers (één geur, de avond, unisex) |
| Geuren | 4 kaarten: Iris, Noir, Amber, Sage (gelabelde productfoto's) |
| CTA | aanmeldformulier "Join the night list": voornaam, e-mail, opt-in (niet vooraf aangevinkt) |
| Footer | AI- en privacyvermelding |

Visuals (min. 3): campagnefilm, 6 productfoto's, skyline-achtergrond (allemaal in `assets/`).
Huisstijl: Space Grotesk + Cormorant Garamond (Google Fonts), #7453A2, #140D4F, #E28413, #FBF5F3.

## MailerLite-koppeling (klaar)
- Het formulier behoudt de eigen huisstijl, maar verstuurt naar MailerLite-form `203580669380527733` (account `2749389`) via
  `https://assets.mailerlite.com/jsonp/2749389/forms/203580669380527733/subscribe`.
- Velden: `fields[name]` (voornaam), `fields[email]`, plus de verplichte opt-in-checkbox (niet vooraf aangevinkt, wordt in de browser gecontroleerd).
- Na verzenden verschijnt de melding "Welcome to the night." op de pagina; bij een fout verschijnt een rode melding.
- Een kleine tracking-call (`/takel`) telt formulierweergaven in MailerLite.
- Getest met een gesimuleerde MailerLite-respons (geen echte inschrijving aangemaakt). Test zelf live met je eigen e-mailadres zodra de site online staat.
- Zet in MailerLite double opt-in aan (Forms > jouw form > Settings) voor de GDPR.

## Publiceren op GitHub Pages
1. Maak een nieuwe public repository op github.com (bv. `maison-ambrose`).
2. Upload `index.html` en de map `assets/` (Add file > Upload files) en commit.
3. Settings > Pages > Source: "Deploy from a branch" > Branch `main` / `(root)` > Save.
4. Na 1–2 minuten staat de site op `https://<gebruikersnaam>.github.io/maison-ambrose/`. Zet die link in README en verslag en test hem.

## Lokaal bekijken
Open `index.html` in de browser (dubbelklik).
