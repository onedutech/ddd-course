## Exercice : Fabrique (Factory) en DDD - Domaine de la gestion de bibliothèque

### **Contexte**

Dans une bibliothèque universitaire, il existe plusieurs types de documents :  
- Livres  
- Revues  
- Thèses

Chaque type de document possède des règles de création spécifiques :
- Un **livre** doit avoir un ISBN, un titre, un ou plusieurs auteurs.
- Une **revue** doit avoir un ISSN, un titre, un numéro de volume.
- Une **thèse** doit avoir un titre, un auteur, un directeur de thèse, et une année de soutenance.

La création de ces documents doit garantir la validité de leurs données dès l’instanciation.

---

### **Objectif**

- Concevoir une **factory** (fabrique) dans le contexte DDD pour encapsuler la création des différents types de documents.
- Appliquer la fabrique pour centraliser les règles de création et garantir la cohérence métier.

---

### **Travail demandé**

1. **Modélisez les entités ou agrégats** pour les trois types de documents (Livre, Revue, Thèse).
2. **Identifiez les règles de création** propres à chaque type de document.
3. **Implémentez une ou plusieurs fabriques** (factories) qui :
   - Centralisent la logique de création.
   - Empêchent la création d’objets invalides.
   - Peuvent être utilisées par un service applicatif ou un service de domaine.
4. **Écrivez un exemple d’utilisation** de la fabrique pour créer chaque type de document.

---

### **Questions de réflexion**

- Pourquoi la fabrique est-elle préférable à l’utilisation directe des constructeurs dans ce contexte ?
- Comment la fabrique aide-t-elle à exprimer le langage métier et à garantir la cohérence du modèle ?

---

### **Bonus**

- Proposez une extension pour gérer la création groupée de plusieurs documents (ex : acquisition d’un lot de livres).
- Ajoutez des contrôles supplémentaires (ex : ISBN/ISSN valide, année de soutenance non future).

---

**Livrables attendus :**
- Code ou pseudo-code des entités/agrégats et de la/les fabrique(s)
- Exemple d’utilisation
- Réponses aux questions de réflexion
