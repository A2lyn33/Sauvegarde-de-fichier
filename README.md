# 🛡️ Mise en place de la sauvegarde du volume de partage de fichiers

## 📋 Prérequis

- Disque dur supplémentaire non formaté pour la sauvegarde du volume

## ⚙️ Installer le rôle de Serveur Backup

1. Sélectionner `Manage` --> `Add Roles and features`
2. Sélectionner les paramètres de votre serveur, puis cocher la case `Windows Server Backup`

![Ajouter les rôles et fonctionnalités](https://github.com/WildCodeSchool/TSSR-2402-P3-G3-BuildYourInfra-Ekoloclast/blob/main/S13/BackupInstall%20Capture/role%20serveur.png)

3. Sélectionner `Next` puis `Finish`

## 💾 Créer la partition qui accueillera la sauvegarde

1. Sélectionner `Tools` --> `Computer Management`
2. Sélectionner `Disk Management`

![Gestion des disques](https://github.com/WildCodeSchool/TSSR-2402-P3-G3-BuildYourInfra-Ekoloclast/blob/main/S13/BackupInstall%20Capture/partition.png)

3. Clic droit sur le nouveau disque puis sélectionner `Initialize`
4. Clic droit sur le nouveau disque puis sur nouvelle partition, laisser les paramètres par défaut jusqu'au choix de la lettre
5. Choisir un nom de label puis terminer

## ⏲️ Créer la planification de sauvegarde

1. Sur le Server Manager, sélectionner `Tools` --> `Windows Server Backup`
2. Sélectionner `Backup Schedule Wizard`
3. Sélectionner `Custom`
4. Sélectionner `Add Items` puis sélectionner le lecteur à sauvegarder
5. Paramétrer les options selon votre choix
6. Sélectionner `Back up to a volume`
7. Sélectionner `Add Items` puis sélectionner le lecteur où seront sauvegardées les données
8. Sélectionner `Keep the volume destination` puis terminer

![Planification de sauvegarde](https://github.com/WildCodeSchool/TSSR-2402-P3-G3-BuildYourInfra-Ekoloclast/blob/main/S13/BackupInstall%20Capture/backup%20confir.png)
