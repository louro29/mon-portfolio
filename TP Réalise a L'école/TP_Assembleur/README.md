# 💻 TD - Initiation au langage Assembleur avec le simulateur LittleThinker

## 🧠 Objectif pédagogique du Lab

Ce travail dirigé a pour but d'introduire les étudiants au **langage assembleur** à travers l'utilisation d'un **simulateur de processeur** nommé *LittleThinker*. Il permet de comprendre la logique de bas niveau d’un processeur et la manière dont les instructions sont exécutées.


## 🎯 Objectifs pédagogiques — BTS SIO

| Bloc  | Compétence visée                                                                 |
|-------|-----------------------------------------------------------------------------------|
| B1.1  | Comprendre l’organisation interne d’un processeur et le rôle des registres       |
| B1.2  | Manipuler un langage bas niveau pour appréhender la logique machine              |
| B3.2  | Mettre en place un environnement de simulation et automatiser son exécution      |
| B4.1  | Diagnostiquer un dysfonctionnement par simulation d’instructions processeur      |

## 🖥️ Contexte technique

Le simulateur LittleThinker simule :
- Un **accumulateur** (registre de calcul)
- 5 **registres d’instructions** (#0 à #4)
- Un **compteur ordinal**
- Un **registre d’état** (Z = zéro, N = négatif)
- Une mémoire de 50 cases adressables par `$` ou indirectement par `$#numéro_registre`

