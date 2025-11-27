# Logiciel de gestion MVC 

## 1. Contexte
Ce projet consiste à réaliser un **logiciel de gestion** en Java selon l’architecture **MVC** (Modèle – Vue – Contrôleur).

Le logiciel est utilisé par deux types d’utilisateurs : **Administrateur et Gestionnaire**

> Le développement est organisé avec le cadre **SCRUD**
## 2. Besoin
### Objectif :
Permettre la gestion des données principales de l’application via des opérations CRUD :
- Create (Créer)
- Read (Consulter, Lister)
- Update (Modifier)
- Delete (Supprimer)

### Fonctions attendues
- Authentification : se connecter / se déconnecter
- Gestion Clients : créer, consulter, modifier, supprimer
- Gestion Produits : créer, consulter, modifier, supprimer





### Répartition MVC 
- Modèle : classes métier (Client, Produit) 
- Contrôleur : reçoit les actions utilisateur et appelle les services
- Vue : écrans 

## 3. Résultat 
### Livrables :
- Diagramme de cas d’utilisation
![La page principale](https://github.com/Takidoo/Gestionnaire-De-Stock/blob/master/thumbnail/dc.png)
- Diagramme de classe
![La page principale](https://github.com/Takidoo/Gestionnaire-De-Stock/blob/master/thumbnail/dclasse.png)

### Ce que l’application permet à la fin 
- Connexion utilisateur
![La page login](https://github.com/Takidoo/Gestionnaire-De-Stock/blob/master/thumbnail/login.png)

- Interface (Vue) permettant de lister/ajouter/modifier/supprimer 
![La page principale](https://github.com/Takidoo/Gestionnaire-De-Stock/blob/master/thumbnail/main.png)


### Justification du patron de conception 

Nous avons choisi la patron **Modèle-Vue-Contrôleur** pour séparer la logique métier de l’interface utilisateur :
- Le Modèle regroupe les règles de gestion du stock (marchandise, quantités, entrées/sorties)
- La Vue s’occupe de de l’affichage (boutons) et de la saisie 
- Le Contrôleur reçoit les actions de l’user (ajouter, retirer et rechercher produit) et appelle les méthodes du Modèle
> Cette méthode rend le code plus lisible et cohérent.

