# Gestion du stock de DVD - Extranet 


## Description du projet

Ce projet a pour objectif de développer une application Extranet en utilisant **Spring Boot** pour permettre au gérant d'un magasin de DVD de gérer à distance son stock. Cette solution permettra de suivre en temps réel l'état de l'inventaire, d'ajouter de nouveaux DVD, de modifier les informations des articles existants, et de supprimer ceux qui ne sont plus disponibles.

L'application est accessible via une interface web sécurisée, facilitant la gestion des stocks depuis n'importe quel appareil connecté à Internet.


## Fonctionnalités

- **Consultation du stock** : Affichage des DVD disponibles avec des détails tels que le titre, la quantité, le genre, etc.
- **Ajout de DVD** : Insertion de nouveaux titres avec des informations comme le nom du film, le genre, la date de sortie, etc.
- **Mise à jour des DVD** : Modification des données d'un DVD existant (titre, prix, quantité, etc.).
- **Suppression de DVD** : Retrait des DVD qui ne sont plus en stock ou en vente.
- **Recherche avancée** : Recherche de DVD par titre, genre, acteur ou année de sortie.
- **Notifications** : Alerte lorsqu'un DVD est en rupture de stock ou atteint un seuil défini.
- **Historique des transactions** : Suivi des entrées et sorties du stock pour analyser les mouvements.


## Technologies utilisées

- **Backend** : Spring Boot (Java)
- **Base de données** : [A définir]
- **Frontend** : [A définir]
- **Sécurité** : [A définir]
- **API REST** : Exposition d'une API RESTful pour interagir avec les données du stock
- **Outils de build** : Maven / Gradle


## Prérequis

- **Java 17+** : [Télécharger ici](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html)
- **Maven** : [Télécharger Maven](https://maven.apache.org/download.cgi)
- **[A définir]**  : Configurer une base de données locale ou utiliser une instance distante


## Installation et configuration

### 1. Cloner le dépôt

```bash
git clone https://github.com/username/dvd-stock-management-springboot.git
cd dvd-stock-management-springboot
```

### 2. Configurer l'application

Renommez le fichier application.properties.example en application.properties, puis configurez les détails de votre base de données :

#### **Exemple de configuration MySQL :**

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/dvd_store
spring.datasource.username=your_db_username
spring.datasource.password=your_db_password

#### **Configuration JPA / Hibernate :**
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 3. Installation des dépendances
Exécutez Maven pour installer les dépendances du projet :
 
```bash
mvn clean install
```

### 4. Lancer l'application
Démarrez l'application Spring Boot avec la commande suivante :

```bash
mvn spring-boot:run
````

### 5. Accéder à l'application
L'application sera accessible à l'adresse suivante :

```bash
http://localhost:8080
```

## API REST
L'API expose plusieurs endpoints pour gérer les DVD. Voici quelques exemples :

* GET /api/dvds : Récupère tous les DVD
* GET /api/dvds/{id} : Récupère un DVD par son ID
* POST /api/dvds : Ajoute un nouveau DVD
* PUT /api/dvds/{id} : Met à jour un DVD existant
* DELETE /api/dvds/{id} : Supprime un DVD


## Tests
Pour exécuter les tests unitaires et d'intégration, utilisez la commande suivante :

```bash
mvn test
```

## Licence
Ce projet est sous licence [Nom de la licence, ex: MIT, Apache 2.0, GPL].
