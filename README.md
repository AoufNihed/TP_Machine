# 🧠 Simulation du Manque de Phase dans un Moteur Asynchrone

> Projet de simulation pédagogique pour l’analyse du comportement d’un moteur asynchrone en cas de manque de phase, avec visualisation et analyse FFT.

---

## 📁 Contenu du dépôt

Ce dépôt contient :
- Une **simulation en Python** du courant triphasé d’un moteur en mode normal et en cas de **manque de phase**.
- Une **analyse FFT (Fast Fourier Transform)** pour observer les composantes fréquentielles.
- Des **visualisations** des signaux temporels et des spectres en fréquence.
- Une **interprétation technique** du phénomène.

---

## ⚙️ Objectifs pédagogiques

- Comprendre les effets du **déséquilibre de phase** dans un moteur triphasé.
- Visualiser la **différence entre un fonctionnement normal et un fonctionnement dégradé**.
- Utiliser la **transformée de Fourier** pour détecter des anomalies dans les signaux électriques.
- Montrer l’intérêt de l’**analyse fréquentielle** dans la maintenance prédictive.

---

## 🧪 Description technique

### 🟢 Fonctionnement normal :
- Courants triphasés équilibrés (Ia, Ib, Ic).
- Phase espacée de 120°.
- Spectre FFT avec pic principal à **50 Hz** (fréquence du réseau).

### 🔴 Manque de phase :
- Une phase (ex : Ib) devient **nulle**.
- Création d’un **déséquilibre** dans les courants.
- Apparition d’**harmoniques** dans le spectre FFT (100 Hz, 150 Hz, etc).

---

## 📊 Méthodologie

1. Génération de signaux sinusoïdaux simulant les courants triphasés.
2. Visualisation dans le domaine **temporel**.
3. Calcul de la **FFT** avec `scipy.fft` pour chaque phase.
4. Visualisation des spectres dans le domaine **fréquentiel**.
5. Comparaison des deux cas (normal vs. défaut).

---

## 📌 Outils utilisés

- Python 🐍
- Numpy 📐
- Matplotlib 📊
- Scipy ⚙️ (FFT)

---

## 🧠 Résultats attendus

- ✅ En mode normal : Spectre clair avec fréquence principale à 50 Hz.
- ❌ En cas de manque de phase : Déséquilibre visible + harmonique détectée.
- Ce type de défaut peut être détecté **automatiquement** avec une surveillance temps réel.

---
