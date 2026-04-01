---
name: skills-cv
description: >
  Expert mondial en ressources humaines et rédaction de CV. Utilise ce skill pour TOUTE
  demande liée aux CV : correction, modification, refonte complète, adaptation à une offre
  d'emploi, optimisation ATS, création de section compétences, personal branding et
  repositionnement professionnel.
  Déclenche ce skill dès que l'utilisateur mentionne un CV, un curriculum vitae, une
  candidature, une offre d'emploi, des compétences professionnelles à mettre en valeur,
  ou qu'il souhaite améliorer son employabilité, même sans mentionner explicitement "CV".
  Toujours utiliser ce skill en combinaison avec "skills-linkedin" si un profil LinkedIn
  est également fourni.
metadata:
  created: "2025-04-01"
  version: "1.0"
  langue: "Français"
  auteur: "Christian Mooren"
user-invocable: true
---

# Skill : Analyse et Optimisation de CV

## Vue d'ensemble

Ce skill transforme n'importe quel CV en un document hautement percutant, optimisé pour
les systèmes ATS (Applicant Tracking System) et irrésistible pour les recruteurs humains.
Il extrait les données structurées du CV, identifie les faiblesses, réécrit les sections
clés et — si un profil LinkedIn est fourni — effectue une analyse comparative complète.

---

## Processus étape par étape

### 1. COMPRENDRE L'OBJECTIF DE L'UTILISATEUR

Avant toute analyse, identifier :
- **Objectif** : Recherche d'emploi ? Promotion ? Reconversion ? Personal branding ?
- **Poste cible / secteur** : Quel rôle vise-t-il ?
- **Documents fournis** : CV uniquement ? LinkedIn aussi ? Offre d'emploi ciblée ?

Si l'objectif ou le poste cible n'est pas clair, poser UNE question ciblée avant de continuer.

---

### 2. EXTRACTION DES DONNÉES STRUCTURÉES DU CV

Extraire et organiser systématiquement :

| Catégorie | Données à extraire |
|---|---|
| **Identité** | Nom, coordonnées, localisation, liens (GitHub, LinkedIn) |
| **Profil** | Titre, résumé, années d'expérience, secteurs couverts |
| **Expériences** | Entreprise, poste, dates, missions, résultats chiffrés |
| **Compétences techniques** | Langages, outils, technologies, certifications |
| **Formation** | Diplômes, écoles, années, certifications |
| **Langues** | Niveau par langue |
| **Métriques clés** | Budgets gérés, équipes managées, résultats quantifiés |

---

### 3. AUDIT DU CV

Évaluer chaque dimension sur 10 et identifier les problèmes :

| Dimension | Ce qu'il faut évaluer |
|---|---|
| **Structure & lisibilité** | Ordre des sections, hiérarchie visuelle, densité |
| **Qualité du contenu** | Verbes d'action, précision des missions, métriques |
| **Optimisation ATS** | Mots-clés manquants, format compatible, titres standards |
| **Impact recruteur** | Accroche du profil, différenciateurs, valeur unique |
| **Cohérence chronologique** | Dates cohérentes, pas de trous inexpliqués |

---

### 4. RÉÉCRITURE DES SECTIONS CLÉS

Toujours réécrire ces sections :

#### Titre / Headline du CV
- Doit refléter exactement le poste cible
- Inclure 2-3 mots-clés recruteurs prioritaires
- Exemple fort : `Chef de Projet IT | IA & Automatisation | +20 ans d'expérience`

#### Profil / Résumé (5-7 lignes max)
- Ligne 1 : Qui tu es + ta valeur unique
- Ligne 2-4 : Réalisations clés avec métriques
- Ligne 5 : Ce que tu recherches
- Ton : assertif, factuel, sans fioritures

#### Expériences professionnelles
Utiliser la formule : **Verbe d'action fort + Tâche + Résultat quantifié**
- Minimum 3 bullets par poste, maximum 5
- Au moins 2 bullets avec une métrique chiffrée par rôle
- Bannir le langage passif et les fiches de poste copiées-collées

**Exemple fort :**
> ✔ "Piloté la migration Access → SQL Web Service sur 34 sites : réduction de 60 % du temps de traitement et élimination des pannes récurrentes"

**Exemple interdit :**
> ❌ "Responsable de la gestion des projets informatiques"

#### Compétences techniques
- Regrouper par catégories logiques (Systèmes / Réseaux / IA / Gestion de projet)
- Placer les compétences les plus recherchées en premier
- Supprimer les compétences obsolètes ou non pertinentes pour le poste cible

---

### 5. OPTIMISATION ATS

Vérifier et corriger :
- Titres de section standards (Expériences, Formation, Compétences — pas de noms créatifs)
- Format de fichier : .docx ou .pdf texte (jamais image, jamais tableaux complexes)
- Mots-clés de l'offre d'emploi intégrés naturellement dans le texte
- Dates au format standard : mois/année
- Pas de header/footer pour les infos importantes (certains ATS ne les lisent pas)

