# Elektriciteit Pertz - website

## Structuur
- `index.html` - de website
- `css/style.css` - alle styling
- `js/script.js` - het mobiele menu
- `images/` - hier voeg je foto's toe (zie images/LEES-MIJ.txt)

## Openen
Dubbelklik op `index.html` om de site lokaal te bekijken in je browser.

## Foto's toevoegen
Zet een foto met de juiste naam in de `images` map (zie LEES-MIJ.txt daar) en
ze verschijnt automatisch op de bijhorende projectkaart. Geen foto? Dan blijft
de kaart gewoon donkergrijs.

## Naar GitHub pushen

```bash
cd elektriciteit-pertz
git init
git add .
git commit -m "Eerste versie site Elektriciteit Pertz"
git branch -M main
git remote add origin https://github.com/<jouw-gebruikersnaam>/ElektriciteitPertz.git
git push -u origin main
```

Maak de repo eerst aan op github.com (New repository → geen README/gitignore aanvinken, die heb je al).

## Deployen op Vercel

1. Log in op [vercel.com](https://vercel.com) met je GitHub-account.
2. Klik **Add New → Project**.
3. Selecteer de `ElektriciteitPertz` repo.
4. Framework preset: **Other** (statische site, geen build-commando nodig).
5. Klik **Deploy**.

Na een minuut krijg je een live URL zoals `elektriciteit-pertz.vercel.app`. Bij elke
`git push` naar `main` deployt Vercel automatisch de nieuwe versie.

### Eigen domeinnaam (optioneel)

In het Vercel-dashboard van je project: **Settings → Domains** → voeg je eigen
domein toe (bv. `elektriciteitpertz.be`) en volg de DNS-instructies.
