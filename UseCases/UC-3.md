## UC-3 – Ajouter un livre à sa bibliothèque

<br>**Numéro** : UC-3
<br>**Nom** : Ajouter un livre à sa bibliothèque  
<br>**Acteur principal** : Lecteur  
<br>**Paquetage** : Gestion personnelle  
<br>**Importance** : Haute  
<br>**Fréquence** : Fréquente  
<br>**Objet du domaine** : Livre, Lecture, Liste de lecture

### Préconditions
- Le lecteur est connecté à son compte.
- Le livre existe déjà dans le catalogue global.

### Postconditions
- Le livre est ajouté dans une des listes de l'utilisateur (à lire, en cours, terminé).

### Scénario nominal

| Étape | Utilisateur | Système |
|-------|-------------|---------|
| 1 | Recherche un livre dans le catalogue | Affiche les résultats |
| 2 | Sélectionne un livre | Affiche la fiche du livre |
| 3 | Clique sur "Ajouter à ma bibliothèque" | Propose un état (à lire, en cours, lu) |
| 4 | Choisit l’état de lecture | Ajoute le livre dans la liste correspondante |
| 5 | — | Confirme l’ajout avec un message de succès |

### Exceptions
- Le système affiche : « Impossible d’ajouter ce livre pour le moment. »

### FQM – Fonction / Qualité / Mesure

| Fonction | Qualité | Mesure |
|----------|---------|--------|
| Ajouter un livre à sa bibliothèque | Réactivité | Ajout < 2 secondes |
| Ajouter un livre à sa bibliothèque | Fiabilité | Taux d’échec < 1 % |
| Ajouter un livre à sa bibliothèque | Accessibilité | Fonction disponible sur tous les appareils |
