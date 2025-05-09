# TP-EVARD

## 1. Source Code Management

### GitLab CE
- **Version** : 17.9.7
- **Éditeur** : GitLab B.V.
- **Origine** : Pays-Bas
- **Licence** : MIT
- **Lien éditeur** : [GitLab](https://about.gitlab.com/)
- **Dépendances** :
  - **Postgres**
    - Version : 17.3
    - Éditeur : PostgreSQL Global
    - Origine : Californie
    - Licence : PostgreSQL License
    - [Lien éditeur](https://postgresql.org)

#### Vulnérabilités (CVE) :
- **CVE-2025-2443** : XSS via Maven proxy cache headers (Score : 7.5)
  - Un attaquant peut injecter du code malveillant dans le navigateur via des en-têtes de cache, contournant les protections CSP.
- **CVE-2025-1908** : Suivi des activités de navigation (Score : 6.8)
  - Permet à un attaquant de suivre la navigation des utilisateurs et voler des sessions.
- **CVE-2025-0639** : Déni de service via aperçu des problèmes (Score : 6.5)
  - Exploitation de l'aperçu pour surcharger le serveur et le rendre indisponible.
- **CVE-2025-1677** : Déni de service via exportation CI (Score : 6.2)
  - Envoi de données lourdes lors d'un export CI provoquant un crash.

---

## 2. ITSM et collaboration

### GLPI
- **Version** : 10.0.18
- **Éditeur** : Teclib'
- **Origine** : France
- **Licence** : GPLv3
- **Lien éditeur** : [GLPI](https://glpi-project.org/)
- **Dépendances** :
  - **MariaDB**
    - Licence : GPLv2

#### Vulnérabilités (CVE) :
- **CVE-2025-25192** : Accès non autorisé au mode débogage (Score : 7.2)
  - Activation du mode debug par utilisateur à privilèges faibles révélant des infos sensibles.
- **CVE-2025-23046** : Accès non autorisé via OauthIMAP (Score : 7.1)
  - Authentification contournée via configuration incorrecte OAuth IMAP.
- **CVE-2025-24799** : Injection SQL avant authentification (Score : 9.8)
  - Injection SQL possible sans être connecté via point d'inventaire.
- **CVE-2025-24801** : Exécution de code post-authentification (Score : 8.7)
  - Exécution forcée de fichiers PHP après login sur GLPI.

---

## 3. Configuration Management

### Ansible
- **Version** : v2.17.11
- **Éditeur** : Red Hat
- **Origine** : USA
- **Licence** : GPLv3
- **Lien éditeur** : [Ansible](https://www.ansible.com/)

#### Vulnérabilités (CVE) :
- **CVE-2023-4237** : Fuite de clés privées dans les logs (Score : 7.5)
  - Clé privée EC2 accidentellement imprimée dans les logs standards.
- **CVE-2023-39059** : Exécution de code via variables additionnelles (Score : 8.6)
  - Injection et exécution de code distant via variables supplémentaires.

---

## 4. Deployment

### Argo CD
- **Version** : 2.11
- **Éditeur** : CNCF
- **Origine** : Monde
- **Licence** : Apache 2.0
- **Lien éditeur** : [Argo CD](https://argo-cd.readthedocs.io/)

- **Dépendances** :
  - **Kubernetes**
    - Version : 1.30
    - Éditeur : CNCF
    - Origine : Monde
    - Licence : Apache 2.0
    - [Lien éditeur](https://kubernetes.io/)

#### Vulnérabilités (CVE) :
- **CVE-2024-40634** : Déni de service via payload JSON massif (Score : 7.5)
  - JSON volumineux provoquant une saturation mémoire serveur et arrêt.
- **CVE-2024-37152** : Fuite de paramètres sensibles (Score : 7.2)
  - Paramètres exposés publiquement via API de configuration.
- **CVE-2024-45338** : Déni de service via parsing YAML (Score : 7.8)
  - YAML malformé ralentissant ou bloquant l'analyse.

---

## 5. Threat and Vulnerability Management

### OpenVAS
- **Version** : 22.4
- **Éditeur** : Greenbone Networks
- **Origine** : Allemagne
- **Licence** : GPLv2
- **Lien éditeur** : [OpenVAS](https://www.greenbone.net/)

- **Dépendances** :
  - **Postgres**
    - Version : 17.3
    - [Lien éditeur](https://postgresql.org)
  - **Redis**
    - Version : 7.2
    - Éditeur : Redis Ltd
    - Licence : BSD 3-Clause
    - [Lien éditeur](https://redis.io/)

#### Vulnérabilités (CVE) :
- **CVE-2018-9995** : Bypass authentification DVR (Score : 9.8)
  - Accès à des flux vidéo DVR sans authentification via faille d'authentification.

---

## 6. Logging & Monitoring

### Graylog
- **Version** : 5.2
- **Éditeur** : Graylog, Inc.
- **Origine** : Allemagne / USA
- **Licence** : GPLv3 (Community Edition)
- **Lien éditeur** : [Graylog](https://www.graylog.org/)

- **Dépendances** :
  - **MongoDB**
    - Version : 7.0
    - Éditeur : MongoDB, Inc.
    - Licence : SSPL
    - [Lien éditeur](https://www.mongodb.com/)
  - **Elasticsearch**
    - Version : 8.12
    - Éditeur : Elastic N.V.
    - Licence : Elastic License 2.0 / SSPL
    - [Lien éditeur](https://www.elastic.co/elasticsearch/)

#### Vulnérabilités (CVE) :
- **CVE-2024-24823** : Réutilisation de sessions après déconnexion (Score : 7.1)
  - Sessions non invalidées après déconnexion sur cluster multi-nœuds.
- **CVE-2024-24824** : Injection de classes via API (Score : 8.1)
  - Chargement de classes arbitraires via cluster_config API.

---

## 7. Quality / Testing

### SonarQube Community Edition
- **Version** : 10.3
- **Éditeur** : SonarSource
- **Origine** : Suisse (Europe)
- **Licence** : LGPLv3
- **Lien éditeur** : [SonarSource](https://www.sonarsource.com/)

- **Dépendances** :
  - **Postgres**
    - Version : 17.3
    - [Lien éditeur](https://postgresql.org)

#### Vulnérabilités :
- **CVE-2024-20721** : Expiration insuffisante des sessions (Score : 6.5)
  - Sessions non révoquées après changement de mot de passe, exposant des risques d'usurpation.

---

## 8. Build

### Jenkins
- **Version** : 2.452
- **Éditeur** : Jenkins Community (Continuous Delivery Foundation)
- **Origine** : USA
- **Licence** : MIT
- **Lien éditeur** : [Jenkins](https://www.jenkins.io/)

#### Vulnérabilités (CVE) :
- **CVE-2024-43044** : Lecture de fichiers via connexions agents (Score : 8.8)
  - Accès à des fichiers sensibles du serveur via connexions agents compromis.
- **CVE-2024-43045** : Accès aux vues utilisateurs (Score : 6.5)
  - Utilisateurs faibles peuvent accéder aux vues "Mes Vues" d'autres comptes utilisateurs.
