# Présentation de Cortex XDR

## Plateforme de détection et réponse étendue (XDR)

### Qu'est-ce que Cortex XDR ?

**Cortex XDR** de Palo Alto Networks est une solution de cybersécurité avancée  
qui unifie la protection des endpoints, la détection des menaces et la  
réponse aux incidents. Cette plateforme XDR (Extended Detection and Response)  
corrèle les données de sécurité provenant de multiples sources pour offrir  
une visibilité complète sur les menaces sophistiquées.

### Gestion centralisée des endpoints

L'interface principale de Cortex XDR présente une vue exhaustive de tous  
les endpoints de l'infrastructure avec **166 terminaux sur 189 résultats**.  
Chaque endpoint est répertorié avec ses informations critiques :

- **Nom de l'endpoint**
- **Type** (workstation/serveur)
- **Statut de connexion**
- **Système d'exploitation**
- **Version de l'agent**
- **Adresses IP**
- **Utilisateur associé**

### Surveillance d'état en temps réel

Le système affiche clairement le statut de connexion de chaque endpoint  
avec des **indicateurs visuels** :
- **Points verts** pour les terminaux connectés
- **Points rouges** pour ceux déconnectés

Cette visibilité immédiate permet aux équipes de sécurité d'identifier  
rapidement les gaps de couverture et les terminaux nécessitant une  
attention particulière.

### Diversité des environnements supportés

Cortex XDR protège une large gamme de systèmes d'exploitation :
- **Windows** (11, 10, 7, Server 2019)
- **macOS** (Sequoia)
- **Linux** (Ubuntu, Rocky Linux, Alma, Debian)

Cette couverture multiplateforme assure une protection homogène dans des  
environnements IT hétérogènes.

### Système de ticketing automatisé

**Fonctionnalité clé** : Lorsque l'antivirus Cortex XDR détecte une activité  
considérée comme inhabituelle ou suspecte, le système génère automatiquement  
un ticket d'incident.

Ces tickets sont centralisés dans une interface dédiée avec :
- **Identifiant unique** (SOC-xxxx)
- **Description détaillée** de l'incident
- **Responsable assigné**
- **Entreprise concernée**
- **Statut de traitement**

### Workflow de réponse aux incidents

Les tickets générés suivent un workflow structuré avec différents statuts :
- **Résolu**
- **Fermé**
- **En cours**

Chaque ticket inclut :
- Date de création
- Définition de l'incident
- Actions entreprises
- Traçabilité complète

### Classification et priorisation intelligente

Le système classe automatiquement les incidents selon :
- **Criticité**
- **Type d'incident**
- **Entreprise cliente** (ex: Griffine Industries)
- **Assignation** aux analystes appropriés
