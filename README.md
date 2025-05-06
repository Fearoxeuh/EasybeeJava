# 📦 Easybee - Gestion de Stock & Commandes

Easybee est une application Java de bureau qui permet la gestion de produits, commandes, et utilisateurs. Elle est conçue pour les petites entreprises souhaitant suivre leurs stocks et gérer leurs commandes efficacement.

---

## 🔧 Prérequis

- Java JDK 17 ou supérieur
- MySQL Server
- Un IDE Java (ex : IntelliJ IDEA, Eclipse) ou terminal
- [Git (optionnel)](https://git-scm.com/)

---

## 🖥️ Installation

### 1. Clonez le projet (ou décompressez l'archive)

```bash
git clone https://votre-repo/easybee.git
cd easybee
```

### 2. Importez dans votre IDE

- Ouvrez le dossier `EasybeeJava-main`
- Configurez le JDK (Java 17 recommandé)
- Ajoutez les fichiers `.jar` du dossier `lib/` au classpath du projet

### 3. Configurez la base de données

- Lancez votre serveur MySQL
- Exécutez le script SQL :

```sql
-- Dans un client MySQL
SOURCE path_to/EasybeeJava-main/easybee_projet2.sql;
```

- Vérifiez que les identifiants dans `src/utils/ConnexionBdd.java` correspondent à votre configuration locale (host, port, user, password)

### 4. Compilez et exécutez

#### Avec un IDE :
- Exécutez la classe `App.java` dans le package `app`

#### En ligne de commande :
```bash
javac -cp "lib/*" -d bin src/**/*.java
java -cp "bin:lib/*" app.App
```

---

## 🧪 Fonctionnalités principales

- Authentification des utilisateurs
- Ajout, suppression, modification de produits
- Passation et suivi des commandes
- Interface graphique intuitive en Java Swing

---

## 📂 Structure du projet

```
EasybeeJava-main/
├── lib/                # Bibliothèques externes (JDBC, BCrypt)
├── src/                # Code source Java
│   ├── app/            # Point d'entrée de l'application
│   ├── dao/            # Accès à la base de données
│   ├── model/          # Modèles de données
│   ├── ui/             # Interfaces utilisateurs
│   └── utils/          # Utilitaires (connexion BDD)
├── easybee_projet2.sql # Script SQL pour la base de données
├── logoEasybee.png     # Logo de l'application
```

---

## 🤝 Auteurs

Projet développé par [Hedouin Enzo, Leo Carboni] dans le cadre du BTS SIO.
