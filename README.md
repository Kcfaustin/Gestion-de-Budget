# AppBudget

Application web/PWA simple.

## Demarrage en local

### Prerequis
- Node.js installe

### Etapes
1. Cloner le repo:
   git clone https://github.com/TON-USERNAME/AppBudget.git
2. Entrer dans le dossier:
   cd AppBudget
3. Lancer le serveur local:
   npx serve .
4. Ouvrir l'URL affichee dans le terminal, souvent http://localhost:3000.

## Deploiement sur Vercel

1. Pousser le projet sur GitHub.
2. Ouvrir Vercel et cliquer sur New Project.
3. Importer le repo AppBudget depuis GitHub.
4. Laisser Vercel detecter le projet comme site statique.
5. Ne rien mettre dans Build Command ni dans Output Directory.
6. Cliquer sur Deploy.


## Mise à Jour

Dans sw.js actuel :
jsconst CACHE = 'budgetsplit-v1';

À chaque fois que tu fais une mise à jour, change juste le numéro :

jsconst CACHE = 'budgetsplit-v2'; // v3, v4...

## Notes

- Eviter d'ouvrir index.html en double-clic pour tester la PWA.
- Si le cache PWA gene les changements: DevTools > Application > Service Workers > Unregister.
- Une fois deployee sur Vercel, le site doit rester en HTTPS pour que le service worker fonctionne correctement.
