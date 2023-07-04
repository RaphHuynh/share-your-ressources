# A propos de `share-your-ressources` 

Ce repo est un projet communautaire qui vous permet de partager des ressources, outils, applications, cours, etc. que vous trouvez intéressants.

Pour garder le repo propre et facile à naviguer, voici quelques directives à suivre lors de l'ajout d'une nouvelle ressource.

### Faire une pull-request <a id="making-a-pull-request"></a>

Pour ajouter une ressource, il est obligatoire de faire une pull-request :

- Fork le projet, un nouveau dépôt devrait être créé sur votre compte github.
- Cloner ce repo sur votre machine locale :
  ```bash
  git clone https://github.com/TonPseudo/share-your-ressources.git
  ```
- Créer une nouvelle branche :
  ```bash
  git checkout -b my-new-branch
  ```
- Faire vos modifications localement
- Commit et push vos modifications :
  ```bash
  git add .
  git commit -m "my new commit"
  git push origin my-new-branch
  ```
- Github vous proposera de faire une pull-request, cliquez sur le bouton et remplissez le formulaire.

Si tu as un problème, tu peux te référer à [ce tutoriel](https://www.digitalocean.com/community/tutorials/how-to-create-a-pull-request-on-github) ou demander de l'aide sur le [serveur Discord](https://discord.gg/Htg7jDAGHB).

### Ajouter une nouvelle ressource

Tout d'abord, vous devez choisir la bonne catégorie et sous-catégorie pour votre ressource. Si vous ne trouvez pas de catégorie appropriée, vous pouvez en créer une nouvelle.

> **Note:** Si vous créez une nouvelle [catégorie et/ou sous-catégorie](#category-format), vous devrez modifier le [sommaire](summary-format).

Ensuite, lorsque vous avez trouvé le bon endroit pour votre ressource, vous pouvez l'ajouter au bon fichier :
- `LINK-fr.md` pour les ressources en français
- `LINK.md` pour les ressources en anglais

Une fois les modifications faites, vous pouvez faire une [pull-request](#making-a-pull-request).
Idéalement, vous devriez décrire vos changements et les faire en chaque langue.

### Ajouter une nouvelle langue

Si vous souhaitez ajouter une nouvelle langue, vous devez créer un nouveau fichier :
- `LINK-langage.md` pour les ressources dans votre langue
- `README-langage.md` pour le fichier `README.md` dans votre langue

Une fois le fichier créé, vous pouvez ajouter un badge dans le fichier `README.md` :
```md
[![en](https://img.shields.io/badge/lang-en-blue.svg)](./README.md)
[![fr](https://img.shields.io/badge/lang-fr-blue.svg)](./README-fr.md)
[![langage](https://img.shields.io/badge/lang-langage-blue.svg)](./README-langage.md)
```

### Format des catégories <a id="category-format"></a>

Chaque catégorie doit suivre ce format :
```md
---
## Catégorie <a id="ancreVersCategorie1"></a>
Description de la catégorie (optionelle)

### Sous-catégorie 1 <a id="ancreVersSousCategorie1"></a>
Description de la sous-catégorie (optionelle)

| Description                 | Link                        |
| --------------------------- | --------------------------- |
| Description de la ressource | [Nom de la ressource](lien) |
```

### Format du sommaire <a id="summary-format"></a>

Le sommaire doit contenir chaque catégorie et sous-catégorie et doit être mis à jour :
```md
1. [Catégorie 1](#ancreVersCategorie1)
    - [Sous-catégorie 1](#ancreVersSousCategorie1)
    - [Sous-catégorie 2](#ancreVersSousCategorie2)
2. [Catégorie 2](#ancreVersCategorie2)
    - [Sous-catégorie 1](#ancreVersSousCategorie1)
    - [Sous-catégorie 2](#ancreVersSousCategorie2)
```
