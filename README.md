# RSYNC
Appreneez à utiliser rsync pour vos backups avec le scénario suivant.

## **SCENARIO :**
- Prendre en charge un projet de sauvegarde et restauration.
- L’objectif du projet consiste à tester deux stratégies différentes (1 & 2).
- Les sauvegardes doivent s'executer automatiquement depuis chaque système et être ensuite centraliser sur le serveur de sauvegarde dédié.
- Les restaurations doivent s'executer manuellement uniquement et depuis les systèmes.
- Chaque action doit être tracée, horodatée et commentée.



## **TON INFRASTRUCTURE :**
- 1 serveur de sauvegarde et 5 systèmes à sauvegarder : web, fichiers, emails, RH et IT.



## **STRATÉGIE 1 : INCREMENTALE**
### Sauvegarde
- La première stratégie consiste à sauvegarder les données de même nature et donc relatives à chaque machine virtuelle. Conserve la version N du jour et N-1 de la veille de chaque élément arborescence (dossiers et fichiers). Conserve chaque ancienne sauvegarde pour un nombre de jour maximum.
### Restauration
- Les utilisateurs doivent pouvoir restaurer la version N ou N-1 de l'ensemble de leur documents.

## **STRATÉGIE 2 : DIFFERENTIELLE**
### Sauvegarde 
- La seconde stratégie consiste à sauvegarder quotidiennement les systèmes et donc machines virtuelles entière ce qui veut dire beaucoup de volume, d'où la sauvegarde différée. Choisi une heure stratégique pour qu'elles soient planifiées de manière à ne pas perturber le travail des collaborateurs. Si la sauvegarde est intérrompue, prévoie sa reprise lors de la sauvegarde suivante jusqu'à ce qu'elle soit totalement transférée.
### Restauration 
- Les utilisateurs doivent pouvoir restaurer la seule sauvegarde du système entier de la veille si terminée.



## **LIVRABLES :**
### Rassembler les scripts
1. Des sauvegardes et restaurations incrémentales
2. Des sauvegardes et restaurations différentielles
3. La configuration du planificateur de tâches
4. Des fichiers de traces