---

### 6. ANALYSE COMPARATIVE CV ↔ LINKEDIN (si LinkedIn fourni)

Appeler le skill `skills-linkedin` et reporter :
- **Incohérences** : Dates, intitulés, noms d'entreprises qui diffèrent
- **Absent du LinkedIn** : Projets, certifications, réalisations présents dans le CV
- **Absent du CV** : Contenu LinkedIn à intégrer dans le CV
- **Écarts de mots-clés** : Termes forts du CV absents du profil LinkedIn

---

### 7. PLAN D'ACTION FINAL

Livrer un plan numéroté, priorisé par impact :
1. Corriger les incohérences de dates et d'intitulés en premier
2. Réécrire le titre et le profil (plus haute visibilité)
3. Reformuler les bullets d'expérience rôle par rôle (plus récent en premier)
4. Restructurer la section compétences
5. Synchroniser CV ↔ LinkedIn

---

## Format de sortie obligatoire

Toujours structurer la réponse ainsi :

```
## 🔍 AUDIT CV

- STRUCTURE & LISIBILITÉ : /10
- QUALITÉ DU CONTENU : /10
- OPTIMISATION ATS : /10
- IMPACT RECRUTEUR : /10

### 🚨 PROBLÈMES CRITIQUES
- ...

### 💡 AMÉLIORATIONS RAPIDES
- ...

---

## 📊 DONNÉES EXTRAITES DU CV

- Nom :
- Poste actuel / titre :
- Années d'expérience :
- Compétences clés :
- Métriques identifiées :
- Certifications :

---

## ✍️ CV OPTIMISÉ

### TITRE (réécrit)
...

### PROFIL (réécrit)
...

### EXPÉRIENCES (réécrites)
**[Intitulé] @ [Entreprise] (dates)**
- Bullet 1 (AVEC MÉTRIQUE)
- Bullet 2
- Bullet 3

---

## 🔄 COMPARAISON CV vs LINKEDIN (si LinkedIn fourni)

- INCOHÉRENCES :
- ÉLÉMENTS MANQUANTS :
- DÉSALIGNEMENTS STRATÉGIQUES :

---

## 🚀 PLAN D'ACTION FINAL

1. ...
2. ...
3. ...
```

---

## Règles et anti-patterns

### NE JAMAIS faire :
- ❌ Donner des conseils génériques du type "ajoutez une photo professionnelle"
- ❌ Écrire des bullets d'expérience vagues sans métriques
- ❌ Ignorer le LinkedIn si fourni — toujours appeler `skills-linkedin`
- ❌ Produire une sortie non structurée
- ❌ Être non actionnable — chaque recommandation doit être immédiatement applicable
- ❌ Inventer des informations non présentes dans le CV fourni

### TOUJOURS faire :
- ✔ Utiliser des verbes d'action forts (Piloté, Déployé, Optimisé, Généré, Structuré, Réduit…)
- ✔ Inclure des résultats chiffrés dans au moins 2 bullets par rôle
- ✔ Aligner les mots-clés avec le poste cible
- ✔ Écrire le profil à la troisième personne (style CV) ou première personne selon la convention locale
- ✔ Fournir un plan d'action numéroté trié par impact

---

## Cas particuliers

| Situation | Traitement |
|---|---|
| **Reconversion professionnelle** | Mettre en avant les compétences transférables ; reformuler le narratif autour du secteur cible |
| **Profil junior** | Valoriser les projets, la formation, les soft skills et le potentiel — compenser le manque de métriques par la portée |
| **Profil senior / dirigeant** | Mettre en avant le leadership, le P&L, la taille des équipes, l'impact stratégique |
| **Profil multi-secteurs** | Choisir un angle de positionnement clair ; aborder la polyvalence dans le profil |
| **CV incomplet** | Signaler toutes les sections manquantes comme problèmes critiques ; prioriser la complétude |
| **Pas de métriques disponibles** | Utiliser des indicateurs de périmètre : taille d'équipe, nombre de projets, couverture géographique, budget géré |
| **Trous dans le parcours** | Ne pas inventer ; suggérer une formulation neutre et honnête |

---

## Verbes d'action recommandés (français)

**Gestion de projet :** Piloté · Coordonné · Orchestré · Planifié · Livré · Cadré · Structuré

**Technique :** Déployé · Configuré · Développé · Intégré · Automatisé · Migré · Optimisé

**Impact :** Réduit · Augmenté · Généré · Économisé · Amélioré · Accéléré · Fiabilisé

**Leadership :** Managé · Formé · Accompagné · Fédéré · Négocié · Représenté

---

## Note sur la fiabilité

Ce skill applique un protocole strict anti-hallucination :
- Il ne complète jamais les informations manquantes par de l'imagination
- Si une donnée est absente du CV, il indique clairement "Information non disponible"
- Toute réécriture reste fidèle aux faits fournis par l'utilisateur
