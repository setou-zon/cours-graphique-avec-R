# Guide de Déploiement GitHub Pages

## Étapes pour Déployer votre Cours R

### 1. Préparation du Repository GitHub

1. **Créer un nouveau repository sur GitHub**
   - Allez sur [github.com](https://github.com)
   - Cliquez sur "New repository"
   - Nommez-le : `cours-r-epidemiologie` (ou autre nom de votre choix)
   - Cochez "Add a README file"
   - Cliquez "Create repository"

### 2. Upload des Fichiers

**Option A : Via l'interface web GitHub**
1. Dans votre repository, cliquez "uploading an existing file"
2. Glissez-déposez tous les fichiers de ce dossier :
   - `index.html` (fichier principal du cours)
   - `README.md` (description du projet)
   - `_config.yml` (configuration GitHub Pages)
   - `DEPLOYMENT_GUIDE.md` (ce guide)

**Option B : Via Git en ligne de commande**
```bash
# Cloner votre repository
git clone https://github.com/VOTRE-USERNAME/cours-r-epidemiologie.git
cd cours-r-epidemiologie

# Copier les fichiers dans le dossier
cp /chemin/vers/les/fichiers/* .

# Ajouter et commiter
git add .
git commit -m "Ajout du cours R en épidémiologie"
git push origin main
```

### 3. Activation de GitHub Pages

1. **Aller dans les paramètres du repository**
   - Cliquez sur l'onglet "Settings" de votre repository
   - Descendez jusqu'à la section "Pages" dans le menu de gauche

2. **Configurer la source**
   - Source : "Deploy from a branch"
   - Branch : "main" (ou "master")
   - Folder : "/ (root)"
   - Cliquez "Save"

3. **Attendre le déploiement**
   - GitHub va construire votre site (1-2 minutes)
   - Une fois prêt, l'URL sera affichée : `https://VOTRE-USERNAME.github.io/cours-r-epidemiologie`

### 4. Vérification

1. **Tester l'URL**
   - Cliquez sur l'URL fournie par GitHub
   - Vérifiez que le cours s'affiche correctement
   - Testez la navigation entre les sections

2. **Vérifier la responsivité**
   - Testez sur mobile et desktop
   - Vérifiez que les tableaux sont lisibles
   - Assurez-vous que le menu de navigation fonctionne

### 5. Personnalisation (Optionnel)

**Modifier le titre et la description :**
- Éditez `_config.yml` pour changer le titre et la description
- Modifiez `README.md` pour adapter la documentation

**Ajouter un domaine personnalisé :**
1. Dans Settings > Pages > Custom domain
2. Entrez votre domaine (ex: `cours.monsite.com`)
3. Créez un fichier `CNAME` avec votre domaine

### 6. Mise à Jour du Contenu

Pour mettre à jour le cours :
1. Modifiez `index.html` localement
2. Commitez et poussez les changements :
```bash
git add index.html
git commit -m "Mise à jour du cours"
git push origin main
```
3. GitHub Pages se mettra à jour automatiquement (1-2 minutes)

### 7. Fonctionnalités Avancées

**Analytics :**
- Ajoutez Google Analytics dans `index.html`
- Suivez les visites et l'engagement

**SEO :**
- Le fichier `_config.yml` inclut déjà les métadonnées de base
- Ajoutez des mots-clés dans `index.html` si nécessaire

**Sécurité :**
- GitHub Pages utilise HTTPS par défaut
- Aucune configuration supplémentaire nécessaire

### 8. Dépannage

**Le site ne s'affiche pas :**
- Vérifiez que GitHub Pages est activé dans Settings
- Attendez 5-10 minutes après l'activation
- Vérifiez qu'il n'y a pas d'erreurs dans l'onglet "Actions"

**Erreurs de build :**
- Vérifiez la syntaxe du fichier `_config.yml`
- Assurez-vous que `index.html` est valide
- Consultez l'onglet "Actions" pour les détails d'erreur

**Problèmes de mise en forme :**
- Vérifiez que tous les CSS sont inclus dans `index.html`
- Testez localement avant de déployer
- Utilisez les outils de développement du navigateur

### 9. Partage et Collaboration

**Partager le cours :**
- L'URL GitHub Pages peut être partagée directement
- Ajoutez le lien dans vos documents de formation
- Créez un QR code pour un accès mobile facile

**Collaboration :**
- Invitez des collaborateurs dans Settings > Manage access
- Utilisez les Issues pour les suggestions d'amélioration
- Créez des branches pour les modifications importantes

### 10. Maintenance

**Sauvegardes :**
- GitHub conserve automatiquement l'historique
- Téléchargez régulièrement une copie locale

**Mises à jour :**
- Mettez à jour le contenu selon l'évolution des données
- Ajoutez de nouvelles sections si nécessaire
- Maintenez les liens externes à jour

---

## Support Technique

Si vous rencontrez des problèmes :
1. Consultez la [documentation GitHub Pages](https://docs.github.com/pages)
2. Vérifiez les [statuts GitHub](https://www.githubstatus.com/)
3. Contactez l'équipe de formation pour assistance

## Ressources Utiles

- [Guide GitHub Pages](https://pages.github.com/)
- [Documentation Jekyll](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
- [HTML/CSS Validator](https://validator.w3.org/)

---

**Bonne chance avec votre déploiement !** 🚀

