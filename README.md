# HodorPro — تطبيق ذكي لإدارة الغيابات 🎓

<div align="center">

<img src="icon-192.png" alt="HodorPro Logo" width="120" style="border-radius:24px"/>

### تطبيق إدارة الغيابات للأساتذة
**Application de gestion des absences pour enseignants**

[![GitHub Pages](https://img.shields.io/badge/Live-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://drissharafi.github.io/MobAbsence)
[![Version](https://img.shields.io/badge/Version-1.0-green?style=for-the-badge)](https://github.com/drissharafi/MobAbsence)
[![License](https://img.shields.io/badge/License-Free-orange?style=for-the-badge)](https://github.com/drissharafi/MobAbsence)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20Web-lightgrey?style=for-the-badge)](https://github.com/drissharafi/MobAbsence)

</div>

---

## 🌐 Application en ligne

```
https://drissharafi.github.io/MobAbsence
```

> Ouvrez ce lien dans **Chrome** sur Android → Menu ⋮ → **"Ajouter à l'écran d'accueil"**

---

## 📱 Aperçu

HodorPro est une application mobile progressive (PWA) conçue spécialement pour les enseignants marocains. Elle permet de gérer les absences des élèves rapidement, sans connexion internet, et avec une interface disponible en **français et en arabe**.

---

## ✨ Fonctionnalités

### 📋 Gestion des absences
- ✅ Faire l'appel en un tap : **P** (Présent) / **A** (Absent) / **R** (Retard)
- 🔍 Recherche rapide d'élève
- 🎯 Filtre par statut (absents uniquement)
- ✓✓ Marquer tous les élèves d'un coup

### 👥 Gestion des élèves
- Ajouter / Modifier / Supprimer des élèves
- Organiser par classes
- Fiche élève avec statistiques complètes
- Taux de présence par élève

### 📊 Rapports & Export
- 📄 Export **CSV** — compatible tous les tableurs
- 📊 Export **Excel (.xlsx)** — 3 feuilles : absences, résumé élèves, par classe
- 📑 Export **PDF** — rapport complet prêt à imprimer
- 📥 Import **CSV / Excel** — importer une liste d'élèves

### 🔔 Alertes & Historique
- ⚠️ Alertes automatiques après 3 absences
- 📅 Historique complet de tous les appels
- 📈 Statistiques par classe et par élève

### ⚙️ Paramètres
- 🌙 **Mode sombre** — confortable pour les yeux
- 🌐 **Interface bilingue** — Français / العربية (RTL)
- ☁️ **Sauvegarde** — export JSON pour sécuriser les données
- 🔄 Sauvegarde automatique après chaque appel

### 📱 Technique
- 💯 **100% hors ligne** — fonctionne sans internet
- 🔒 **Données privées** — stockées uniquement sur l'appareil
- 🔋 **Légère** — moins de 1 Mo, ne consomme pas la batterie
- 📲 **Installable** — comme une vraie app Android

---

## 🚀 Installation

### Sur Android (recommandé)
1. Ouvrez **Chrome** sur votre téléphone
2. Allez sur `https://drissharafi.github.io/MobAbsence`
3. Menu **⋮** → **"Ajouter à l'écran d'accueil"**
4. Appuyez **"Installer"** ✅

### Sur iPhone
1. Ouvrez **Safari** (pas Chrome)
2. Allez sur le lien de l'app
3. Icône **Partager** ↑ → **"Sur l'écran d'accueil"** ✅

### APK Android direct
Téléchargez l'APK depuis la section [Releases](https://github.com/drissharafi/MobAbsence/releases)

---

## 📂 Structure du projet

```
MobAbsence/
├── index.html              ← Application complète (HTML + CSS + JS)
├── icon-192.png            ← Logo HodorPro 192×192
├── README.md               ← Ce fichier
└── android/                ← Projet Android Studio (APK)
    ├── app/
    │   ├── src/main/
    │   │   ├── assets/
    │   │   │   └── index.html
    │   │   ├── java/com/hodorpro/app/
    │   │   │   └── MainActivity.java
    │   │   ├── res/
    │   │   │   ├── mipmap-*/
    │   │   │   │   └── ic_launcher.png
    │   │   │   └── values/
    │   │   │       ├── strings.xml
    │   │   │       └── styles.xml
    │   │   └── AndroidManifest.xml
    │   └── build.gradle
    ├── build.gradle
    └── settings.gradle
```

---

## 🛠️ Technologies utilisées

| Technologie | Rôle |
|---|---|
| **HTML5** | Structure de l'interface |
| **CSS3** | Design, mode sombre, RTL arabe |
| **JavaScript ES6** | Logique métier et navigation |
| **localStorage** | Base de données locale |
| **Web App Manifest** | Installation PWA |
| **Canvas API** | Icône dynamique |
| **SheetJS** | Import/Export Excel |
| **Java (Android)** | Wrapper WebView natif |
| **AdMob SDK** | Publicités (bannière + interstitiel) |
| **Gradle** | Compilation Android |

---

## 💰 Monétisation

L'application utilise **Google AdMob** pour afficher des publicités :
- **Bannière** — affichée en bas de l'écran
- **Interstitiel** — plein écran toutes les 5 pages

> Pour activer les vraies publicités, remplacez les IDs de test dans `MainActivity.java` par vos IDs AdMob depuis [admob.google.com](https://admob.google.com)

---

## 📋 Format d'import CSV

```csv
Nom,Classe
أحمد المحمودي,2APIC1
فاطمة الزهراء,2APIC1
سارة بنعلي,1APIC1
```

---

## 🔧 Compilation APK

### Prérequis
- [Android Studio](https://developer.android.com/studio) (gratuit)
- Android SDK 34

### Étapes
```bash
1. Ouvrir le dossier android/ dans Android Studio
2. Attendre la sync Gradle (3-5 min)
3. Build → Generate Signed APK
4. Créer un Keystore (garder précieusement !)
5. Choisir "release" → Finish
6. APK dans : app/release/app-release.apk
```

---

## 🏪 Publication Play Store

1. Créer un compte sur [Google Play Console](https://play.google.com/console) (25 USD)
2. Générer un **AAB** (Android App Bundle) au lieu de APK
3. Remplir la fiche : description, screenshots, icône 512×512
4. Ajouter la politique de confidentialité
5. Soumettre → validation 1-3 jours ✅

---

## 📊 Compatibilité

| Plateforme | Version minimum | Status |
|---|---|---|
| Android | 5.0 (API 21) | ✅ Supporté |
| Android | 14 (API 34) | ✅ Testé |
| iPhone (Safari) | iOS 13+ | ✅ Supporté |
| Chrome Desktop | Toute version | ✅ Supporté |

---

## 🔒 Politique de confidentialité

HodorPro respecte la vie privée des utilisateurs :
- ❌ Aucune donnée collectée sur nos serveurs
- ✅ Toutes les données stockées localement sur l'appareil
- ✅ Aucun compte requis
- ✅ Fonctionne sans connexion internet
- ⚠️ Les publicités AdMob peuvent collecter des données anonymes (voir [politique Google](https://policies.google.com/privacy))

---

## 📞 Contact & Support

- **Développeur** : Driss Harafi
- **GitHub** : [@drissharafi](https://github.com/drissharafi)
- **App** : [drissharafi.github.io/MobAbsence](https://drissharafi.github.io/MobAbsence)

---

## 📄 Licence

Ce projet est distribué gratuitement pour usage personnel et éducatif.

---

<div align="center">

**HodorPro v1.0** — Fait avec ❤️ pour les enseignants marocains

*تسجيل الغياب • تتبع الحضور • حماية قانونية*

</div>
