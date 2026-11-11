# StoreIT

Plateforme de stockage et de partage de fichiers inspirée de Google Drive.

![Next.js](https://img.shields.io/badge/-Next.js-black?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/-Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Appwrite](https://img.shields.io/badge/-Appwrite-FD366E?style=for-the-badge&logo=appwrite&logoColor=white)

## Sommaire

1. [À propos](#à-propos)
2. [Stack technique](#stack-technique)
3. [Fonctionnalités](#fonctionnalités)
4. [Installation](#installation)
5. [Structure du projet](#structure-du-projet)
6. [Ce que ce projet m'apprend](#ce-que-ce-projet-mapprend)

## À propos

StoreIT permet à un utilisateur de téléverser, organiser, télécharger et partager ses fichiers (documents, images, vidéos, audio) depuis une interface responsive.

C'est un projet personnel que je développe pour apprendre Next.js (App Router, Server Components, Server Actions) et pour découvrir Appwrite comme backend (authentification, base de données, stockage).

## Stack technique

| Catégorie | Technologies |
|---|---|
| Framework | Next.js, React |
| Langage | TypeScript |
| Backend (BaaS) | Appwrite (Auth, Databases, Storage) |
| UI | Tailwind CSS, shadcn/ui |
| Formulaires | React Hook Form, Zod |

## Fonctionnalités

- [ ] Authentification sans mot de passe par code OTP envoyé par email
- [ ] Inscription, connexion et déconnexion
- [ ] Upload de fichiers (documents, images, vidéos, audio) avec limite de taille
- [ ] Consultation, renommage et suppression de fichiers
- [ ] Téléchargement de fichiers
- [ ] Partage de fichiers avec d'autres utilisateurs par email
- [ ] Dashboard : espace utilisé, fichiers récents, répartition par type
- [ ] Recherche globale
- [ ] Tri des fichiers (date, nom, taille)
- [x] Interface responsive (mobile et desktop)


## Installation

### Prérequis

- [Node.js](https://nodejs.org/)
- npm
- Un compte [Appwrite](https://appwrite.io/) (Cloud ou auto-hébergé)

### Cloner le dépôt

```bash
git clone https://github.com/<ton-utilisateur>/<ton-repo>.git
cd <ton-repo>
```

### Installer les dépendances

```bash
npm install
```

### Configurer les variables d'environnement

Crée un fichier `.env.local` à la racine du projet :

```env
NEXT_PUBLIC_APPWRITE_ENDPOINT="https://cloud.appwrite.io/v1"
NEXT_PUBLIC_APPWRITE_PROJECT=""
NEXT_PUBLIC_APPWRITE_DATABASE=""
NEXT_PUBLIC_APPWRITE_USERS_COLLECTION=""
NEXT_PUBLIC_APPWRITE_FILES_COLLECTION=""
NEXT_PUBLIC_APPWRITE_BUCKET=""
NEXT_APPWRITE_KEY=""
```

Renseigne les valeurs depuis la console Appwrite : crée un projet, une base de données avec deux collections (utilisateurs et fichiers), un bucket de stockage et une clé d'API.


### Lancer le projet

```bash
npm run dev
```

L'application est accessible sur [http://localhost:3000](http://localhost:3000).

## Structure du projet

```
.
├── app/            # Routes et pages (App Router)
├── components/     # Composants React (dont components/ui pour shadcn)
├── lib/
└── public/         # Images et icônes
```

## Ce que ce projet m'apprend

- Le routage et la structure d'une application avec l'App Router de Next.js
- La différence entre Server Components et Client Components
- L'utilisation des Server Actions pour communiquer avec le backend
- L'intégration d'un BaaS (Appwrite) : authentification, base de données et stockage de fichiers
- La validation de formulaires typés avec Zod et React Hook Form
- La création d'une interface responsive avec Tailwind CSS et shadcn/ui

## Auteur

Hugo, étudiant en BUT Informatique à l'IUT de Lille.
GitHub : [Montsy744](https://github.com/Montsy744)
