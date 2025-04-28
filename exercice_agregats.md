
## ✏️ Exercice — Travailler avec les Agrégats

### Contexte :

Vous travaillez sur une application de **gestion de commandes e-commerce**.

Voici les éléments métier du domaine :

-   Un **Client** passe une ou plusieurs **Commandes**.
    
-   Chaque **Commande** contient plusieurs **Lignes de Commande** (produit + quantité).
    
-   Chaque **Commande** est associée à un **Paiement** (réalisé ou en attente).
    
-   Une Commande peut être dans l'un des états suivants : **En attente**, **Payée**, **Expédiée**.
    
-   Le **Paiement** d'une Commande ne peut être effectué que si :
    
    -   La Commande est complète,
        
    -   Le montant total est supérieur à zéro.
        

----------

### Tâches demandées :

1.  **Identifiez les Agrégats** du domaine :
    
    -   Où sont les **frontières naturelles** ?
        
    -   Quelle est la **racine d’agrégat** (Aggregate Root) ?
        
2.  **Définissez la structure de l’agrégat principal** (`Commande`) :
    
    -   Quelles entités/objets doivent rester **internes** à l'agrégat ?
        
    -   Quelles règles d'intégrité doivent être **garanties** immédiatement à l’intérieur de l'agrégat ?
        
3.  **Concevez les principales méthodes métiers** :
    
    -   Ajouter une ligne de commande,
        
    -   Payer une commande,
        
    -   Expédier une commande.
        
4.  **Posez des règles de cohérence** :
    
    -   Que doit vérifier la commande avant d'accepter un paiement ?
        

----------

### Contraintes :

-   Toutes les modifications à l’intérieur de l'agrégat doivent **passer par la racine** (`Commande`).
    
-   Les entités internes (ex : `LigneCommande`) ne doivent **jamais être manipulées directement** depuis l'extérieur.
    
-   Les règles d'invariants doivent être **immédiatement cohérentes** après toute modification.
    

----------