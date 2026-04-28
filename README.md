# ADAM Ads Specialist PWA

ADAM est une PWA separee du cockpit HOLIAE.

Elle lit le Google Sheet `HOLIAE_Cockpit_Data` et affiche :
- la decision du jour depuis `ADAM_Advice`
- les fuites budget
- les classifications de search terms
- les decisions campagnes
- les keywords et ad groups a traiter
- les idees creativite RSA/assets
- la qualite des donnees

## Donnees attendues

Le script `holiae_cockpit_automation/google_ads_daily_sync.js` doit remplir les onglets `GAds_*`.

Le script `holiae_cockpit_automation/sheet_apps_script.js` doit remplir `ADAM_Advice` via `syncAdamAdvice`.

## Deploiement

Publier ce dossier comme une PWA statique, par exemple via GitHub Pages.

Fichiers requis :
- `index.html`
- `manifest.json`
- `sw.js`
- `icon-192.png`
- `icon-512.png`

## Limite v1

ADAM ne modifie pas Google Ads automatiquement. Il recommande seulement les actions a valider.
