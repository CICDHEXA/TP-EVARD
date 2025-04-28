## Stack de l'utilisateur

### GitLab CE
- **Nom** : GitLab CE
- **Version** : 17.9.7
- **CVE** :
  - **CVE-2025-2443**
    - Nom : XSS via Maven proxy cache headers
    - Score : 7.5
    - Descriptif : Un attaquant peut injecter du code malveillant dans le navigateur via des en-têtes de cache contournant les sécurités
  - **CVE-2025-1908**
    - Nom : Suivi des activités de navigation
    - Score : 6.8
    - Descriptif : Permet le suivi des activités utilisateurs menant à un risque de prise de contrôle de comptes
  - **CVE-2025-0639**
    - Nom : Déni de service via aperçu des problèmes
    - Score : 6.5
    - Descriptif : Exploitation de l'aperçu des problèmes pour provoquer une indisponibilité du service
  - **CVE-2025-1677**
    - Nom : Déni de service via exportation CI
    - Score : 6.2
    - Descriptif : Charge utile lourde envoyée lors d'export CI pouvant entraîner un crash du service

### GLPI
- **Nom** : GLPI
- **Version** : 10.0.18
- **CVE** :
  - **CVE-2025-25192**
    - Nom : Accès non autorisé au mode débogage
    - Score : 7.2
    - Descriptif : Utilisateur peu privilégié pouvant activer le debug et accéder à des infos sensibles
  - **CVE-2025-23046**
    - Nom : Accès non autorisé via OauthIMAP
    - Score : 7.1
    - Descriptif : Authentification contournée via un compte IMAP configuré incorrectement
  - **CVE-2025-24799**
    - Nom : Injection SQL avant authentification
    - Score : 9.8
    - Descriptif : Exécution de requêtes SQL par des attaquants non authentifiés sur l'inventaire
  - **CVE-2025-24801**
    - Nom : Exécution de code post-authentification
    - Score : 8.7
    - Descriptif : Chargement forcé de fichiers PHP sur serveur GLPI après authentification

### Ansible
- **Nom** : Ansible
- **Version** : v2.17.11
- **CVE** :
  - **CVE-2023-4237**
    - Nom : Fuite de clés privées dans les logs
    - Score : 7.5
    - Descriptif : Module EC2 clé affichant accidentellement la clé privée dans la sortie standard
  - **CVE-2023-39059**
    - Nom : Exécution de code via variables additionnelles
    - Score : 8.6
    - Descriptif : Injection de charges utiles malveillantes exploitant la fonctionnalité des variables

### Argo CD
- **Nom** : Argo CD
- **Version** : 2.11
- **CVE** :
  - **CVE-2024-40634**
    - Nom : Déni de service via payload JSON massif
    - Score : 7.5
    - Descriptif : Payload JSON massif causant surconsommation mémoire et plantage serveur
  - **CVE-2024-37152**
    - Nom : Fuite de paramètres sensibles
    - Score : 7.2
    - Descriptif : Paramètres de configuration exposés via API sans authentification
  - **CVE-2024-45338**
    - Nom : Déni de service via parsing YAML
    - Score : 7.8
    - Descriptif : YAML malformé ralentissant l'analyse et entraînant indisponibilité du service

### OpenVAS
- **Nom** : OpenVAS
- **Version** : 22.4
- **CVE** : 
    - **CVE-2018-9995**
        - Nom : Bypass authentification DVR
        - Score : 9.8
        - Descriptif : Permet à un attaquant d'accéder au flux vidéo DVR sans authentification

### Graylog
- **Nom** : Graylog
- **Version** : 5.2
- **CVE** :
  - **CVE-2024-24823**
    - Nom : Réutilisation de sessions après déconnexion
    - Score : 7.1
    - Descriptif : Sessions utilisateurs restent actives après déconnexion dans un cluster
  - **CVE-2024-24824**
    - Nom : Injection de classes via API
    - Score : 8.1
    - Descriptif : Chargement de classes arbitraires via API PUT sur configuration cluster

### SonarQube Community Edition
- **Nom** : SonarQube
- **Version** : 10.3
- **CVE** :
  - **Fuite de données encryptées**
    - Score : 6.5
    - Descriptif : URI encrypt exposant des données sensibles dans les journaux du serveur web

### Jenkins
- **Nom** : Jenkins
- **Version** : 2.452
- **CVE** :
  - **CVE-2024-43044**
    - Nom : Lecture de fichiers via connexions agents
    - Score : 8.8
    - Descriptif : Lecture non autorisée de fichiers sur serveur Jenkins à travers connexion agent
  - **CVE-2024-43045**
    - Nom : Accès aux vues utilisateurs
    - Score : 6.5
    - Descriptif : Accès non autorisé aux vues "Mes vues" d'autres utilisateurs par permission Overall/Read

