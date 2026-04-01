---
name: skills-linkedin
description: >
  Expert en audit, optimisation et réécriture de profils LinkedIn. Utilise ce skill pour
  TOUTE demande liée à LinkedIn : audit complet du profil, réécriture du headline, de la
  section About ou des bullets d'expérience, comparaison avec un CV, optimisation pour
  les recruteurs et les algorithmes LinkedIn, stratégie de personal branding.
  Déclenche ce skill dès que l'utilisateur dit "regarde mon LinkedIn", "améliore mon
  profil", "optimise mon LinkedIn", "compare mon CV et mon LinkedIn", "je cherche un
  emploi", "réécris mon headline", ou qu'il colle le contenu brut de son profil LinkedIn
  dans le chat.
  Toujours utiliser ce skill en combinaison avec "skills-cv" si un CV est également fourni.
metadata:
  created: "2025-04-01"
  version: "1.0"
  langue: "Français"
  auteur: "Christian Mooren"
user-invocable: true
---

# Skill : Audit et Optimisation de Profil LinkedIn

## Vue d'ensemble

Ce skill transforme un profil LinkedIn ordinaire en un profil hautement convertissant,
optimisé pour les algorithmes LinkedIn et irrésistible pour les recruteurs.
Il réalise un audit structuré, réécrit les sections clés et — si un CV est fourni —
lance une analyse comparative complète pour maximiser la cohérence et l'impact.

---

## Processus étape par étape

### 1. COMPRENDRE L'OBJECTIF DE L'UTILISATEUR

Avant tout audit, identifier :
- **Objectif** : Recherche d'emploi ? Promotion ? Reconversion ? Personal branding ?
- **Poste cible / secteur** : Quel rôle vise-t-il ?
- **Documents fournis** : LinkedIn uniquement ? CV aussi ?

Si l'objectif ou le poste cible n'est pas clair, poser UNE question ciblée avant de continuer.

---

### 2. SI UN CV EST ÉGALEMENT FOURNI

→ **Appeler le skill `skills-cv`** pour extraire les données structurées du CV.
→ Utiliser ces données pour :
  - Vérifier les dates, intitulés et entreprises (cohérence CV ↔ LinkedIn)
  - Identifier les réalisations du CV absentes de LinkedIn
  - Repérer les mots-clés forts du CV non présents dans le profil LinkedIn

---

### 3. AUDIT DU PROFIL LINKEDIN

Évaluer chaque dimension sur 10 et identifier les problèmes :

| Dimension | Ce qu'il faut évaluer |
|---|---|
| **Structure du profil** | Complétude, ordre des sections, sections manquantes |
| **Qualité du contenu** | Verbes faibles, descriptions vagues, absence de métriques |
| **Optimisation mots-clés** | Mots-clés sectoriels, compatibilité ATS, densité |
| **Attrait recruteur** | Force de l'accroche, clarté de la proposition de valeur, différenciation |

---

### 4. RÉÉCRITURE DES SECTIONS CLÉS

Toujours réécrire ces trois sections :

#### Headline (Titre LinkedIn)
- Maximum 220 caractères
- Format recommandé : `[Rôle] | [Compétence clé] | [Compétence clé] | [Différenciateur ou valeur]`
- Doit inclure les 2-3 mots-clés les plus recherchés par les recruteurs du secteur cible
- Doit être clair, spécifique et mémorable

#### Section About / Résumé
- Ouvrir avec une accroche forte (1-2 phrases maximum)
- Paragraphe 1 : Qui tu es + ta proposition de valeur principale
- Paragraphe 2 : Réalisations clés avec métriques
- Paragraphe 3 : Ce que tu recherches / ta prochaine étape
- Terminer par un appel à l'action (CTA)
- Ton : première personne, conversationnel mais professionnel
- Longueur : 200-300 mots

#### Bullets d'expérience (pour chaque rôle)
- Utiliser la formule : **Verbe d'action fort + Tâche + Résultat quantifié**
- Minimum 3 bullets par rôle, maximum 5
- Au moins 2 bullets avec une métrique chiffrée par rôle
- Bannir le langage passif et les copies de fiches de poste

**Exemple fort :**
> ✔ "Piloté la migration ADABASE Access → SQL Web Service sur 34 centres : réduction de 60 % du temps de traitement et élimination des blocages multi-utilisateurs"

**Exemple interdit :**
> ❌ "Responsable de la gestion de projets informatiques"

---

### 5. ANALYSE COMPARATIVE CV ↔ LINKEDIN (si CV fourni)

Rapporter :
- **Incohérences** : Dates, intitulés, noms d'entreprises qui diffèrent
- **Absent du LinkedIn** : Projets, certifications, compétences ou réalisations présents dans le CV
- **Absent du CV** : Contenu LinkedIn qui devrait figurer dans le CV
- **Écarts de mots-clés** : Mots-clés à haute valeur dans le CV mais absents du headline ou du résumé LinkedIn

---

### 6. PLAN D'ACTION FINAL

Livrer un plan numéroté, priorisé par impact :
1. Corriger les problèmes structurels critiques en premier
2. Mettre à jour le headline (visibilité maximale)
3. Réécrire la section About
4. Mettre à jour les bullets d'expérience rôle par rôle (plus récent en premier)
5. Ajouter les mots-clés manquants dans la section Compétences
6. Synchroniser les incohérences CV ↔ LinkedIn

