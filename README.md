# 🚀 **Défi DevOps en 7 Jours : De Zéro à l'Automatisation CI/CD sur AWS**  
**Déployez une application Java avec EC2, GitHub et les Outils AWS**  

---

## 🌟 **Aperçu du Projet**  
Ce défi vous guide pas à pas dans la création d'un **pipeline CI/CD complet** pour une application web Java, en utilisant les services AWS. En 7 jours, vous automatiserez tout, du commit de code au déploiement en production !  

**Outils Clés Utilisés** :  
- **AWS** : EC2, CodeArtifact, CodeBuild, CodeDeploy, CloudFormation, CodePipeline  
- **DevOps** : Git/GitHub, Apache Maven, VSCode en Remote-SSH  
- **Infrastructure as Code (IaC)** : Templates CloudFormation  

---

## 🎯 **Pourquoi ce Projet ?**  
- ✅ **Montez en compétences DevOps** : Maîtrisez l'intégration continue, le déploiement automatisé et l'IaC.  
- ✅ **Boostez votre portfolio** : Ajoutez un projet concret avec AWS, très demandé par les recruteurs.  
- ✅ **100% Pratique** : Chaque jour, un livrable opérationnel à partager.  

---

## 🛠️ **Prérequis**  
Avant de commencer :  
1. Un [Compte AWS](https://aws.amazon.com/fr/) (Éligible au Free Tier)  
2. [VSCode](https://code.visualstudio.com/) installé localement  
3. Bases en ligne de commande Linux  
4. Un [Compte GitHub](https://github.com/)  

---

## 🗓️ **Guide Jour par Jour**  

### **Jour 1 : Déployez l'Application sur EC2**  
**Objectif** : Héberger une app Java sur AWS EC2 et se connecter via VSCode.  
**Étapes** :  
1. Lancez une instance EC2 (Amazon Linux 2023).  
2. Installez VSCode + l'extension Remote-SSH.  
3. Connectez-vous à EC2 via SSH :  
   ```bash  
   ssh -i ~/chemin/vers/ma-clé.pem ec2-user@<ip-publique>  

   Installez Java (Corretto 8) et Maven :
   sudo dnf install -y java-1.8.0-amazon-corretto-devel  
wget https://archive.apache.org/dist/maven/maven-3/3.5.2/binaries/apache-maven-3.5.2-bin.tar.gz  

Jour 2 : Synchronisez avec GitHub
Objectif : Versionnez votre code avec Git/GitHub.
Étapes :

Installez Git sur EC2 :

bash
Copy
sudo dnf install git -y  
Créez un dépôt GitHub et liez-le :

bash
Copy
git init  
git remote add origin https://github.com/<votre-utilisateur>/<nom-depot>.git  
Poussez le code :

bash
Copy
git add . && git commit -m "Commit initial"  
git push -u origin main  
(Voir le Guide Complet pour les Jours 3 à 7)

📐 Architecture Technique
mermaid
Copy
graph TD  
    A[GitHub] --> B[AWS CodePipeline]  
    B --> C[CodeBuild]  
    C --> D[CodeDeploy]  
    D --> E[Instances EC2]  
    E --> F[CloudFormation]  
💡 Bonnes Pratiques
🔒 Sécurité : Utilisez des rôles IAM, restreignez l'accès SSH.

📝 Documentation : Maintenez un README à jour et un journal de bord.

🔄 Tests : Automatisez les tests avant chaque déploiement.

 Besoin d'Aide ?
Bloqué sur une étape ? Contactez-moi ! Je suis là pour vous aider :

📧 Email : Gorysow20@gmail.com

💼 LinkedIn : https://www.linkedin.com/in/gorysow/

🐙 GitHub : https://github.com/Gory20

❓ FAQ
Q : Pourquoi Git ne détecte pas mes modifications ?
R : Vérifiez les règles .gitignore ou forcez l'ajout :

bash
Copy
git add -f chemin/vers/fichier.jsp  
Q : Comment réduire les coûts AWS ?
R : Utilisez des instances Spot, surveillez votre budget avec AWS Cost Explorer.

🤝 Contribuez !
Ce projet est open source ! Pour contribuer :

Forkez le dépôt

Créez une branche :

bash
Copy
git checkout -b fonctionnalite/votre-idee  
Soumettez une Pull Request

🚀 Réalisé avec passion par Gory Sow | GitHub

