# Projet JEE - Sudoku 9x9

## Description

Math Puzzle - Sudoku 9x9 est une application web de jeu de réflexion développée avec Spring Boot.

L’application permet à l’utilisateur de créer un compte, se connecter, jouer au Sudoku, sauvegarder une partie, reprendre une partie sauvegardée et consulter son score.

## Technologies utilisées

- Java 17
- Spring Boot
- Spring MVC
- Thymeleaf
- Spring Data JPA
- H2 Database
- Maven
- HTML / CSS / JavaScript

## Fonctionnalités

- Inscription d’un utilisateur
- Connexion et déconnexion
- Génération d’une grille Sudoku 9x9
- Vérification de la solution
- Sauvegarde de la partie
- Reprise d’une partie sauvegardée
- Gestion du score
- Déblocage progressif des niveaux
- Consultation des données via H2 Console

## Architecture

Le projet suit l’architecture MVC :

- Controller : gestion des requêtes HTTP
- Service : logique métier du jeu Sudoku
- Model : entités de l’application
- Repository : accès aux données
- View : pages HTML avec Thymeleaf

## Base de données H2

Lien H2 Console :

http://localhost:8090/h2-console

Paramètres :

JDBC URL: jdbc:h2:file:./data/mathpuzzle-db
User Name: sa
Password: vide

## Lancement du projet

Importer le projet comme projet Maven, puis lancer :

mvn spring-boot:run

Accès à l’application :

http://localhost:8090

## Réalisé dans le cadre d’un projet académique JEE
