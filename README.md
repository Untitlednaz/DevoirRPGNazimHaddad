## Fonctionnalités

1. **Affichage du magasin d’armes** :
   - Le joueur peut consulter les armes disponibles dans le magasin.
   - Chaque arme a des caractéristiques uniques : nom, dégâts, prix.

2. **Achat d’armes** :
   - Le joueur peut acheter une arme s’il a assez d’or.
   - Si le joueur n’a pas assez d’or, un message lui indique qu’il ne peut pas effectuer l’achat.

3. **Gestion du menu** :
   - Le joueur peut choisir parmi différentes actions via un menu interactif :
     - Afficher le magasin,
     - Quitter le jeu.

## Structure du code

Le projet est organisé en plusieurs classes pour bien séparer les responsabilités :

1. **`Weapon`** :
   - Classe de base pour toutes les armes.
   - Contient les attributs communs : `name`, `damage`, `price`.
   - Méthode pour afficher les informations de l’arme (`displayInfo`).

2. **Armes spécifiques** :
   - **`Axe`** : Une hache avec des dégâts élevés.
   - **`Hammer`** : Un marteau puissant mais cher.
   - **`Bow`** : Un arc léger et abordable.
   - Ces classes héritent de `Weapon` pour réutiliser les propriétés et méthodes.

3. **`WeaponStore`** :
   - Représente le magasin d’armes.
   - Gère la liste des armes disponibles.
   - Permet au joueur de visualiser les armes et d’en acheter.

4. **`RPGGame`** :
   - Classe principale contenant la méthode `main`.
   - Gère l’interaction avec le joueur via la console.
   - Affiche le menu principal et réagit aux choix du joueur.
