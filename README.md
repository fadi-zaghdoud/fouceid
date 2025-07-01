# FouceID - Mental Health & Wellness Platform

Une plateforme complète de santé mentale et de bien-être avec suivi d'humeur, méditation et services de santé mentale.

## 🚀 Déploiement sur Vercel

Ce projet est configuré pour être déployé facilement sur Vercel.

### Méthode 1: Déploiement via Git (Recommandé)

1. Poussez votre code sur GitHub/GitLab/Bitbucket
2. Connectez votre dépôt à Vercel
3. Vercel détectera automatiquement la configuration

### Méthode 2: Déploiement direct

1. Installez la CLI Vercel:
   ```bash
   npm i -g vercel
   ```

2. Dans le dossier du projet, exécutez:
   ```bash
   vercel
   ```

3. Suivez les instructions pour déployer

## 📁 Structure du projet

```
/
├── public/           # Pages HTML principales
│   ├── signin.html   # Page de connexion (page d'accueil)
│   ├── signup.html   # Page d'inscription
│   ├── meditation.html # Page de méditation
│   ├── mood.html     # Suivi d'humeur
│   ├── profile.html  # Profil utilisateur
│   ├── services.html # Services
│   ├── contact.html  # Contact
│   ├── FAQ.html      # FAQ
│   └── style.css     # Styles CSS
├── src/
│   └── input.css     # Fichier source Tailwind
├── video/            # Fichiers vidéo
├── *.png, *.jpg      # Images et assets
├── index.html        # Page d'accueil (redirige vers signin)
├── vercel.json       # Configuration Vercel
├── package.json      # Dependencies Node.js
└── tailwind.config.js # Configuration Tailwind
```

## 🎨 Technologies utilisées

- **HTML5** - Structure des pages
- **Tailwind CSS** - Framework CSS utilitaire
- **JavaScript** - Interactivité
- **Vercel** - Hébergement et déploiement

## 📱 Pages disponibles

- `/` - Page d'accueil (redirige vers signin)
- `/signin` - Connexion
- `/signup` - Inscription
- `/meditation` - Méditation
- `/mood` - Suivi d'humeur
- `/profile` - Profil utilisateur
- `/services` - Services
- `/contact` - Contact
- `/faq` - FAQ

## 🔧 Développement local

1. Installez les dépendances:
   ```bash
   npm install
   ```

2. Démarrez le serveur de développement:
   ```bash
   npm run dev
   ```

3. Pour construire le projet:
   ```bash
   npm run build
   ```

## 📝 Notes de déploiement

- Le projet est configuré comme site statique
- La page d'accueil (`/`) redirige automatiquement vers la page de connexion
- Tous les assets (images, vidéos) sont servis directement
- Les routes sont configurées pour des URLs propres (sans .html)

## 🛡️ Sécurité

Le projet inclut des headers de sécurité configurés dans `vercel.json`:
- X-Content-Type-Options: nosniff
- X-Frame-Options: DENY  
- X-XSS-Protection: 1; mode=block
