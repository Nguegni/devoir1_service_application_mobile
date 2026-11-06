# devoir1_service_application_mobile
Exercice 1 — Parts de marché des systèmes d'exploitation mobiles &amp; Exercice 2 — Architecture Android
# Devoir : Systèmes d'exploitation mobiles et architecture Android

## Introduction

Les systèmes d'exploitation mobiles jouent un rôle essentiel dans le fonctionnement des smartphones. Android, iOS et HarmonyOS figurent parmi les principaux systèmes du marché.

Ce travail présente leurs parts de marché, puis explique les différences entre Android Runtime et les bibliothèques natives, deux composants importants de l'architecture Android.

---

## Exercice 1 : Parts de marché d'Android, iOS et HarmonyOS

### 1. Présentation des systèmes

**Android** est un système d'exploitation basé sur Linux, développé principalement par Google. Il est utilisé par de nombreux fabricants de smartphones, notamment Samsung, Xiaomi, OPPO et Tecno.

**iOS** est le système d'exploitation développé par Apple pour ses iPhone. Contrairement à Android, son utilisation est réservée aux appareils compatibles d'Apple.

**HarmonyOS** est un système développé par Huawei. Il est principalement présent dans l'écosystème de Huawei et occupe une position importante sur le marché chinois.

### 2. Parts de marché mondiales

Selon Counterpoint Research, les parts des ventes mondiales de smartphones au deuxième trimestre 2026 sont les suivantes :

| Système | Part de marché |
|---|---:|
| Android | 75 % |
| iOS | 20 % |
| HarmonyOS | 5 % |
| **Total** | **100 %** |

Ces données représentent la répartition des ventes de smartphones durant le trimestre étudié, et non celle de l'ensemble des appareils déjà en circulation.

### 3. Comparaison avec le marché chinois

Au deuxième trimestre 2026, la situation en Chine est différente :

| Système | Part de marché en Chine |
|---|---:|
| Android | 58 % |
| iOS | 18 % |
| HarmonyOS | 24 % |

HarmonyOS occupe ainsi la deuxième place en Chine, devant iOS, alors qu'il se situe à la troisième place au niveau mondial.

### 4. Analyse des résultats

Android domine le marché mondial. Sa présence chez de nombreux fabricants lui permet de couvrir différentes gammes de smartphones.

iOS conserve une place importante grâce à l'écosystème Apple et à la commercialisation des iPhone.

HarmonyOS affiche une part mondiale plus limitée, mais sa forte présence en Chine montre qu'un système peut être particulièrement compétitif sur un marché national.

Il faut également distinguer la part des ventes récentes de celle des appareils effectivement utilisés. Les chiffres peuvent varier selon la méthode de mesure, la région et la période.

### Conclusion de l'exercice 1

Android reste le système dominant dans les ventes mondiales de smartphones au deuxième trimestre 2026, avec 75 %. iOS suit avec 20 %, tandis que HarmonyOS représente 5 %. Toutefois, l'exemple de la Chine montre que cette hiérarchie peut varier selon les régions.

---

## Exercice 2 : Différences entre Android Runtime et les bibliothèques natives

### 1. Android Runtime (ART)

Android Runtime, abrégé ART, est l'environnement d'exécution utilisé par les applications Android modernes.

Il permet notamment d'exécuter le bytecode DEX produit à partir du code d'une application écrite en Java ou Kotlin.

Ses principales fonctions sont :

- L'exécution du code DEX des applications.
- La compilation du code grâce aux mécanismes JIT (*Just-In-Time*) et AOT (*Ahead-Of-Time*).
- La gestion automatique de la mémoire des objets gérés grâce au ramasse-miettes (*Garbage Collector*).
- La prise en charge de mécanismes de diagnostic et de débogage.

ART a remplacé Dalvik comme environnement d'exécution principal à partir d'Android 5.0.

### 2. Bibliothèques natives

Les bibliothèques natives sont des composants logiciels généralement écrits en C ou C++ et compilés en code machine.

Elles fournissent des fonctionnalités spécialisées utilisées par le système Android ou par certaines applications.

Quelques exemples :

- **SQLite** : gestion de bases de données locales.
- **OpenGL ES** : fonctionnalités graphiques 2D et 3D.
- **Bibliothèques multimédias** : traitement de l'audio et de la vidéo.
- **Bibliothèques système** : fonctions de bas niveau nécessaires au fonctionnement du système.

Certaines bibliothèques natives peuvent être utilisées à travers les API Android. Les développeurs peuvent également utiliser le NDK (*Native Development Kit*) pour intégrer leur propre code natif.

### 3. Tableau comparatif

| Critère | Android Runtime | Bibliothèques natives |
|---|---|---|
| Nature | Environnement d'exécution | Ensemble de composants logiciels |
| Fonction | Exécuter le code DEX | Fournir des fonctionnalités spécialisées |
| Technologies | DEX, AOT, JIT | Principalement C/C++ et code machine |
| Mémoire | Gestion automatique des objets gérés | Gestion mémoire propre au code natif |
| Utilisation | Applications Android | Système et applications |
| Exemple | Exécution du code Java/Kotlin | Graphisme et bases de données |

### 4. Exemple pratique

Prenons l'exemple d'une application Android développée en Kotlin qui affiche des informations provenant d'une base de données locale.

Android Runtime intervient dans l'exécution du code Kotlin compilé de l'application.

Pour accéder à une base SQLite, l'application peut utiliser les API Android qui reposent sur des composants natifs.

Ainsi, Android Runtime et les bibliothèques natives travaillent ensemble pour assurer le fonctionnement de l'application.

### Conclusion de l'exercice 2

Android Runtime est chargé de l'exécution du code géré des applications Android, tandis que les bibliothèques natives proposent des fonctionnalités spécialisées reposant sur du code compilé.

Ces deux composants sont complémentaires et jouent des rôles distincts dans l'architecture du système d'exploitation Android.

---

## Références bibliographiques

1. Counterpoint Research — *Global Smartphone Sales Share by Operating System*, 30 août 2026.  
   https://counterpointresearch.com/en/insights/global-smartphone-os-market-share

2. Android Developers — *Platform Architecture*.  
   https://developer.android.com/guide/platform

3. Android Open Source Project — *Android Runtime and Dalvik*.  
   https://source.android.com/docs/core/runtime

4. Android Developers — *Android NDK Concepts*.  
   https://developer.android.com/ndk/guides/concepts

*Travail de recherche — Novembre 2026.*
