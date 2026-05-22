# creatievemaan.nl – Jekyll website

Statische website voor **De Creatieve M(a)an** (Jan-Willem Manenschijn), gebouwd met [Jekyll](https://jekyllrb.com/) en gedeployed via GitHub Pages.

## Pagina's

- **Home** – introductie en highlights
- **Over mij** – achtergrond en werkwijze
- **Aan de slag** – spellen en sessies die je kunt boeken
- **Projecten** – o.a. Raccoon Serious Games en Jump Serious Games

## Lokaal draaien

```bash
bundle install
bundle exec jekyll serve
```

Open [http://127.0.0.1:4000](http://127.0.0.1:4000).

## GitHub Pages

1. Ga in de repository naar **Settings → Pages**
2. Kies **Source: GitHub Actions**
3. Bij een push naar `main` bouwt en deployt de workflow `.github/workflows/pages.yml` automatisch

### Custom domain (creatievemaan.nl)

Het bestand `CNAME` staat al op `creatievemaan.nl`. Voeg bij je DNS-provider een record toe:

| Type  | Naam | Waarde              |
|-------|------|---------------------|
| CNAME | @    | `janwillemm.github.io` |
| CNAME | www  | `janwillemm.github.io` |

(Vervang `janwillemm` door je GitHub-gebruikersnaam als die afwijkt.)

Schakel in GitHub Pages-instellingen **Enforce HTTPS** in.

## Structuur

```
_config.yml          Site-instellingen en navigatie
_data/games.yml      Spellen voor “Aan de slag”
_projects/           Individuele projectpagina's
_layouts/            HTML-templates
_includes/           Header, footer, head
assets/              CSS, JS, afbeeldingen
```

## Huisstijl

Kleuren en typografie zijn overgenomen van [creatievemaan.nl](https://creatievemaan.nl):

- Primary `#2E3A59`
- Secondary `#B2F5EA`
- Accent `#FF6F61`
- Fonts: Montserrat & Open Sans
