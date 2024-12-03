
# TD 1 : Atelier Pratique - Plan de Sécurité pour SECURBANK

### Groupe :
- **Mehdi**
- **Charles**
- **Vicenzo**
- **Charly**

## Contexte
Vous êtes en charge de définir un plan de sécurité pour **SECURBANK**, une banque traditionnelle développant une plateforme bancaire en ligne. Ce projet doit répondre aux contraintes réglementaires et intégrer la sécurité tout au long du cycle de développement.

### Détails du projet
- **Clientèle attendue** : 100 000 clients la première année.
- **Budget** : 2 millions d'euros.
- **Délai** : 12 mois.
- **Équipe projet** : 20 développeurs, 5 ops, 2 experts sécurité.

### Fonctionnalités clés
1. Création de compte en ligne avec vérification KYC (Know Your Customer).
2. Virements nationaux et internationaux.
3. Gestion des cartes bancaires.
4. Développement d’une application mobile.
5. API pour partenaires externes.

### Contraintes réglementaires
- **RGPD** : Gestion des données personnelles.
- **DSP2** : Authentification forte et sécurité des transactions.
- **Réglementation bancaire spécifique**.

---

## Travail Réalisé

### 1. Phases Critiques

#### **Training**
- **Risques** : Manque de sensibilisation à la sécurité chez les développeurs et ops.
- **Contrôles** :
  - Formation obligatoire sur les principes OWASP et RGPD.
  - Certification des compétences en sécurité.
- **Livrables** :
  - Attestations de formation.
  - Documentation des compétences acquises.

#### **Requirements**
- **Risques** : Absence de définition claire des exigences de sécurité.
- **Contrôles** :
  - Analyse des risques via des modèles comme STRIDE.
  - Définition des métriques de sécurité conformes aux réglementations RGPD et DSP2.
- **Livrables** :
  - Liste des exigences de sécurité.
  - Matrice de conformité.

#### **Design**
- **Risques** : Architecture logicielle vulnérable à des failles de type injection ou XSS.
- **Contrôles** :
  - Application des principes de **Secure by Design**.
  - Revue d’architecture pour valider les zones critiques.
- **Livrables** :
  - Diagrammes de flux de données.
  - Modèles de menaces identifiés.

#### **Implementation**
- **Risques** : Introduction de failles de sécurité dans le code (ex. : injection SQL).
- **Contrôles** :
  - Validation des entrées utilisateur.
  - Utilisation de bibliothèques sécurisées et analyse statique du code.
- **Livrables** :
  - Rapport des analyses de sécurité du code.
  - Code source documenté et conforme.

#### **Verification**
- **Risques** : Vulnérabilités non détectées avant le déploiement.
- **Contrôles** :
  - Tests de pénétration.
  - Automatisation des scans de vulnérabilités.
- **Livrables** :
  - Rapport des tests.
  - Liste des corrections apportées.

#### **Release**
- **Risques** : Configurations non sécurisées en production.
- **Contrôles** :
  - Revue de sécurité finale.
  - Mise en place d’un plan de réponse aux incidents.
- **Livrables** :
  - Checklist de sécurité de la release.
  - Procédure de déploiement.

#### **Response**
- **Risques** : Absence de détection rapide des incidents.
- **Contrôles** :
  - Surveillance continue avec un SIEM.
  - Formation des équipes sur la gestion des incidents.
- **Livrables** :
  - Rapports d’incidents.
  - Journaux d’audit centralisés.

---

### 2. Risques Majeurs

#### **Risque 1 : Fuite de données clients**
- **Impact** : Perte de confiance, amendes RGPD, atteinte à la réputation.
- **Probabilité** : Moyenne.
- **Mesures de mitigation** :
  - Chiffrement des données sensibles (AES-256).
  - Mise en place de contrôles d'accès stricts (RBAC).

#### **Risque 2 : Compromission des API partenaires**
- **Impact** : Escalade d’attaques vers d’autres systèmes.
- **Probabilité** : Haute.
- **Mesures de mitigation** :
  - Authentification forte avec OAuth 2.0.
  - Limitation des appels via des quotas et journaux.

#### **Risque 3 : Attaques par déni de service (DDoS)**
- **Impact** : Indisponibilité des services, pertes financières.
- **Probabilité** : Moyenne.
- **Mesures de mitigation** :
  - Utilisation d’un CDN pour absorber les attaques.
  - Détection et blocage automatisé des IP malveillantes.

---

### 3. Indicateurs de Performance (KPIs)

#### **KPI 1 : Temps moyen de détection d’un incident**
- **Définition** : Temps écoulé entre le déclenchement de l’incident et sa détection.
- **Cible** : Moins de 10 minutes.
- **Mesure** : Analyse des journaux et alertes SIEM.

#### **KPI 2 : Taux de correction des vulnérabilités détectées**
- **Définition** : Pourcentage de vulnérabilités corrigées dans les délais.
- **Cible** : 95% dans un délai de 15 jours.
- **Mesure** : Suivi des rapports de tests et des tickets.

#### **KPI 3 : Disponibilité des services**
- **Définition** : Pourcentage de disponibilité des services pour les utilisateurs finaux.
- **Cible** : 99,9%.
- **Mesure** : Monitoring des services et calcul de l’Uptime.

---
