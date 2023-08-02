# TestNG Framework with Appium, Java 11 and Allure Report
Basic-framework-mobile-android est un framework d'automatisation mobile basé sur Appium et TestNG et qui s'exécute sur les devices Android.

Si vous souhaitez tester une application mobile de préférence sur Android.</br>
🌟Si vous êtes `TESTEUR AUTOMATICIEN` et que vous voulez apprendre à automatiser des tests fonctionnels.</br>
🌟Si vous êtes un `RECRUTEUR` pour évaluer les compétences de nos testeurs automaticiens talentueux.</br>
🌟 Ou encore si vous êtes un `PARTICULIER`ou une `ENTREPRISE` à la recherche de solution
répondant à vos besoins d'automatisation en test alors ce framework est fait pour vous!</br></br>
🎁 Ce framework permet d'exécuter vos tests en séquentiel sur le périphérique Android de votre choix, 
que ce soit un device physique ou un émulateur.</br>
🎁 Vous pouvez un rapport détaillé des tests sur Allure.</br>
🎁 Il s'exécute également sur la plateforme `Windows 10 et 11`.</br>

### 🎯Sommaire:
🏷️[Architecture et Présentation du framework](#architecture-et-présentation-du-framework)<br/>
🏷️[Technologies et outils utilisés](#technologies-et-outils-utilisés)</br>
🏷️[Fonctionnalités](#fonctionnalités)<br/>
🏷️[Environnement de développement](#environnement-de-développement)<br/>
🏷️[Installation du framework](#installation-du-framework)<br/>
🏷️[Pré-requis](#prérequis)</br>
🏷️[Exécution du framework](#exécution-du-framework)<br/>
🏷️[Reporting](#Reporting)<br/>
🏷️[Mise à jour et adaptation du Framework](#mise-à-jour-et-adaptation-du-framework)<br/>
🏷️[Déboggage et Maintenance](#déboggage-et-maintenance)<br/>

### 🎯Architecture et Présentation du framework 
````
📦framework-simple-mobile-android
┣ 📂src
┃ ┣ 📂main
┃ ┃ ┣ 📂resources
┃ ┃ ┃ ┗ 📜config.properties
┃ ┣ 📂test
┃ ┃ ┣ 📂java
┃ ┃ ┃ ┣📂FrameworkSimpleAndroid
┃ ┃ ┃ ┃ ┣ 📂base
┃ ┃ ┃ ┃ ┃ ┗ 📜BaseTest.java
┃ ┃ ┃ ┃ ┣ 📂pages
┃ ┃ ┃ ┃ ┃ ┗ 📜LoginPage.java
┃ ┃ ┃ ┃ ┃ ┗ 📜MenuPage.java
┃ ┃ ┃ ┃ ┃ ┗ 📜ProductPage.java
┃ ┃ ┃ ┃ ┃ ┗ 📜SettingsPage.java
┃ ┃ ┃ ┃ ┃ ┣ 📂tests
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜LoginTests.java
┃ ┃ ┃ ┃ ┃ ┣ 📂utils
┃ ┃ ┃ ┃ ┃ ┃ ┗ 📜TestUtils.java
┃ ┃ ┣ 📂resources
┃ ┃ ┃ ┃ ┣ 📂app
┃ ┃ ┃ ┃ ┃ ┗ 📑Android-MyDemoAppRN.apk
┃ ┃ ┃ ┃ ┣ 📂data
┃ ┃ ┃ ┃ ┃ ┗ 📑loginUsers.json
┃ ┃ ┃ ┃ ┣ 📂strings
┃ ┃ ┃ ┃ ┃ ┗ 📑strings.xml
┃ ┃ ┃ ┃ ┗ 📑allure.properties
┃ ┃ ┣ 📂Test-output
┃ ┃ ┃ ┗ 📂allure-report
┃ ┃ ┃ ┗ 📂allure-results
┣ 📑pom.xml
┣ 📑README.md
┣ 📑testng.xml
````

## 🎯Technologies et outils utilisés
➡️ IntelliJ - IDE<br/>
➡️ Appium - Mobile Automation library<br/>
➡️ Maven - Build automation tool<br/>
➡️ Java - Programming language<br/>
➡️ TestNG - Unit testing framework<br/>
➡️ Allure Reports - Reporting framework <br/>

## 🎯Fonctionnalités

✅ Abstraction layer pour les intérations UI (click, sendkeys, ...)<br/>
✅ Paramétrisation par les fichier TestNG XML et config.properties<br/>
✅ Abstraction layer pour les jeux de données<br/>
✅ Abstraction layer pour les textes statiques<br/>
✅ Exécution sur devices physiques (et/ou Emulateurs ) Android<br/>
✅ Démarrage automatique programmé du serveur Appium<br/>


## 🎯Environnement de développement

| Logiciel                       | Version           | Description                                                                                                     | Windows  | Macbook  |
|--------------------------------|-----------------  |-----------------------------------------------------------------------------------------------------------------|----------|----------|
| Java JDK                       | JAVA 11           | [Dowloadable here](https://www.oracle.com/eg/java/technologies/javase/jdk11-archive-downloads.html)             |     X    |    X     |
| Android SDK via Android studio | current available | [Dowloadable here](https://developer.android.com/studio?gclid=Cj0KCQjwuLShBhC_ARIsAFod4fIcuMWb00yxfjGTPrFEemQ_pc3UrvmvB45VSYcnueWrfyX8fLJpz_4aAthfEALw_wcB&gclsrc=aw.ds)             |     X    |    X     |
| Node.js                        | 18.15.0           | [Dowloadable here](https://nodejs.org/en/download)                                                               |     X    |    X     |
| npm                            | 9.5.0             | Downloaded with node.js                                                                                          |     X    |    X     |
| appium                         | 2.0.0-beta.59     | terminal: npm install -g appium@next                                                                             |     X    |    X     |
| appium client (wd)             | current available | terminal: npm install wd                                                                                         |     X    |    X     |
| maven                          | 3.8.6             | [Downloadable here](https://maven.apache.org/download.cgi)                                                       |     X    |    X     |
| Allure                         | current available | [Downloadable here](https://docs.qameta.io/allure/)                                                              |     X    |    X     |


## 🎯Installation du framework

#### Prérequis
🟥 NB: POUR EXÉCUTER CE FRAMEWORK, VOUS DEVEZ AVOIR UNE BONNE CONNEXION INTERNET !

- Devices
  - 📌**Device physique**

    | Description                           | Obligatoire     |
    |---------------------------------------|-----------------|
    | Mode développeur activé sur le device | x               | 
    | Débogage usb activé                   | x               | 
    | Connexion internet activée            | x               | 
    | Device déverouillé                    | x               | 
    | Device connecté au poste via usb      | x               | 


  - 📌**Emulateur** : </br>
    - L'émulateur doit être lancé et en bon état de marche

## 🎯Exécution du framework

- **Depuis l'IDE**:</br>
Depuis un éditeur de code, lancer l'exécution du fichier **testng.xml**

- **Depuis la CLI** (Command Line Interface = invite de commandes):</br>
  Commandes a exécuter depuis un terminal:
```shell
  cd project_repository
  mvn clean test
```
### 🎯Reporting
Les différents rapports et artefacts resultants de l'exécution des tests seront disponibles dans le dossier:
Rapport disponible :
- **_Test-output_**/**_allure-report_**

## 🎯Mise à jour et adaptation du Framework

#### 🪙 Ajouter une nouvelle application
1. Ajouter la(les) nouvelle(s) application(s) dans le dossier **apps** (_chemin d'accès_: src/test/resources/apps)
2. Mettre a jour les informations de l'application dans le fichier **config.properties**(_chemin d'accès_: src/main/resources/config.properties)</br>

   | **Variable**       | **value**         |   
   |--------------------|-------------------|
   | androidAppLocation | apk_path          | 
   | androidAppActivity | apk_activity_name | 
   | androidAppPackage  | apk_package_name  |

#### 🪙 Ajouter de nouveaux tests
- La redaction des tests se fera dans le dossier **tests** (_chemin d'accès: src/test/FrameworkSimpleAndroid/tests_ ) grâce au page Object Design pattern.
- Les pages du Page OBject Design pattern seront ,quand à elles , définies dans le dossier **pages** (_chemin d'accès: src/test/java/FrameworkSimpleAndroid/pages_)

## 🎯Déboggage et Maintenance
### 🔴Débogage
- Erreur suite à une tentative de **_Build module_** :
  Vérifier que l'environnement de travail et l'IDE sont bien paramétrés pour **Java 11**
- Erreur suite à une tentative de **_maven compile_** :
  Vérifier que l'environnement de travail et l'IDE sont bien paramétrés pour **Java 11**

### 🔴Maintenance
- Dépendances:
  Régulièrement vérifier le fichier pom.xml pour s'assurer que les dependances sont a jour, si non les mettre a jour.
  Site de téléchargement des dépendances maven : https://mvnrepository.com


