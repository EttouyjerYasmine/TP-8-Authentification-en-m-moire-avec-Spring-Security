# TP 8 – Authentification en mémoire avec Spring Security

## 📌 Résumé pédagogique

Ce TP présente les bases de **Spring Security** à travers une authentification simple **en mémoire**, en utilisant deux utilisateurs : `admin` et `user`. Vous allez apprendre :

### ✔️ Génération automatique de sécurité par Spring Boot

### ✔️ Configuration d’utilisateurs en mémoire

### ✔️ Définition des règles d’accès selon les rôles

### ✔️ Mise en place de routes protégées

### ✔️ Test des accès via navigateur

---

## 🧩 Étape 1 – Sécurité par défaut

Spring Boot active automatiquement Spring Security et génère :

### • Nom d’utilisateur par défaut : `user`

### • Mot de passe aléatoire affiché dans la console

Exemple :

```
Using generated security password: 2a3c41d7-8c5b-4d5a-a145-5e6f8c9fbd14
```

Toutes les routes sont protégées par défaut.

---

## 🧩 Étape 2 – Créer `SecurityConfig.java`

Fichier : `ma.fstg.security.config.SecurityConfig`

Déclare :

### ✔️ Deux utilisateurs (`admin`, `user`) en mémoire

### ✔️ Leurs rôles

### ✔️ Les règles d’accès

### ✔️ Le formulaire de connexion

---

## 🧩 Étape 3 – Routes à tester

Les routes ajoutées dans le contrôleur :

### • `/` → Accès après connexion

### • `/user/dashboard` → Rôle USER et ADMIN

### • `/admin/dashboard` → Rôle ADMIN uniquement

---

## 🧪 Étape 4 – Comptes de test

### 🔑 Compte utilisateur

* **Username :** `user`
* **Password :** `1111`
* **Accès :** `/user/dashboard`

### 🔑 Compte administrateur

* **Username :** `admin`
* **Password :** `1234`
* **Accès :** `/user/dashboard` et `/admin/dashboard`

---

## ▶️ Lancer les tests

Démarrer l’application puis accéder aux URL suivantes :

### • [http://localhost:8080/](http://localhost:8080/)

### • [http://localhost:8080/user/dashboard](http://localhost:8080/user/dashboard)

### • [http://localhost:8080/admin/dashboard](http://localhost:8080/admin/dashboard)

---

## 📂 Structure du projet

```
src/main/java
 └── ma/fstg/security
       ├── config/SecurityConfig.java
       └── web/HomeController.java
```

---


---

## ✔️ Tester notre travail
-![1](https://github.com/user-attachments/assets/968293ce-f89f-4157-9d81-82045c02d2d5)
-![2](https://github.com/user-attachments/assets/f811bc27-e5fb-4edb-8ff4-0efc6d70dd11)
-![3](https://github.com/user-attachments/assets/c5875aef-80c5-47f9-b1a8-eae1891dd9c1)
