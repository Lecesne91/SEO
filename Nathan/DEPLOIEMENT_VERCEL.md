# 🚀 Déploiement sur Vercel

## ✅ Fichiers Vercel créés
- `vercel.json` : Configuration Vercel optimisée
- `.vercelignore` : Fichiers à exclure du déploiement

## 📝 Étapes de déploiement

### Option 1 : Via l'interface Vercel (Recommandé)

1. **Créer un compte Vercel**
   - Va sur https://vercel.com
   - Connecte-toi avec GitHub, GitLab ou email

2. **Pousser le code sur GitHub**
   ```bash
   cd /Users/kylian/Desktop/Nathan
   git init
   git add .
   git commit -m "Initial commit - Site développeur freelance Paris"
   git branch -M main
   git remote add origin https://github.com/TON-USERNAME/developpeur-freelance-paris.git
   git push -u origin main
   ```

3. **Importer le projet sur Vercel**
   - Sur Vercel, clique "New Project"
   - Sélectionne ton repo GitHub
   - Vercel détecte automatiquement que c'est un site statique
   - Clique "Deploy" !

4. **Configuration du domaine**
   - Dans les settings du projet Vercel
   - Ajoute ton domaine : `www.developpeur-freelance-paris.com`
   - Configure les DNS chez ton registrar :
     ```
     Type: CNAME
     Name: www
     Value: cname.vercel-dns.com
     ```

### Option 2 : Via CLI Vercel

1. **Installer Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **Déployer**
   ```bash
   cd /Users/kylian/Desktop/Nathan
   vercel
   ```

3. **Suivre les instructions** dans le terminal

## 🎯 Configuration incluse dans vercel.json

✅ **URLs propres** : `/services` au lieu de `/services.html`
✅ **Headers de sécurité** : Protection XSS, clickjacking, etc.
✅ **Cache optimisé** : CSS et images cachés pendant 1 an
✅ **Redirections** : `/home` → `/`

## 🔍 Après le déploiement

1. **Vérifier le site** : https://ton-projet.vercel.app
2. **Soumettre le sitemap** à Google Search Console
   - URL du sitemap : `https://www.developpeur-freelance-paris.com/sitemap.xml`
3. **Tester les performances** sur PageSpeed Insights
4. **Configurer les analytics** (Google Analytics, Plausible, etc.)

## ⚡ Avantages Vercel pour ce site

- ✅ **Gratuit** pour les sites statiques
- ✅ **HTTPS automatique**
- ✅ **CDN global** (chargement ultra-rapide)
- ✅ **Déploiement automatique** à chaque push Git
- ✅ **Aperçus de PR** (preview deployments)
- ✅ **Domaine personnalisé** gratuit

## 📊 Performance attendue

- **Lighthouse Score** : 95-100/100
- **Temps de chargement** : < 1 seconde
- **First Contentful Paint** : < 0.5s
- **Core Web Vitals** : Excellents (bon pour le SEO !)

---

**Ton site est prêt à être déployé sur Vercel ! 🎉**
