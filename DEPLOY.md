# Déployer le Planificateur de Menus sur GitHub Pages

## Prérequis
- Un compte GitHub (gratuit) : https://github.com

## Étapes de déploiement

### 1. Créer un repository sur GitHub

1. Allez sur https://github.com/new
2. Nom du repository : `menu-generator` (ou ce que vous voulez)
3. Laissez "Public" coché (nécessaire pour GitHub Pages gratuit)
4. Ne cochez PAS "Add a README file"
5. Cliquez sur "Create repository"

### 2. Pousser le code vers GitHub

Après avoir créé le repository, GitHub vous affiche des commandes. Exécutez celles-ci dans le Terminal :

```bash
cd ~/menu-generator
git remote add origin https://github.com/VOTRE_USERNAME/menu-generator.git
git branch -M main
git push -u origin main
```

Remplacez `VOTRE_USERNAME` par votre nom d'utilisateur GitHub.

### 3. Activer GitHub Pages

1. Allez dans votre repository sur GitHub
2. Cliquez sur **Settings** (onglet en haut)
3. Dans le menu de gauche, cliquez sur **Pages**
4. Dans "Source", sélectionnez **Deploy from a branch**
5. Dans "Branch", sélectionnez **main** et **/ (root)**
6. Cliquez sur **Save**

### 4. Accéder à votre application

Après 1-2 minutes, votre application sera disponible à :

```
https://VOTRE_USERNAME.github.io/menu-generator/
```

## Utilisation sur iPhone

1. Ouvrez Safari sur votre iPhone
2. Allez à l'URL de votre application
3. Appuyez sur le bouton **Partager** (carré avec flèche vers le haut)
4. Faites défiler et appuyez sur **Sur l'écran d'accueil**
5. Donnez un nom (ex: "Menus") et appuyez sur **Ajouter**

L'application apparaîtra comme une app sur votre écran d'accueil !

## Mettre à jour l'application

Quand vous modifiez des fichiers :

```bash
cd ~/menu-generator
git add -A
git commit -m "Description des changements"
git push
```

Les changements seront en ligne en 1-2 minutes.

## Alternatives gratuites

### Netlify (encore plus simple)
1. Allez sur https://app.netlify.com
2. Créez un compte (gratuit)
3. Glissez-déposez le dossier `menu-generator` sur la page
4. Votre site est en ligne immédiatement !

### Vercel
1. Allez sur https://vercel.com
2. Connectez votre compte GitHub
3. Importez le repository
4. Déploiement automatique !
