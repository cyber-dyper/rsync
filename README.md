# 🚀 RSYNC - Sauvegarde et Restauration Automatisées 🛠️

## 🎉 **Bienvenue sur ce nouveau projet !** 🎉

Tu apprendras ici à utiliser **rsync** pour automatiser tes **sauvegardes** et **restaurations** à travers un scénario réaliste et professionnel. 

---

## 🎯 **SCÉNARIO : Sauvegarde & Restauration** 

📦 **Objectif du projet :**
- Prendre en charge un projet de **sauvegarde** et **restauration** complet.
- Tester deux **stratégies de sauvegarde** différentes (**incrémentale** & **différentielle**).
- Automatiser les **sauvegardes** sur tous les systèmes, puis les centraliser sur un **serveur de sauvegarde dédié**.
- Maintenir la **restauration manuelle**, uniquement depuis les systèmes clients.
- Assurer une **traçabilité complète** avec horodatage et commentaires pour chaque action.

---

## 🏗️ **TON INFRASTRUCTURE :**

🖥️ **1 serveur de sauvegarde** 🛡️

💻 **5 systèmes à sauvegarder :**
- 🌐 **Serveur web**
- 📂 **Serveur de fichiers**
- 📧 **Serveur de mails**
- 👥 **Serveur RH**
- 💼 **Serveur IT**

---

## 🧠 **STRATÉGIE 1 : Sauvegarde INCRÉMENTALE** 

### 💾 **Sauvegarde :** 

- Sauvegarder uniquement les **données de même nature** liées à chaque **machine virtuelle**.
- Conserver la version **N du jour** et **N-1 de la veille** pour chaque dossier et fichier.
- Limiter la rétention des anciennes sauvegardes à un nombre de jours défini.
- Gérer de manière optimale l'espace de stockage tout en offrant une **historique de versions** suffisant.

### 🔄 **Restauration :** 

- Permettre aux utilisateurs de restaurer la version **N** ou **N-1** de l'ensemble de leurs documents.
- Assurer une restauration **rapide** et **intuitive**.

---

## 💡 **STRATÉGIE 2 : Sauvegarde DIFFÉRENTIELLE** 

### 💽 **Sauvegarde :** 

- Sauvegarder quotidiennement l'intégralité des **machines virtuelles**, incluant systèmes et données.
- Utiliser une **sauvegarde différentielle** pour réduire le volume des données transférées quotidiennement.
- Planifier les sauvegardes à une **heure stratégique**, évitant toute perturbation du travail des collaborateurs.
- Mettre en place une **reprise automatique** des sauvegardes en cas d'interruption, jusqu'à leur achèvement complet.

### 🛠️ **Restauration :** 

- Offrir la possibilité de restaurer **l'intégralité du système** à partir de la **dernière sauvegarde complète** disponible.
- Simplifier le processus pour garantir une remise en production rapide en cas de panne.

---

## 📦 **LIVRABLES : Ce que tu dois fournir** 

### 📜 **1. Scripts de Sauvegarde & Restauration Incrémentale** 
- Automatisation complète de la stratégie **incrémentale**.
- Scripts documentés avec commentaires clairs sur chaque étape.

### 📑 **2. Scripts de Sauvegarde & Restauration Différentielle** 
- Mise en œuvre de la stratégie **différentielle**, avec gestion des volumes de données.
- Scripts optimisés pour minimiser l'impact sur la bande passante et le temps d'arrêt.

### ⏰ **3. Configuration du Planificateur de Tâches** 
- Paramétrage du planificateur de tâches pour automatiser les sauvegardes à des moments clés.
- Assurer que chaque tâche est bien enregistrée et facilement maintenable.

### 📝 **4. Fichiers de Traces** 
- Génération de **logs détaillés** pour chaque opération de sauvegarde et restauration.
- Inclure des **horodatages**, des **statuts de réussite/échec** et des **commentaires personnalisés**.

---

## 💪 **Prêt à automatiser tes sauvegardes comme un pro ?** 🚀
N'oublie pas de t'amuser tout en sécurisant tes données ! 😉
