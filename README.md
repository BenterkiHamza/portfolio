# Portfolio — Hamza Benterki

Site vitrine statique (un seul fichier `index.html`, aucune dépendance à installer).

## Déployer sur Vercel (le plus simple, 2 minutes)

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
Tout le contenu (texte, projets, liens) est dans `index.html` — pas de build, modifie directement le HTML/CSS et redéploie.
