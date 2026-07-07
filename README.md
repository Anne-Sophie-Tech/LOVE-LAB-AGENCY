# Love Lab Agency — Site vitrine

## Contenu
- `index.html` : le site complet (HTML + CSS + JavaScript intégrés dans un seul fichier).
  Les images (logo, favicon) sont encodées en base64 directement dans le fichier :
  aucune image externe à gérer, aucune dépendance à installer.

## Déploiement — plusieurs options simples

### 1. Hébergement statique gratuit (le plus rapide)
Ces services déploient un site statique en quelques clics, gratuitement :
- **Netlify** (netlify.com) : glissez-déposez le dossier sur "Deploys" → Drag and drop.
- **Vercel** (vercel.com) : "Add New Project" → importer le dossier.
- **GitHub Pages** : créez un dépôt, ajoutez `index.html` à la racine, activez
  "GitHub Pages" dans Settings > Pages.
- **Cloudflare Pages** : même principe, glisser-déposer le dossier.

### 2. Hébergement mutuel classique (OVH, Hostinger, o2switch, etc.)
1. Connectez-vous à votre espace d'hébergement (FTP ou gestionnaire de fichiers).
2. Copiez `index.html` à la racine du dossier public (souvent nommé `www`,
   `public_html` ou `httpdocs`).
3. Renommez-le `index.html` s'il ne l'est pas déjà (c'est le cas ici).
4. Votre site est en ligne à l'adresse de votre nom de domaine.

### 3. Nom de domaine
Si vous n'avez pas encore de nom de domaine (ex. lovelabagency.fr),
vous pouvez en réserver un chez OVH, Gandi, Namecheap, etc., puis le pointer
vers l'hébergement choisi ci-dessus.

## Personnalisation rapide
- **Prix** : recherchez les commentaires `<!-- MODIFIER LE PRIX ICI -->`
  dans `index.html` (onglet Tarifs).
- **Email de réception des formulaires** : recherchez `AGENCY_EMAIL` dans la
  balise `<script>` et remplacez par votre adresse réelle.
- **Téléphone / adresse** : recherchez le bloc `<footer>` en bas du fichier.

## Fonctionnement des formulaires
Les formulaires (Inscription, Agenda) fonctionnent sans backend : à l'envoi,
la messagerie du visiteur s'ouvre avec un message pré-rempli à destination
de votre adresse email. Si vous souhaitez plus tard un vrai système
(enregistrement en base de données, agenda synchronisé, notifications
automatiques), cela nécessitera une évolution technique (formulaire connecté
à un service comme Formspree/Netlify Forms, ou un vrai backend).
