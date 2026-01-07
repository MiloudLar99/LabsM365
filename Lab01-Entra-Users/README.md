🧪 Lab 01 – Creating Users in Microsoft Entra ID
🎯 Objetivo del laboratorio

Crear cuentas de usuario en Microsoft Entra ID utilizando:

El portal de administración (GUI)

PowerShell (Microsoft Graph) para automatizar la creación de usuarios

🛠️ Pasos realizados (versión limpia y pro)
1️⃣ Acceso al entorno Entra ID

Inicio de sesión en Microsoft Entra Admin Center

Revisión de usuarios existentes en el tenant

Verificación de que los usuarios no están sincronizados desde on-premises (On-premises sync = No)

2️⃣ Creación de usuarios desde el portal (GUI)

Creación manual de nuevos usuarios desde Users > New user

Configuración de:

User Principal Name (UPN)

Display name

Contraseña personalizada

Job title

Department

Usage location

Validación de que los usuarios se crean correctamente en el tenant

🧑‍💼 Usuarios creados desde el portal:

Edmund Reeve (HR)

Miranda Snider (Operations)

3️⃣ Preparación del entorno PowerShell

Instalación de PowerShell 7

Instalación del módulo Microsoft.Graph

Autenticación contra Microsoft Graph con permisos administrativos

4️⃣ Creación de usuarios mediante PowerShell (automatización)

Creación de un perfil de contraseña reutilizable

Creación de un usuario mediante el cmdlet New-MgUser

Definición de atributos clave:

Nombre y apellidos

UPN

Ubicación

Departamento

Puesto de trabajo

Verificación de la creación del usuario mediante Get-MgUser

👨‍💻 Usuario creado mediante PowerShell:

Cody Godinez (Sales)

5️⃣ Verificación final

Comprobación de que los usuarios aparecen correctamente en Entra ID

Validación del estado de las cuentas creadas

📘 Referencia

Lab basado en la guía oficial de Microsoft MD-102:
https://github.com/MicrosoftLearning/MD-102T00-Microsoft-365-Endpoint-Administrator



## 📸 Evidencias

### Acceso y vista general de usuarios
![Users overview](screenshots/01-entra-users-overview.png)

### Creación de usuario – Edmund Reeve
![Create user Edmund](screenshots/02-create-user-edmund-basic-info.png)
![Edmund properties](screenshots/03-create-user-edmund-properties.png)
![Edmund assignments](screenshots/04-create-user-edmund-assignments.png)
![Review Edmund](screenshots/05-review-create-edmund.png)

### Creación de usuario – Miranda Snider
![Review Miranda](screenshots/06-create-user-miranda-review.png)

### Verificación final
![Users list](screenshots/07-users-list-after-creation.png)

### Preparación del entorno PowerShell
![PowerShell version](screenshots/08-powershell-version.png)

