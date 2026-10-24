<div align="center">

# 📋 EduForms — v1.0.0

### **Studio moderne et souverain de création, collecte et analyse de formulaires hors-ligne**
*Une alternative professionnelle, locale et respectueuse de la vie privée à Google Forms & Microsoft Forms.*

[![Version](https://img.shields.io/badge/Version-1.0.0-008080.svg?style=for-the-badge&logo=tag&logoColor=white)](#)
[![Plateforme](https://img.shields.io/badge/Plateforme-Windows%2010%20%7C%2011%20(64--bit)-0078D6.svg?style=for-the-badge&logo=windows&logoColor=white)](#)
[![Moteur](https://img.shields.io/badge/Moteur-Python%203.11%20%7C%20PySide6-4169E1.svg?style=for-the-badge&logo=python&logoColor=white)](#)
[![Données](https://img.shields.io/badge/Données-100%25%20Hors--ligne%20(SQLite)-22C55E.svg?style=for-the-badge&logo=sqlite&logoColor=white)](#)
[![Licence](https://img.shields.io/badge/Licence-Propriétaire%20Gratuite-EAB308.svg?style=for-the-badge)](#)
[![Qualité](https://img.shields.io/badge/Tests-80%2F80%20validés-brightgreen.svg?style=for-the-badge&logo=pytest&logoColor=white)](#)

---

</div>

## 📌 Présentation

**EduForms** est une application de bureau complète permettant de concevoir des formulaires d'enquête et d'évaluation, de collecter des réponses sur le terrain ou en classe, et d'analyser automatiquement les résultats sous forme de graphiques statistiques interactifs.

Conçue dès l'origine selon le paradigme **Offline-First**, EduForms garantit une autonomie opérationnelle totale :
- 🔒 **100 % Confidentiel & Souverain** : Vos questionnaires et données ne quittent jamais votre ordinateur. Aucune télémétrie, aucun compte requis, zéro dépendance envers le cloud.
- ⚡ **Ultra-Rapide & Fluide** : Moteur natif PySide6 (Qt6) avec base de données SQLite locale.
- 🎒 **Pédagogique & Professionnel** : Idéal pour les établissements scolaires, les universités, les associations et les professionnels soucieux de la protection des données (RGPD-compliant par conception).

---

## 🌟 Fonctionnalités Clés

### 🎨 1. Studio de Conception Ergonomique
- **Organisation modulaire en sections** : Structurez vos formulaires complexes avec des sections repliables et réordonnables à volonté.
- **7 types de questions riches** :
  - 📝 **Texte court** (avec contraintes de longueur et aide contextuelle).
  - 📄 **Paragraphe développé** (champs multilignes avec comptage de caractères).
  - 🔘 **Choix unique (Boutons radio)** aux styles épurés et lisibles.
  - ☑️ **Choix multiples (Cases à cocher)** avec validation de sélections.
  - 🔽 **Liste déroulante** pour les choix volumineux.
  - ⭐ **Échelle linéaire** (1-5 ou 1-10 avec libellés des bornes minimales et maximales).
  - 📅 **Date & Calendrier** avec détection de la date système et sélecteur pop-up interactif.
- **Validateur sémantique en temps réel** : Signalement instantané des incohérences (questions sans option, titres vides, etc.).
- **Prévisualisation interactive immédiate** : Testez le formulaire tel que le répondant le verra avant de le diffuser.

---

### ✍️ 2. Expérience de Collecte & Saisie Optimisée
- 🖥️ **Mode Plein Écran Immersif (`F11`)** : Parfait pour transformer un PC en borne de sondage ou sécuriser les sessions de passation.
- 🔍 **Zoom Visuel Dynamique (80 % à 150 %)** :
  - Barre de zoom avec raccourcis clavier universels (`Ctrl + +`, `Ctrl + -`, `Ctrl + 0`).
  - Lisibilité optimale pour vidéoprojecteurs et écrans haute densité (HiDPI).
- 📅 **Sélecteur de Date Google Forms-Style** :
  - Icône native de calendrier intégrée au champ.
  - Fenêtre contextuelle contrastée et lumineuse (en-tête bleu canard `#008080`, fond blanc immaculé).
  - Pré-remplissage avec la date du jour.
- 📈 **Indicateur de progression interactif** affiché en temps réel au fur et à mesure de la saisie.

---

### 📊 3. Tableaux de Bord & Analyses Statistiques
- 🥧 **Diagrammes circulaires (Donut / Camembert)** : Répartition chromatique claire avec pourcentages précis et légendes détaillées.
- 📊 **Graphiques à barres horizontales** : Comparaison immédiate de la popularité de chaque modalité.
- 📈 **Histogrammes de distribution d'échelles** avec note moyenne globale en étoiles (ex. `⭐ Note moyenne : 4.33 / 5`).
- 💬 **Flux de réponses ouvertes textuelles** pour explorer l'ensemble des retours qualitatifs.
- 🔄 **Bascule instantanée Camembert ↔ Barres** en un clic.
- 💾 **Export haute résolution PNG** : Enregistrez n'importe quel graphique directement sur votre disque pour l'intégrer dans vos rapports.

---

### 📁 4. Exports & Interopérabilité
- 📊 **Microsoft Excel (`.xlsx`)** : Génération automatisée de classeurs avec en-têtes stylisés, bordures de données et colonnes ajustées.
- 📄 **Format universel CSV (`.csv`)** : Encodage UTF-8 avec BOM assurant une compatibilité immédiate avec tous les tableurs sans problème d'accents.
- 📦 **Modèles de formulaires transportables (`.formulaire.json` / `.eduform`)** : Exportez vos gabarits pour les partager d'un poste à un autre sans aucune configuration.

---

## 🚀 Installation & Démarrage

### Option A : Installateur Windows Tout-en-Un (Recommandé)
Aucun prérequis ni installation de Python ne sont nécessaires :
1. Rendez-vous dans la section [Releases](https://github.com/cryzo-py/EduForms/releases).
2. Téléchargez **`EduForms_Setup_v1.0.0.exe`**.
3. Lancez l'assistant et suivez les instructions.
4. Démarrez **EduForms** directement depuis le Menu Démarrer ou le raccourci Bureau !

### Option B : Exécution depuis les sources (Développeurs)
```bash
# 1. Cloner le dépôt
git clone https://github.com/cryzo-py/EduForms.git
cd EduForms

# 2. Créer et activer un environnement virtuel
python -m venv .venv
.venv\Scripts\activate

# 3. Installer les dépendances
pip install -r requirements.txt

# 4. Lancer l'application
python run.py