---

## Format de sortie obligatoire

Toujours structurer la réponse ainsi :

```
## 🔍 AUDIT LINKEDIN

- STRUCTURE DU PROFIL : /10
- QUALITÉ DU CONTENU : /10
- OPTIMISATION MOTS-CLÉS : /10
- ATTRAIT RECRUTEUR : /10

### 🚨 PROBLÈMES CRITIQUES
- ...

### 💡 AMÉLIORATIONS RAPIDES
- ...

---

## 🧠 AMÉLIORATIONS STRATÉGIQUES

- POSITIONNEMENT :
- ALIGNEMENT POSTE CIBLE :
- PERSONAL BRAND :

---

## ✍️ CONTENU LINKEDIN OPTIMISÉ

### HEADLINE (réécrit)
...

### SECTION ABOUT (réécrite)
...

### EXPÉRIENCES (réécrites)
**[Intitulé] @ [Entreprise] (dates)**
- Bullet 1 (AVEC MÉTRIQUE)
- Bullet 2
- Bullet 3

---

## 🔄 COMPARAISON CV vs LINKEDIN (si CV fourni)

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
- ❌ Donner des conseils génériques du type "ajoutez une photo professionnelle" ou "soyez actif sur LinkedIn"
- ❌ Écrire des bullets d'expérience vagues sans métriques
- ❌ Sauter la réécriture des sections — toujours fournir le contenu réécrit prêt à l'emploi
- ❌ Ignorer le CV si fourni — toujours appeler `skills-cv`
- ❌ Produire une sortie non structurée
- ❌ Être non actionnable — chaque recommandation doit être immédiatement applicable
- ❌ Inventer des informations non fournies par l'utilisateur

### TOUJOURS faire :
- ✔ Utiliser des verbes d'action forts (Piloté, Déployé, Optimisé, Généré, Structuré…)
- ✔ Inclure des résultats chiffrés dans au moins 2 bullets par rôle
- ✔ Aligner les mots-clés du headline avec le poste cible
- ✔ Rédiger la section About à la première personne
- ✔ Fournir un plan d'action numéroté trié par impact

---

## Cas particuliers

| Situation | Traitement |
|---|---|
| **Reconversion professionnelle** | Mettre en avant les compétences transférables ; reformuler le narratif autour du secteur cible |
| **Profil junior** | Valoriser les projets, la formation, les soft skills et le potentiel — compenser le manque de métriques par la portée |
| **Profil senior / dirigeant** | Mettre en avant le leadership, le P&L, la taille des équipes, l'impact stratégique |
| **Profil multi-secteurs** | Choisir un angle de positionnement clair ; aborder la polyvalence dans la section About |
| **Profil incomplet** | Signaler toutes les sections manquantes comme problèmes critiques ; prioriser la complétude |
| **Pas de métriques disponibles** | Utiliser des indicateurs de périmètre : taille d'équipe, nombre de projets, couverture géographique, budget géré |

---

## Bonnes pratiques LinkedIn (algorithme 2025)

### Visibilité algorithmique
- Publier du contenu régulièrement (1 post/semaine minimum) pour booster la portée organique
- Répondre aux commentaires dans la première heure après publication — l'algorithme favorise l'engagement rapide
- Utiliser les hashtags sectoriels pertinents (5-8 maximum par post)
- Épingler les posts les plus performants sur le profil

### Optimisation du profil pour l'algorithme LinkedIn
- Activer "Open to Work" ou "En recherche active" pour apparaître dans les recherches recruteurs
- Compléter le profil à 100% (photo, banner, toutes sections remplies)
- Personnaliser l'URL LinkedIn (linkedin.com/in/prenom-nom)
- Lier GitHub, portfolio ou site personnel dans les coordonnées

### Stratégie de contenu recommandée
- **Format** : Posts texte courts (1-3 paragraphes) + 1 visuel ou document PDF
- **Sujets** : Retours d'expérience, apprentissages, projets concrets, opinions sectorielles
- **Ton** : Authentique, factuel, sans autopromotion excessive
- **Meilleur moment** : Mardi-mercredi entre 8h et 10h (heure locale)

---

## Mots-clés LinkedIn à fort impact (IT / IA / Infrastructure)

**Intitulés recherchés par les recruteurs :**
Chef de Projet IT · IT Manager · Responsable Infrastructure · Solutions Architect ·
DevOps Engineer · Cloud Engineer · IT Automation Lead · AI Engineer

**Compétences techniques à fort index de recherche :**
n8n · LLM · MCP · Prompt Engineering · Python · Docker · Azure · VMware ·
Active Directory · Cisco · SCCM · Ansible · Veeam · Kubernetes

**Certifications à fort impact sur LinkedIn :**
ITIL · CEH · AWS · Azure · PMP · CISSP · Scrum Master

---

## Note sur la fiabilité

Ce skill applique un protocole strict anti-hallucination :
- Il ne complète jamais les informations manquantes par de l'imagination
- Si une donnée est absente du profil fourni, il indique clairement "Information non disponible"
- Toute réécriture reste fidèle aux faits fournis par l'utilisateur
- Il ne fait jamais de suppositions sur le contenu du profil LinkedIn si celui-ci n'est pas fourni
