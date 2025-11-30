# 📋 Procédure de Restauration de Fichiers d'un Serveur avec Veeam Backup & Replication

## 🔓 Étape 1 : Accès à la Console Veeam

1. Ouvrez le menu Démarrer de Windows
2. Accédez à "Apps" (Applications) → "Veeam"
3. Cliquez sur "Veeam Backup & Replication Console"
4. Attendez le chargement complet de l'interface

## 🔍 Étape 2 : Localiser la Sauvegarde du Serveur

1. Dans le volet gauche de la console, cliquez sur "Backups" (Sauvegardes)
2. Vérifiez que vous voyez votre serveur dans la liste des sauvegardes
3. Si le serveur n'est pas visible, assurez-vous que la sauvegarde a été complétée

## ⏱️ Étape 3 : Sélection du Point de Récupération

1. Développez la sauvegarde de votre serveur en cliquant sur la flèche à côté du nom
2. Vous verrez une liste de points de récupération (snapshots) avec leurs dates et heures
3. Sélectionnez le point de récupération à partir duquel vous souhaitez restaurer les fichiers
4. Généralement, choisissez le plus récent avant la perte de données

## 🗂️ Étape 4 : Accès à l'Explorateur de Fichiers Veeam

1. Cliquez droit sur le point de récupération sélectionné
2. Sélectionnez "Restore files..." (Restaurer des fichiers...)
3. Une nouvelle fenêtre s'ouvrira avec l'explorateur de fichiers

## 🔐 Étape 5 : Authentification (si nécessaire)

1. Vous pouvez être invité à fournir les identifiants de connexion du serveur
2. Entrez le nom d'utilisateur et le mot de passe administrateur du serveur
3. Cliquez sur "OK" pour vous connecter

## 📁 Étape 6 : Navigation dans le Système de Fichiers

1. L'explorateur Veeam affiche la structure complète du serveur sauvegardé
2. Naviguez jusqu'au dossier contenant les fichiers à restaurer
3. Vous pouvez explorer les lecteurs (C:, D:, etc.) et tous les dossiers
4. Utilisez les icônes de navigation pour vous déplacer dans l'arborescence

## ✅ Étape 7 : Sélection des Fichiers à Restaurer

1. Localisez le ou les fichiers que vous souhaitez restaurer
2. Pour un seul fichier : cliquez sur le fichier pour le sélectionner
3. Pour plusieurs fichiers : utilisez Ctrl+Clic pour une sélection multiple
4. Pour sélectionner tous les fichiers d'un dossier : utilisez Ctrl+A

## 🔎 Étape 8 : Vérification de la Sélection

1. Les fichiers sélectionnés seront mis en surbrillance
2. Vérifiez que vous avez sélectionné tous les fichiers nécessaires
3. Assurez-vous de ne pas avoir sélectionné accidentellement d'autres fichiers

## 🚀 Étape 9 : Lancement de la Restauration

1. Cliquez sur le bouton "Restore" (Restaurer) ou "Next" (Suivant)
2. Une fenêtre de dialogue s'ouvrira pour confirmer les options de restauration
3. Vérifiez les détails de la restauration

## 📍 Étape 10 : Choix de la Destination de Restauration

Option A - Restaurer à l'emplacement d'origine :
1. Sélectionnez "Restore to original location" (Restaurer à l'emplacement d'origine)
2. Cela va restaurer les fichiers à leur emplacement initial sur le serveur

Option B - Restaurer à un emplacement différent :
1. Sélectionnez "Restore to alternate location" (Restaurer à un autre emplacement)
2. Cliquez sur "Browse" (Parcourir)
3. Sélectionnez le dossier de destination
4. Cliquez sur "OK" pour confirmer

## ⚙️ Étape 11 : Configuration des Options de Restauration

1. Décidez comment gérer les fichiers existants :
   - "Overwrite existing files" (Remplacer les fichiers existants)
   - "Skip existing files" (Ignorer les fichiers existants)
   - "Rename restored files" (Renommer les fichiers restaurés)

2. Définissez les permissions de fichier si nécessaire

3. Cochez les options supplémentaires si nécessaire

## 🎯 Étape 12 : Vérification Finale avant Restauration

