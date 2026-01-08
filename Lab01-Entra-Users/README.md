# Practice Lab 0101: Managing Identities in Entra ID


##  Exercise 1: Creating users in Entra ID
🎯 Objectif

Créer des comptes utilisateurs directement dans Microsoft Entra ID via le portail d’administration.

| Name            | User Name                          | Password  | Job title          | Department |
|-----------------|------------------------------------|-----------|--------------------|------------|
| Edmund Reeve    | ereeve@yourtenant.onmicrosoft.com  | P@ssword | HR Rep             | HR         |
| Miranda Snider  | msnider@yourtenant.onmicrosoft.com | P@ssword  | Helpdesk Manager   | Operations |
| Cody Godinez    | cgodinez@yourtenant.onmicrosoft.com | P@ssword  | Sales Rep          | Sales      |


1. Connexion au Microsoft Entra Admin Center
👉 https://entra.microsoft.com

(Compte administrateur)

2. Accès au menu Users > All users
   (Captura del menu)

Création d’un nouvel utilisateur

Type : Member

Mot de passe défini manuellement

Renseignements : nom, fonction, département

Usage location : United States

Aucune affectation de groupes ou rôles
(Configuration par défaut)
(Captura de los datos metidos al usuario.)

Vérification et validation de la création
(Captura de la verificacion de la creacion de los usuarios)

## Exercise 2 – Création d’utilisateurs avec PowerShell (Microsoft Graph)
🎯 Objectif

Créer un utilisateur Microsoft Entra ID via PowerShell 7 en utilisant le module Microsoft Graph.

1. Connexion au tenant
(Captura de la conexion al Tenant)
2. Création du profil mot de passe
(Captura de la creacion de usuarios)
3. Création de l’utilisateur Cody Godinez
(Captura con los datos del usuario Cody Godinez)
4. Vérification
 (Captura de la verificacion de la creacion)

## Exercise 2 – Attribution des rôles administratifs dans Microsoft Entra ID

🎯 Objectif

Analyser et attribuer des rôles administratifs aux utilisateurs du tenant Microsoft Entra ID selon leurs responsabilités.

| Nom             | Responsabilités principales              | Rôle administratif            |
|-----------------|------------------------------------------|-------------------------------|
| Allan Deyoung   | Gestion complète du tenant               | **Global Administrator**      |
| Edmund Reeve    | Gestion des utilisateurs et des groupes  | **User Administrator**        |
| Miranda Snider  | Réinitialisation des mots de passe       | **Helpdesk Administrator**    |


1. Accès à la gestion des rôles
2. (Captura dentro de la pantalla donde puedes editar los roles)
3. Attribution du rôle Global Administrator au Allan Deyoung
   (Captura añadiendo el role global)
5. Attribution du rôle User Administrator au Edmund Reeve
6. (Captura del role añadido)
7. Attribution du rôle Helpdesk Administrator au Miranda Snider

## 

