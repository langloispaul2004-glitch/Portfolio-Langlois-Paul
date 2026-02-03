# Portfolio — Langlois Paul

Site : Portfolio d'architecture présentant des projets de Licence & Master.

## Description
Ce dépôt contient une version statique du portfolio (HTML + React via CDN + Tailwind). Le fichier principal est `index.html`. Le site est pensé pour être publié facilement sur GitHub Pages (ou Netlify / Vercel).

## Structure recommandée
- `index.html` — page principale (site complet, React via CDN)
- `README.md` — ce fichier
- `docs/` (optionnel) — si vous préférez servir `index.html` depuis `/docs` pour GitHub Pages
- `assets/` (optionnel) — images locales, polices, etc.
- `.gitignore` — fichiers/dossiers à ignorer

## Installation / Mise en ligne rapide

1. Si vous partez d'un dossier local contenant `index.html` :

```bash
# initialiser le repo local (SSH)
git init
git branch -M main
git remote add origin git@github.com:langloispaul2004-glitch/Portfolio-Langlois-Paul.git
echo "# Portfolio Langlois Paul" > README.md
cat > .gitignore <<EOF
node_modules/
.env
.DS_Store
.vscode/
EOF
git add index.html README.md .gitignore
git commit -m "Initial commit: ajout du portfolio (index.html)"
git push -u origin main
```

(ou remplacer l'URL remote par la version HTTPS si nécessaire)

2. Si le repo existe déjà et que vous voulez simplement ajouter/mettre à jour `index.html` :

```bash
git clone git@github.com:langloispaul2004-glitch/Portfolio-Langlois-Paul.git
cd Portfolio-Langlois-Paul
# copier/mettre à jour index.html dans ce dossier
git add index.html
git commit -m "Mise à jour du portfolio (index.html)"
git push origin main
```

## Activer GitHub Pages
- Aller sur : `https://github.com/langloispaul2004-glitch/Portfolio-Langlois-Paul`
- Settings → Pages
- Source : Branch = `main`, Folder = `/` (ou `/docs` si vous avez placé `index.html` dans `docs/`)
- Enregistrer. L'URL publique apparaîtra (ex. `https://langloispaul2004-glitch.github.io/Portfolio-Langlois-Paul/`).

## Bonnes pratiques / conseils
- Images : vérifiez que les URLs Google Drive / Googleusercontent sont publiques. Pour plus de fiabilité, placez les images dans `assets/` et poussez-les dans le repo.
- Accessibilité : ajoutez `alt` descriptifs à toutes les balises `<img>` (déjà ajoutés dans la version fournie).
- Liens externes : pour les liens `target="_blank"`, utilisez `rel="noopener noreferrer"`.
- Performance : pour production, il est préférable d'éviter `babel-standalone` et les CDN React en mode dev. Envisagez une conversion vers Vite / Create React App pour construire un bundle optimisé.
- SEO : ajoutez meta tags (description déjà incluse), Open Graph et favicon si besoin.
- Contact/CV : le lien vers le PDF du CV est dans le footer — vérifiez que l'accès est public.

## Contribuer
Si tu veux que je :
- ajuste le README (ajout d'un bio, titres, contact),
- prépare un `CNAME` pour un domaine personnalisé,
- convertisse le projet en build Vite/CRA,
- ou crée un commit/PR directement,

dis‑moi ce que tu souhaites et je prépare les fichiers/commandes.

## Licence
Suggéré : MIT — à adapter selon ta préférence.  
Exemple court (MIT) : inclure un fichier `LICENSE` si tu veux partager/autoriser la réutilisation.

---
Bonne publication ! Si tu veux, je peux te fournir directement le contenu d'un `LICENSE` MIT et d'un `CNAME` (si tu as un nom de domaine).  
```
