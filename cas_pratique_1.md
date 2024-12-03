
# Cas Pratique 1 : Application de Gestion RH avec SDL

### Groupe :
- **Mehdi**
- **Charles**
- **Vicenzo**
- **Charly**

## Contexte
Une entreprise développe une application de gestion RH qui doit respecter plusieurs exigences sécuritaires :
- **Données personnelles sensibles** : Gestion des identités, coordonnées, contrats de travail, etc.
- **Accès multi-niveaux** : Utilisateurs ayant des rôles distincts (RH, employés, managers) avec des permissions adaptées.
- **Interface web** : Accès via un navigateur nécessitant une attention particulière pour prévenir les vulnérabilités (XSS, injections SQL).
- **Base de données centralisée** : Centralisation des données nécessitant une sécurité robuste contre les fuites et accès non autorisés.

---

## Phases SDL Critiques et Actions Associées

### 1. **Planification (Requirements)**
- Identifier les **réglementations applicables** telles que le RGPD (GDPR).
- Réaliser une **analyse des risques** pour chaque fonctionnalité sensible.
- Élaborer un **plan de réponse aux incidents** pour garantir une gestion rapide des brèches de sécurité.

### 2. **Conception (Design)**
- **RBAC (Role-Based Access Control)** : Définir un modèle de gestion des permissions pour restreindre les accès selon les rôles.
- **Segmentation des données sensibles** : Isoler les données critiques dans des sous-systèmes sécurisés.
- Intégrer des **mécanismes d'authentification forts**, comme le MFA (authentification multi-facteurs) et la gestion des sessions.

### 3. **Implémentation**
- Former les développeurs aux **principes OWASP** et aux bonnes pratiques de codage sécurisé.
- Utiliser des **bibliothèques standardisées** pour le chiffrement des données (AES pour les données au repos, TLS pour les données en transit).
- Effectuer des **revues de code** régulières pour identifier et corriger les vulnérabilités.

### 4. **Validation (Vérification et Tests)**
- Réaliser des **tests de pénétration** (pentests) pour simuler des attaques réelles.
- Intégrer des **scans automatisés de sécurité** dans les pipelines CI/CD.
- Documenter toutes les corrections apportées dans un rapport dédié.

### 5. **Déploiement et Maintenance**
- Mettre en place une **surveillance continue** des journaux d'accès pour détecter les comportements anormaux.
- Effectuer des **mises à jour régulières** des bibliothèques, frameworks et composants tiers.
- Planifier des **tests récurrents en production** pour valider la sécurité.

---

## Livrables
| **Phase**         | **Livrables**                                                     |
|--------------------|-------------------------------------------------------------------|
| **Planification**  | Rapport d’analyse des risques, Liste des exigences de sécurité.  |
| **Conception**     | Diagrammes d’architecture, Spécifications des rôles et permissions (RBAC). |
| **Implémentation** | Code source conforme aux bonnes pratiques SDL, Rapport des outils d’analyse statique. |
| **Validation**     | Rapports des tests unitaires, intégration et pénétration.         |
| **Déploiement**    | Procédure de déploiement sécurisée, Stratégie de surveillance en production. |
