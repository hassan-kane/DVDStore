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
- **Base de données** : MySQL / PostgreSQL
- **Frontend** : []
- **Sécurité** : []
- **API REST** : Exposition d'une API RESTful pour interagir avec les données du stock
- **Outils de build** : Maven / Gradle

## Prérequis

- **Java 22** : [Télécharger ici](https://www.oracle.com/java/technologies/javase-jdk22-downloads.html)
- **Maven** : [Télécharger Maven](https://maven.apache.org/download.cgi)
- **MySQL** ou **PostgreSQL** : Configurer une base de données locale ou utiliser une instance distante

