# Portfolio — Hamza Benterki

Site vitrine statique (`index.html` + `style.css`, aucune dépendance à installer).

## Déployer sur Netlify (2 minutes)

**Option A — sans ligne de commande (le plus rapide)**
1. Va sur https://app.netlify.com/drop
2. Glisse-dépose le dossier contenant `index.html` et `style.css` directement dans la page.
3. Netlify déploie immédiatement et te donne une URL du type `nom-aleatoire.netlify.app`.
4. Pour un nom personnalisé : **Site configuration → Change site name** (ex. `hamza-benterki.netlify.app`), ou relie un domaine perso dans **Domain management**.

**Option B — avec la CLI Netlify**
```bash
npm install -g netlify-cli
cd portfolio
netlify login
netlify deploy        # déploiement de test (preview URL)
netlify deploy --prod # mise en ligne définitive
```
Lors du premier `netlify deploy`, la CLI demande le dossier à publier (`publish directory`) : réponds `.` si `index.html` est à la racine.

**Option C — via GitHub (déploiement continu)**
1. Crée un dépôt GitHub et pousse ce dossier dedans.
2. Sur https://app.netlify.com : **Add new site → Import an existing project → Deploy with GitHub**, sélectionne le dépôt.
3. Build settings : laisse **Build command** vide et **Publish directory** = `.` (racine, ou le dossier où se trouve `index.html`).
4. Clique sur **Deploy site**. Chaque `git push` redéploiera automatiquement le site.

## Déployer sur Vercel (alternative, 2 minutes)

**Option A — sans ligne de commande**
1. Va sur https://vercel.com et connecte-toi (avec ton compte GitHub par exemple).
2. Clique sur **Add New → Project**.
3. Choisis **"Deploy without Git" / glisser-déposer un dossier** (ou pousse ce dossier sur un dépôt GitHub puis importe-le).
4. Vercel détecte un site statique automatiquement — aucune configuration nécessaire. Clique sur **Deploy**.
5. Tu obtiens une URL du type `hamza-benterki.vercel.app`. Tu peux la personnaliser dans **Settings → Domains**.

**Option B — avec la CLI Vercel**
```bash
npm install -g vercel
cd portfolio
vercel        # suit les instructions, puis confirme
vercel --prod # pour mettre en ligne la version finale
```

**Option C — via GitHub (déploiement continu)**
1. Crée un dépôt GitHub et pousse ce dossier dedans.
2. Sur vercel.com : **Add New → Project → Import Git Repository**, sélectionne le dépôt.
3. Chaque `git push` redéploiera automatiquement le site.

## Personnaliser
Tout le contenu (texte, projets, liens) est dans `index.html`, le style et les thèmes clair/sombre sont dans `style.css` — pas de build, modifie directement le HTML/CSS et redéploie.