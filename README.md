# 🐧 Linux-SysAdmin-Notes

**Préparation intensive à l'entrée en BTS Cybersécurité (Rentrée Septembre)**

Bienvenue sur ce dépôt ! Ce projet regroupe mes notes, mes recherches et mes tests pratiques sur l'administration système Linux. J'ai décidé de commencer mon apprentissage en amont de ma formation pour construire une base technique solide en monitoring et gestion système.

## 🎯 Objectif

Maîtriser la gestion des ressources système, l'analyse des processus et l'administration du stockage pour mieux comprendre les vecteurs d'attaque et les méthodes de défense en cybersécurité.

---

## 📚 Journal d'Apprentissage

### 🟦 Jour 1 : Monitoring et État du Système
_Objectif : Comprendre comment observer et analyser l'état d'un serveur Linux._

**Outils étudiés :** `top`, `htop`, `ps`

**Points clés maîtrisés :**
* **Analyse des Processus :**
    * `PID` / `PPID` : Identification du processus et de son parent.
    * `STAT` (États) : `R` (Running), `S` (Sleeping), `Z` (Zombie).
    * `NI` (Nice) : Ajustement de la priorité CPU (de -20 à 19).
* **Gestion de la Mémoire :**
    * `VIRT` (Virtual) : Mémoire totale adressée.
    * `RES` (Resident) : Mémoire physique réellement utilisée.
    * `SHR` (Shared) : Mémoire partagée entre plusieurs processus.

* * *

### 🟩 Jour 2 : Cycle de vie et Contrôle des Processus
_Objectif : Maîtriser l'interaction avec les processus et la gestion des signaux._

**Outils étudiés :** `kill`, `pkill`, `killall`

**Points clés maîtrisés :**
* **Gestion des Signaux :**
    * `SIGTERM` (Signal 15) : Fermeture propre (sauvegarde des données).
    * `SIGKILL` (Signal 9) : Arrêt brutal via le noyau (en cas de blocage).
    * `SIGHUP` (Signal 1) : Rechargement de la configuration d'un service.
* **Concepts Avancés :**
    * **Processus Orphelins :** Adoption automatique par `init` ou `systemd` (PID 1).
    * **Foreground vs Background :** Gestion des tâches avec `&`, `fg` et `bg`.
    * **Threads vs Processus :** Différence entre isolation complète et unités d'exécution partagées.

* * *

### 🟧 Jour 3 : Stockage, Mémoire Swap et Performance I/O
_Objectif : Administrer l'espace disque et optimiser les entrées/sorties._

**Outils étudiés :** `df`, `free`, `iostat`

**Points clés maîtrisés :**
* **Gestion du Stockage :**
    * Analyse des partitions et points de montage via `df -h`.
    * Rôle de la **Mémoire Swap** pour pallier la saturation de la RAM.
    * Optimisation via les **Buffers** (écriture) et le **Cache** (lecture).
* **Monitoring des Performances :**
    * Surveillance des **TPS** (Transferts par seconde).
    * Analyse des vitesses de lecture/écriture (`kb_read` / `kb_wrt`).

* * *

## 🛠️ Environnement de test

* **OS :** Ubuntu
* **Outils :** Bash, htop, ps, kill, df, free, iostat.

## ✉️ Contact & Recherche de Stage

Je commence mon **BTS Cybersécurité à distance en septembre**. Très passionné par la sécurité offensive et défensive, je suis déjà en recherche active d'un stage pour mettre en pratique mes compétences et accompagner une entreprise dans sa stratégie de sécurité.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)]([https://www.linkedin.com/in/brice-uhri-916a99366/](https://www.linkedin.com/in/buhri-916a99366/?isSelfProfile=true))
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:uhri.brice@gmail.com)

---
_Note : Ce dépôt est une base de connaissances évolutive que je continue d'enrichir chaque jour._
