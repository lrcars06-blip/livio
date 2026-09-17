# LivElec — site vitrine

Site statique (HTML/CSS/JS) pour Livio Pereira, électricien à Verdun.

Fichiers : `index.html` (site), `mentions-legales.html`, `confidentialite.html`, `logo.png` (emblème), `liv.png` / `elec.png` / `tag-*.png` (découpes du logo pour l'intro), `favicon.png`, `vercel.json`.

## Déploiement Vercel
1. Pousser ce dossier sur un dépôt GitHub.
2. Sur vercel.com → Add New Project → importer le dépôt.
3. Framework preset : **Other**. Build command : vide. Output directory : vide (racine).
4. Deploy.

## Contacts intégrés
- Instagram : @livelec55 (constante `INSTAGRAM_HANDLE` dans `index.html`).

## Nom de domaine
1. Vercel → projet → Settings → Domains → ajouter `livelec.fr` (ou autre) et `www.livelec.fr`.
2. Chez le registrar, enregistrements DNS :
   - `@` → A → `76.76.21.21`
   - `www` → CNAME → `cname.vercel-dns.com`
3. Attendre la propagation (quelques minutes à quelques heures). Le HTTPS est émis automatiquement par Vercel.
4. Vérifier ensuite que `mentions-legales.html` et `confidentialite.html` s'ouvrent depuis le footer et que les liens `mailto:` / `tel:` / WhatsApp fonctionnent sur téléphone.
