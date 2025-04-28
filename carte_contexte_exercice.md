# Exercice : Cartographie des Contextes dans un Système de Logistique Maritime

## Contexte Métier
Vous travaillez pour une entreprise de logistique maritime qui souhaite moderniser son système de gestion des expéditions. Le système actuel est monolithique et difficile à maintenir. L'objectif est de découper le système en contextes bornés (Bounded Contexts) et de définir leurs interactions stratégiques.

### Domaines Clés Identifiés :
1. **Réservation de Cargaison**  
   - Gestion des bookings clients
   - Calcul des tarifs et surréservations (overbooking)
   - Contrats de transport

2. **Suivi de Cargaison**  
   - Traçabilité en temps réel
   - Gestion des transferts de responsabilité
   - Intégration avec les capteurs IoT

3. **Gestion des Stocks Portuaires**  
   - Allocation des espaces de stockage
   - Optimisation des rotations de conteneurs

4. **Facturation & Douanes**  
   - Génération des documents légaux (connaissement, etc.)
   - Intégration avec les systèmes douaniers externes

5. **Partenaire Transporteurs**  
   - Interface avec les compagnies maritimes externes
   - Gestion des créneaux d'accostage

---

## Consignes

### Partie 1 - Identification des Contextes Bornés
1. **Listez 5 contextes bornés** en vous basant sur les domaines clés.  
2. **Classez chaque contexte** en *Core* (cœur métier), *Support* ou *Générique*.

### Partie 2 - Cartographie des Interactions
1. **Dessinez un Context Map** incluant tous les contextes identifiés.  
2. **Annotez les relations** entre contextes en utilisant les patterns DDD appropriés :  
   - Customer/Supplier  
   - Partnership  
   - Shared Kernel  
   - Anti-Corruption Layer (ACL)  
   - Open Host Service (OHS) 
   - Conformist 

### Partie 3 - Étude de Cas : Intégration Douanière
Le système douanier externe utilise un modèle de données incompatible avec le vôtre (ex: `CustomsDeclaration` vs `BillOfLading`).  
1. **Quel pattern utiliser** pour intégrer ce contexte externe ?  
2. **Proposez un exemple de code** illustrant ce pattern.

---

## Livrables Attendus
- Diagramme de contexte (format libre : draw.io, draft.io, Mermaid, etc.)
- Justification écrite des choix de patterns (1 page max)
- Extraits de code pour l'étude de cas (si applicable)

