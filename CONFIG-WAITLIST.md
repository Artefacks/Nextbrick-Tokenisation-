# Configuration de la waitlist — Recevoir les emails

Pour recevoir les emails des personnes qui s'inscrivent à la liste d'attente :

## Étapes

1. **Créez un compte** sur [formspree.io](https://formspree.io) (gratuit)

2. **Créez un nouveau formulaire** :
   - Cliquez sur "New Form"
   - Donnez un nom (ex. "NextBrick Waitlist")

3. **Activez les notifications email** :
   - Dans les paramètres du formulaire, section "Notifications"
   - Par défaut, Formspree envoie chaque soumission à l'adresse email de votre compte
   - Vous pouvez ajouter d'autres adresses si besoin

4. **Récupérez votre ID** :
   - L'URL de votre formulaire ressemble à : `https://formspree.io/f/xyzabcde`
   - L'ID est la partie après `/f/` : `xyzabcde`

5. **Mettez à jour le fichier** `nextbrick.html` :
   - Cherchez `YOUR_FORMSPREE_ID` (vers la ligne 1847)
   - Remplacez par votre ID : `const FORMSPREE_URL = 'https://formspree.io/f/xyzabcde';`

Dès qu'une personne s'inscrit, vous recevrez un email avec son adresse et sa tranche de budget.
