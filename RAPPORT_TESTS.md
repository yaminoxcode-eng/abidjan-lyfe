# Rapport de test — Abidjan Life
Date : 12 novembre 2026
Branche : develop/abidjan-life-stabilisation

## Correction effectuée
- Correction du vecteur horizontal droite/gauche relatif à la caméra.
- Avant : l'axe droite était inversé, ce qui inversait Q/D et les flèches gauche/droite.
- Après : à yaw 0, l'axe droite pointe vers +X et l'axe avant vers -Z.
- Ajout de preventDefault pour les flèches et la barre Espace afin d'éviter le défilement de page pendant le jeu.

## Vérifications réalisées
- Contrôle de syntaxe JavaScript avec Node.js : réussi.
- Test mathématique des vecteurs avant/droite à 0°, 90°, 180° et -90° : réussi. Vecteurs unitaires et perpendiculaires.
- Vérification du fichier sur GitHub : réussie.
- Commit de correction : 4f3d9d65504b0a20868f1986bb164feb4d5db1f9.

## Tests non réalisés
- Test réel des touches dans un navigateur interactif : non validé.
- Chromium headless a dépassé le délai d'exécution dans cet environnement et n'a pas fourni de DOM exploitable.
- Déploiement Vercel : en attente de l'autorisation d'accès à l'équipe Vercel. Aucun projet RAFORI n'a été modifié.

## Conclusion
Le défaut d'inversion gauche/droite est corrigé dans le code de la branche. Les tests de logique et de syntaxe passent, mais il reste à valider le déplacement en jeu dans un navigateur après connexion Vercel.
