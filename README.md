# Prestige Haven — site vitrine trilingue

Site statique de départ pour Prestige Haven. Il comprend les versions française, anglaise et arabe (RTL), les sections Accueil, Services, À propos et Contact, ainsi qu'un formulaire qui prépare un e-mail.

## Fichiers
- `index.html` : structure du site
- `styles.css` : design responsive
- `script.js` : traductions et interactions

## À personnaliser avant publication
1. Vérifier que `contact@prestigehaven.agency` est bien une adresse e-mail active. Le site ne crée pas cette boîte mail.
2. Ajouter le numéro WhatsApp et la zone d'activité réels.
3. Vérifier que les services décrits correspondent exactement à l'activité de l'entreprise.
4. Remplacer les photos de démonstration par des photos que vous avez le droit d'utiliser.
5. Faire relire les traductions et textes commerciaux avant publication.
6. Ajouter une politique de confidentialité adaptée si vous collectez des données personnelles. Le formulaire actuel ouvre l'application e-mail du visiteur et ne stocke pas de données sur le site.

## Tester en local
Ouvrir `index.html` dans un navigateur récent.

## Publication gratuite (méthode GitHub + Cloudflare Pages)
1. Créer un compte GitHub et un dépôt public ou privé nommé `prestige-haven-site`.
2. Importer les quatre fichiers de ce dossier à la racine du dépôt.
3. Dans Cloudflare, ouvrir Workers & Pages et créer une application Pages reliée au dépôt GitHub.
4. Pour un site HTML simple, utiliser le preset `None` et laisser le champ de commande de build vide ; le dossier de sortie doit être `/` ou la racine du projet selon les options présentées.
5. Déployer et tester l'adresse `*.pages.dev` attribuée.
6. Dans le projet Pages, aller dans Custom domains et ajouter `prestigehaven.agency`, puis suivre les instructions affichées par Cloudflare.
7. Si Cloudflare demande de transférer les serveurs DNS, copier exactement les deux serveurs de noms fournis dans Namecheap > Domain List > Manage > Nameservers > Custom DNS.
8. Avant de changer les serveurs DNS, vérifier si des enregistrements e-mail existent déjà. Les recréer dans Cloudflare si nécessaire. Ne jamais inventer les valeurs DNS.
9. Ajouter ensuite `www.prestigehaven.agency` depuis Custom domains si souhaité, et vérifier HTTPS.

La prise en charge d'un domaine racine par Cloudflare Pages nécessite que le domaine soit ajouté comme zone Cloudflare et que ses serveurs de noms pointent vers Cloudflare. Voir la documentation officielle :
https://developers.cloudflare.com/pages/configuration/custom-domains/

Le domaine reste enregistré chez Namecheap. Le renouvellement du domaine n'est pas inclus dans l'hébergement gratuit.