1. Vérifiez à nouveau les paramètres de restauration :
   - Les fichiers sélectionnés
   - L'emplacement de destination
   - Les options de remplacement
   - L'espace disque disponible

2. Cliquez sur "Restore" (Restaurer) ou "Finish" (Terminer) pour démarrer

## 📊 Étape 13 : Suivi du Processus de Restauration

1. Une fenêtre de progression s'affichera
2. Vous verrez un pourcentage d'avancement et la vitesse de transfert
3. Ne fermez pas la fenêtre tant que la restauration n'est pas terminée
4. Attendez le message de completion

## ✔️ Étape 14 : Vérification du Statut de Restauration

1. Une fois terminée, vous verrez un message "Restore completed successfully" (Restauration terminée avec succès)
2. Le journal de restauration montrera tous les fichiers restaurés
3. Vérifiez qu'aucune erreur n'est signalée

## 🚪 Étape 15 : Fermeture de l'Explorateur Veeam

1. Cliquez sur "Close" (Fermer) ou "OK" pour fermer la fenêtre
2. Vous reviendrez à la console principale de Veeam

## 🎉 Étape 16 : Vérification des Fichiers Restaurés

1. Ouvrez l'Explorateur Windows ou accédez directement au serveur
2. Naviguez vers le dossier de destination
3. Vérifiez que tous les fichiers ont été restaurés correctement
4. Vérifiez l'intégrité des fichiers si nécessaire
5. Assurez-vous que les droits d'accès sont corrects

---

## 🚀 Options Avancées de Restauration

### ☁️ Restauration à partir d'une Sauvegarde Sécurisée dans le Cloud

1. Si votre sauvegarde est stockée dans le cloud, Veeam téléchargera les données automatiquement
2. Assurez-vous d'avoir une connexion Internet stable
3. Le processus peut prendre plus de temps selon la taille des fichiers

### 🔄 Restauration de Fichiers Supprimés

1. Utilisez la fonction "FLR" (File Level Recovery) pour accéder aux anciennes versions de fichiers
2. Les points de récupération précédents contiennent les versions antérieures des fichiers
3. Sélectionnez le point de récupération avant la suppression

### 🛡️ Restauration en Cas de Corruption

1. Utilisez un point de récupération antérieur à la corruption
2. Choisissez "Restore to alternate location" pour ne pas écraser les fichiers existants
3. Vérifiez l'intégrité des fichiers après la restauration

---

## 🔧 Dépannage Courant

### ❌ Les fichiers ne s'affichent pas dans l'explorateur Veeam
- Vérifiez que le point de récupération est valide
- Vérifiez que vous avez les permissions nécessaires
- Essayez de sélectionner un autre point de récupération

### 🔐 Erreur d'authentification lors de la connexion
- Vérifiez que le nom d'utilisateur et le mot de passe sont corrects
- Assurez-vous que le compte a les droits administrateur
- Vérifiez que le serveur est accessible sur le réseau

### 💾 Erreur "Insufficient disk space" (Espace disque insuffisant)
- Vérifiez l'espace disponible sur le disque de destination
- Libérez de l'espace disque avant de continuer
- Essayez de restaurer vers un autre disque ou partage réseau

### ⚡ La restauration est très lente
- Vérifiez la bande passante réseau disponible
- Réduisez le nombre de fichiers à restaurer
- Essayez de restaurer à un moment moins chargé

---

## 💡 Points Importants à Retenir

- ⏱️ **Points de récupération** : Plus il y a de points de récupération, plus de choix vous avez pour restaurer
- 🧪 **Test de restauration** : Testez régulièrement vos restaurations pour vérifier l'intégrité des sauvegardes
- 💿 **Destination** : Assurez-vous toujours d'avoir suffisamment d'espace disque à la destination
- 🔑 **Permissions** : Vérifiez les permissions des fichiers restaurés après la restauration
- 📝 **Logs** : Conservez les journaux de restauration pour l'audit et le dépannage

---

## 📚 Ressources Utiles

- 🌐 **Centre d'aide Veeam** : https://helpcenter.veeam.com
- 🔍 **Explorateur de fichiers Veeam** : https://helpcenter.veeam.com/docs/backup/vsphere/file_level_recovery.html
- 💬 **Support Veeam** : https://www.veeam.com/support
