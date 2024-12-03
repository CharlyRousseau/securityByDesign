
# Cas Pratique 2 : Évaluation de Maturité Sécuritaire avec BSIMM

### Groupe :
- **Mehdi**
- **Charles**
- **Vicenzo**
- **Charly**

## Contexte
Une organisation fictive souhaite évaluer la maturité de ses pratiques en sécurité logicielle à l'aide du modèle **BSIMM (Build Security In Maturity Model)**. Ce cadre propose une approche observationnelle basée sur les pratiques réelles d’entreprises matures.

---

## Domaines et Activités

### 1. **Gouvernance**
#### Objectif
Établir un cadre organisationnel pour gérer efficacement la sécurité.

#### Activités par Niveau
- **Niveau 1** : Définir des politiques basiques, comme la gestion des mots de passe.
- **Niveau 2** : Mettre en place des KPI pour suivre les incidents de sécurité.
- **Niveau 3** : Déployer un tableau de bord intégré pour surveiller les incidents en temps réel.

---

### 2. **SSDL Touchpoints (Secure Software Development Lifecycle)**
#### Objectif
Intégrer la sécurité dans toutes les phases du cycle de vie du développement logiciel.

#### Activités par Niveau
- **Niveau 1** : Réaliser des revues de code ponctuelles pour détecter les failles évidentes.
- **Niveau 2** : Intégrer des **tests de sécurité automatisés** dans les pipelines CI/CD.
- **Niveau 3** : Organiser des simulations d’attaques réalistes basées sur des menaces actuelles.

---

### 3. **Déploiement**
#### Objectif
Assurer la sécurité des applications en production.

#### Activités par Niveau
- **Niveau 1** : Maintenir un inventaire des systèmes et logiciels utilisés.
- **Niveau 2** : Mettre en place un processus de gestion des patchs pour les composants tiers.
- **Niveau 3** : Automatiser le déploiement des patchs à l’aide d’outils comme Chef ou WSUS.

---

## Évaluation et Recommandations
### Résultats Actuels
- Gouvernance : Niveau 2, avec des KPI mais un manque de visibilité en temps réel.
- SSDL Touchpoints : Niveau 1, absence de tests automatisés.
- Déploiement : Niveau 1, inventaire des systèmes présent mais patch management manuel.

### Recommandations
- **Gouvernance** : Déployer un tableau de bord intégré pour améliorer la visibilité en temps réel.
- **SSDL Touchpoints** : Intégrer des tests de sécurité automatisés dans les pipelines CI/CD.
- **Déploiement** : Automatiser la gestion des patchs pour réduire les délais et les erreurs humaines.
