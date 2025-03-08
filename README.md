# MINI PROJET: Déploiement et configuration d’infrastructure pour production et environnement de test

## NOTE:

*Le projet en question, avec les fichiers Jenkinsfile, Dockerfile, test, app et requirements, est accessible* **[ICI](https://github.com/Zivan-R/ansible-deploy-f2-f4.git)**

---
## Technos:  
Microsoft Azure, Ansible, Git, GitHub, Jenkins, Docker, MySQL, Python, Pytest  
  
## PROCESS:
**1-** Création de deux VM (VM1 et VM2) sur Microsoft Azure et Installation de Ansible sur VM1  
**2-** Configuration des VM pour accès mutuel en SSH Passwordless  
**3-** Structuration de l’arborescence du projet selon les bonnes pratiques Ansible  
**4-** Écriture du fichier .sql pour la création et configuration de la base de données  
**5-** Import de l’application python + test  
**6-** Création de l’inventory et du playbook de configuration pour VM1 et VM2:  
- Sur VM1:  
  - Installation de Git  
  - Installation des dépendances Java (Open JDK 17)  
  - Installation de Jenkins  
	
- Sur VM2:  
  - Installation et configuration de MySQL  
  - Installation et configuration de Docker  
  - Installation de Python + ses dépendances  
  - Installation de pytest  
  - Installation d’Open JDK 17 (pour faire de VM2 l’Agent Jenkins)  
  - Création du dossier pour Jenkins (/home/jenkins)  
  - Configuration du schéma de la Database  

**7-** Versionning de l’application avec Git et Github  
**8-** Écriture du fichier Dockerfile pour créer une image docker de l’application  
**9-** Écriture du Jenkinsfile  
**10-** Création des credentials SSH dans Jenkins (accès 100% passwordless)  
**11-** Création et connexion de l’agent Jenkins (VM2)  
**12-** Application des bonnes pratiques Jenkins en assignant 0 exécuteurs au contrôleur  
**13-** Création et lancement de la pipeline production  
**14-** Création de l’environnement de test (branche test sur versionning)  
**15-** Création et lancement de la pipeline test  
