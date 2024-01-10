# Projet ergonomie

Site web réalisé dans le cadre du cours *Conception de services et ergonomie*.

## 🚀 Structure du projet

Le projet se structure ainsi :

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
├── README.md
├── package.json
└── tsconfig.json
```

Tous les fichiers `.astro` ou `.md` dans `src/pages/` seront exposés avec leur nom de fichier comme route.

Le dossier `src/components/` contient tous les composants réutilisables.

Le dossier `src/content/` contient des fichiers Markdown pour alimenter le blog.

Toutes les ressources comme les images sont présents dans le dossier `public/`.

## 🧞 Commandes

Voici l'ensemble des commandes disponibles :

| Command                   | Action                                                   |
| :------------------------ | :------------------------------------------------------- |
| `npm install`             | Installe les dépendances                                 |
| `npm run dev`             | Démarre un serveur de développement sur `localhost:4321` |
| `npm run build`           | Construit le site de production dans `./dist/`           |
| `npm run preview`         | Affiche le site de production construit                  |
