# Laboratoire pratique 0102 : Synchronisation des identités à l'aide de Microsoft Entra Connect

## 🧩 Scénario

Contoso Corporation gérait les utilisateurs séparément dans **AD DS** et **Microsoft Entra ID**, ce qui entraînait des incohérences et une gestion inefficace.  
L’objectif de ce lab est de **connecter les deux annuaires** à l’aide de **Microsoft Entra Connect** afin de centraliser la gestion des identités.

## Task 1 – Configuration de la synchronisation avec Microsoft Entra Connect

🎯 Objectif

Configurer la synchronisation d’annuaire entre Active Directory on-premises et Microsoft Entra ID à l’aide de Microsoft Entra Connect Sync.

1. Accès à Entra Connect
- Conexion au *Microsoft Entra Admin Center*
- *Entra ID > Entra Connect*
- Onglet Manage
- Télécharger *Connect Sync Agent*
2. Installation de Microsoft Entra Connect
  - Lancer AzureAdConnect.msi
  - Accepter les termes
  - Mode *Customize*
  - Installer les composants requis.
3. Configuration de l'authentification
  - Méthode: *Password Hash Synchronization*
  - Connexion avec le compte Usuariodeltenant
    (Captura de este paso.)
4. Connexion à l'Active Directory
 - Connexion à Microsoft Entra ID
 - Connexion à Active Directory (Contoso.com)
5. Filtrage des domaines et PU
6. Finalisation

