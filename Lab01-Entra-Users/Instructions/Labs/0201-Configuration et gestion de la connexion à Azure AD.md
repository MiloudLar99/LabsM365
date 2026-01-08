# Practice Lab 0201: Configuring and managing Entra Join

## Exercise 1 – Configuration de Microsoft Entra Join


### 🎯 Objectif du laboratoire

Ce laboratoire a pour objectif de configurer les paramètres des appareils dans Microsoft Entra ID afin de permettre l’inscription des postes Windows dans l’environnement cloud de l’entreprise, tout en appliquant des règles de sécurité et de gouvernance des appareils.

- Les actions réalisées incluent :

- L’autorisation pour tous les utilisateurs de joindre des appareils à Entra ID

- La limitation du nombre maximal d’appareils par utilisateur

- L’attribution de droits d’administrateur local sur tous les appareils Entra join

- L’activation de l’authentification multifacteur par SMS

- La validation du processus de Microsoft Entra Join


## Exercise 1 – Configuration de Microsoft Entra Join
1. Conneion au centre d'administration Microsoft Entra (https://entra.microsoft.com) avec un compte administrateur.
2. Accès à *Devices > All devices > Device settings.*
3. Configuration des paramètres suivants:
 - *Users may join devices to Microsoft Entra ID:* All
 - *Require MFA to register or join devices:* No
 - *Maximum number of devices per user:* 20
4. Configuration des administrateurs locaux des appareils Entra join:
   - Accès à *Local administrator settings*
   - Ajout de l'utilisateur *Allan Deyoung* via le rôle Device Administrator
5. Enregistrement des paramètres.
6. Activation de l'authentification par SMS:
 - *Authentication methods > SMS*
 - Statut défini sur *Enabled*

## Tâche 3 – Validation du Microsoft Entra Join
1. Sur le poste SEA-WS1, ouverture de Windows Terminal (Admin).
2. Exécution de la commande suivante afin de vérifier l’état de jonction du poste : dsregcmd /status
3. Vérification de la valeur AzureAdJoined : YES dans la section Device State, confirmant que le poste est bien joint à Microsoft Entra ID.
4. Ouverture de Computer Management et navigation vers Local Users and * Groups > Groups *.
5. Consultation du groupe Administrators afin de confirmer :
   - L’ajout de l’utilisateur Joni Sherman en tant qu’administrateur local
   - La présence des identités de sécurité (SID) correspondant aux rôles Entra ID Global Administrator et Entra Joined Device Administrator
6. Navigation vers Devices > All devices et validation de la présence du poste SEA-WS1, avec :
   - *Join type:* Microsoft Entra joined
   - *Owner*: Joni sherman

## Tâche 4 - Connexion à Windows avec un utilisateur Microsoft Entra ID

1. Sur le poste SEA-WS1, connexion à Windows avec l’utilisateur JoniS@yourtenant.onmicrosoft.com
 à l’aide du mot de passe du tenant.
2. Attente de la création automatique du profil utilisateur.
3. Validation de l’utilisation de Windows Hello pour le compte Entra ID.
4. Configuration de la sécurisation du compte :
   - Sélection de I want to set up a different method
   - Choix de la méthode Phone pour l’authentification
5. Saisie d’un numéro de téléphone mobile capable de recevoir des SMS, puis validation.
6. Réception et saisie du code de vérification SMS afin de finaliser la configuration de l’authentification par téléphone.
7. Configuration d’un code PIN Windows Hello et validation de la configuration.

## Tâche 5 – Suppression d’un appareil Windows de Microsoft Entra ID
1. Sur le poste SEA-WS1, tout en étant connecté avec l’utilisateur Joni Sherman.
2. Accès à *Settings > Accounts > Access work or school.*
3. Sélection du compte Connected to Contoso’s Azure AD.
4. Sélection de l’option Disconnect, puis confirmation de l’action.
5. Validation de la déconnexion sur la page Disconnect from the organization.
6. Saisie des identifiants administrateur locaux (Admin) afin d’autoriser la suppression de l’appareil.
7. Redémarrage du poste pour finaliser la suppression de l’appareil de Microsoft Entra ID.
   
