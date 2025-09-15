# 🧪 Réacteur Piston - Isomérisation Cis-2-Butène → Trans-2-Butène

## 📋 Description

Ce projet présente une simulation complète d'un réacteur piston (PFR) pour l'isomérisation catalytique du cis-2-butène en trans-2-butène. Le système utilise un contrôleur adaptatif intelligent qui ajuste automatiquement le volume du réacteur pour atteindre une conversion cible précise.

## ⚡ Caractéristiques Principales

- **Réaction :** Isomérisation cis-2-butène ⇌ trans-2-butène
- **Type de Réacteur :** Plug-Flow Reactor (PFR)
- **Contrôle Adaptatif :** Volume auto-optimisé selon la conversion désirée
- **Conversion Cible :** 90% ± 0,0001 (tolérance ultra-précise)
- **Volume Calculé :** 0,988542 m³

## 🔧 Conditions Opératoires

| Paramètre          | Valeur     | Unité  |
|--------------------|------------|--------|
| Température        |   25       | °C     |
| Pression           |   12       | bar    |
| Débit Massique     | 3600       | kg/h   |
| Débit Molaire      |   64,1639  | kmol/h |
| Débit Volumétrique |    5,81905 | m³/h   |

## 📊 Résultats de Simulation

### Composition d'Entrée
- **Cis-2-butène :** 100% (alimentation pure)

### Composition de Sortie
- **Trans-2-butène :** 89,99%
- **Cis-2-butène :** 10,00%

### Performance Énergétique
- **Charge Thermique :** -54,60 kW (exothermique)
- **Temps de Séjour :** 0,16358 h

## 🔬 Modèles Utilisés

### Thermodynamique
- **Package :** Peng-Robinson (PR)
- **Phase :** Liquide
- **Base de Calcul :** Concentrations molaires

### Cinétique
- **Modèle :** Arrhenius
- **Constante pré-exponentielle (A) :** 0,003833 s⁻¹
- **Énergie d'activation (E) :** 0 J/mol
- **Type :** Réaction simple, isotherme

### Géométrie du Réacteur
- **Volume :** 0,988542 m³
- **Diamètre :** 1121,9 mm
- **Longueur :** 1000 mm
- **Nombre de tubes :** 1

## 🎯 Système de Contrôle

Le contrôleur bloc **C-1** implémente une stratégie de contrôle avancée :

- **Variable Manipulée :** Volume du réacteur
- **Variable Contrôlée :** Conversion du cis-2-butène
- **Set-Point :** 90%
- **Tolérance :** 0,0001 (erreur maximale)
- **Algorithme :** Convergence avec solveur Flowsheet

## 🧮 Équation de Réaction

CH₃CH=CHCH₃ (cis) ⇌ CH₃CH=CHCH₃ (trans)

**Stœchiométrie :**
- Cis-2-butène : -1
- Trans-2-butène : +1

**Chaleur de Réaction :** -3600 kJ/kmol

## 💻 Outils de Simulation

- **Logiciel :** Simulateur de procédés avancé
- **Solveur :** Implicit Runge-Kutta
- **Méthode :** Calculs rigoureux avec équations d'état
- **Convergence :** Itérative avec tolérance serrée

## 🚀 Applications Industrielles

Cette simulation trouve des applications dans :

1. **Industrie Pétrochimique**
   - Production de butadiène
   - Synthèse de caoutchouc synthétique

2. **Raffinage**
   - Amélioration de l'indice d'octane
   - Optimisation des coupes essence

3. **Chimie Fine**
   - Intermédiaires de synthèse
   - Matières premières spécialisées

## 📈 Optimisation

Le système démontre :
- **Flexibilité :** Adaptation automatique du volume
- **Précision :** Contrôle ultra-précis de la conversion
- **Stabilité :** Fonctionnement isotherme stable
- **Efficacité :** Minimisation du volume réactionnel

## 🔍 Points Clés d'Ingénierie

- **Innovation :** Contrôle adaptatif du dimensionnement
- **Performance :** 90% de conversion avec tolérance minimale  
- **Robustesse :** Convergence garantie avec solveur implicite
- **Économie :** Volume optimisé pour les conditions données

## 📝 Notes Techniques

- La réaction est légèrement exothermique (-54,6 kW)
- Le fonctionnement isotherme simplifie le contrôle
- La haute pureté du produit (89,99% trans) est excellente
- Le temps de séjour court (0,16 h) optimise la productivité
