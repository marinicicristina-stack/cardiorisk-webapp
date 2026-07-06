# Cahier des charges — CardioRisk Web Application

## 1. Objectif

Développer une application web d’aide à la décision clinique permettant aux médecins de consulter les données d’un patient, visualiser une prédiction de risque cardiovasculaire générée par IA, et comprendre cette prédiction grâce à des explications XAI.

L’application ne remplace pas le médecin : elle l’aide à prendre une décision.

## 2. Utilisateurs

- Médecin
- Cardiologue
- Administrateur

## 3. Fonctionnalités V1

### 3.1 Authentification
- Connexion
- Déconnexion
- Gestion simple des rôles

### 3.2 Gestion des patients
- Liste des patients
- Recherche d’un patient
- Création d’un patient
- Consultation d’un dossier patient

### 3.3 Dossier patient
Le dossier patient contient :
- Informations générales
- ECG
- X-Ray
- Blood Tests
- Echocardiography
- AI Prediction
- Explainability
- Risk Factors

### 3.4 Upload des examens
Le médecin peut importer :
- fichiers ECG
- images X-Ray
- résultats biologiques
- données d’échographie

### 3.5 Prédiction IA
L’application affiche :
- score de risque cardiovasculaire
- niveau de risque : faible, modéré, élevé
- probabilité
- résumé clinique

### 3.6 Explainable AI
L’application affiche :
- facteurs ayant influencé la prédiction
- explications courtes
- visualisation type SHAP ou Grad-CAM
- lien vers les données originales

### 3.7 Facteurs de risque
L’application permet de visualiser :
- âge
- sexe
- tension artérielle
- cholestérol
- glycémie
- IMC
- antécédents

## 4. Fonctionnalités bonus

Si le temps le permet :
- partage du dossier avec un autre médecin
- commentaires médicaux
- historique complet
- notifications
- journal d’audit

## 5. Technologies envisagées

- Frontend : Next.js, React, TypeScript, Tailwind CSS
- Backend : FastAPI
- Base de données : PostgreSQL
- Authentification : JWT
- Déploiement : Docker
- API : REST

## 6. Équipe

- Cristina : Frontend, UI/UX, coordination
- Abdelhak : Backend, API, base de données, sécurité
- Agits : intégration IA, XAI, tests avec données simulées

## 7. Livrables

- Application web fonctionnelle
- Documentation technique
- Cahier des charges
- Maquettes
- Présentation finale
- Démonstration
