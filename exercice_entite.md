
## Exercice — Travail sur les Entités

### Contexte :

Vous devez modéliser une application de **location de véhicules** pour une société de transport.

Voici quelques règles métier de base :

-   Chaque **véhicule** (bus, voiture, camion) est identifié par un **numéro d’immatriculation unique**.
    
-   Un véhicule a des **caractéristiques** (modèlea, marque, nombre de places, type de carburant).
    
-   Les véhicules peuvent être **réservés** pour différentes périodes.
    
-   L’état du véhicule peut évoluer : **disponible**, **en maintenance**, **loué**.
    
-   Les caractéristiques techniques (modèle, marque) **ne changent pas** pendant la vie du véhicule.
    

----------

### Tâches demandées :

1.  **Identifiez** dans ce système ce qui doit être :
    
    -   Une **Entité**,
        
    -   Un **Value Object**.
        
2.  **Concevez la classe `Vehicle`** :
    
    -   Attributs nécessaires,
        
    -   Identité claire,
        
    -   Méthodes pour changer d’état (`rent()`, `return()`, `sendToMaintenance()`, etc.).
        
3.  **Proposez des Value Objects** utiles :
    
    -   Par exemple : `RegistrationNumber`, `VehicleModel`.
        
4.  **Ajoutez des règles métiers** :
    
    -   Un véhicule en maintenance ne peut pas être loué.
        
    -   Un véhicule ne peut être réservé que s’il est disponible.
        

----------

### Contraintes :

-   Chaque Entité doit :
    
    -   Avoir un identifiant naturel ou généré,
        
    -   Être capable d’évoluer au cours du temps.
        
-   Value Objects doivent être **immutables**.