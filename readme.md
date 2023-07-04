# Readme / A lire

This repo is a community project that lets you share resources, tools, applications, courses, etc. that you find interesting.

Ce repo est un projet communautaire qui permet de partager les ressources, outils, applications, cours, etc, que l'on trouve interessant.

## To share / Pour partager 

You have to fork the project. Normally a new repository is created on your github account. You need to clone this repo.

Tu dois fork le projet. Normalement un nouveau repository c'est créé sur ton compte github. Tu dois cloner ce repo.

```
git clone git@github.com:votreCompte/copie-du-depot.git
```

### Share a ressource in an existing category /Partager une ressource dans une catégorie déja existante

<h4><u> The sub-category does not exist / La sous-catégorie n'existe pas ?</u></h4>

In this context, the new sub-category must first be created. Next, you'll need to add the new resource to a new sub-category (in the right place)

Dans ce contexte, il faut d'abord créer la nouvelle sous-categorie. Ensuite, il faudra ajouter la nouvelle ressource dans une nouvelle sous-categorie (au bonne endroit).

- create a new sub-category / créer une nouvelle category :

In the file link.md 

```md
1. [Existing Category](#myCategory)
    - [Existing sub-Category](#mysubcategory)
    <!--Add new category-->
    - [my new sub-category](#mynewsubcategory)
```

Dans le fichier lien.md

```md
1. [Category Existante](#monAncreDeLaCategory)
    - [sous-category existante](#monAncre)
    <!--Ajouter une nouvelle category-->
    - [ma nouvelle category](#monNouvelleAncre)
```

- Add the new ressource / ajouter la nouvelle ressource :

In the file link.md

```html
### name of your new sub-category <a id="nameNewSubCategory"></a>

List of ... ( write a description of what your sub-category contains )

<table>
    <thead>
        <tr>
            <th>
               Description
            </th>
            <th>
                Link
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Descriptions of what your resource contain</td>
            <td><a href="link of your ressource">name of your ressource</td>
        </tr>
    </tbody>
</table>
```

Dans le fichier lien.md

```html
### nom de ta sous-categorie <a id="ancre de ta sous-categorie"></a>

Liste de ... ( écrire une description de ce que contient ta sous-categorie)

<table>
    <thead>
        <tr>
            <th>
               Description
            </th>
            <th>
                Lien
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Descriptions de ce que contient ta ressources</td>
            <td><a href="lien de ta ressource">nom de ta ressources</td>
        </tr>
    </tbody>
</table>
```

To finish, simply commit. 

Pour finir, il suffit de commit.

```
git add .
git commit -m "..."
git push
```

<h4><u> The sub-category exists / La sous-catégoerie existe ? </u></h4>

All you have to do is add the resource where you want it.

Il suffit d'ajouter la ressource à l'endroit voulu.

In file link.md

```html
### name of your sub-category <a id="nameSubCategory"></a>

List of ...

<table>
    <thead>
        <tr>
            <th>
               Description
            </th>
            <th>
                Link
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>descriptions of ressource</td>
            <td><a href="link of ressource">name of ressource</td>
        </tr>
        <!--Start of what you need to add-->
        <tr>
            <td>Descriptions of what your resource contain</td>
            <td><a href="link of your ressource">name of your ressource</td>
        </tr>
        <!--End-->
    </tbody>
</table>
```

Dans le fichier lien.md

```html
### nom de la sous-categorie <a id="ancre de la sous-categorie"></a>

Liste de ... 

<table>
    <thead>
        <tr>
            <th>
               Description
            </th>
            <th>
                Lien
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Description d'une ressource deja créé</td>
            <td><a href="lien d'une ressource deja existante">nom</a></td>
        </tr>
        <!--ce que tu dois rajouter et modifier-->
        <tr>
            <td>Descriptions de ce que contient ta ressources</td>
            <td><a href="lien de ta ressource">nom de ta ressources</td>
        </tr>
        <!--Fin de ce que tu dois rajouter et modifier-->
    </tbody>
</table>
```

To finish, simply commit. 

Pour finir, il suffit de commit.

```
git add .
git commit -m "..."
git push
```

<h4><u> The category does not exist / La category n'existe pas ?</u></h4>

Il faut d'abord créer une category, ensuite créer la sous-category, rajouter la ressource puis commit le projet.

You first need to create a category, then create the sub-category, add the resource and then commit the project.

- Create new category / créer une nouvelle categorie :

In file link.md

```md
<h1 align="center">List of link</h1>

## Summary

1. [Ressource pour dev Front](#front-end)
  - [police d'écriture](#font)
  - [image / icon svg](#svg)
  - [design UX/UI](#ux-ui)

2. [Ressource pour dev Back](#back-end)
   - [outils pour les call API](#call-api) 

3. [Ressource pour devops](#devops)
    - [terminal](#terminal)
      - [macos](#terminal-macos)
      - [windows](#terminal-windows)
      - [linux](#terminal-linux)

4. [Intelligence artificielle](#IA)
    - [outils](#outils-ia)

<!--Add-->
NumberOfNewCategory. [Name new Category](#nameCategory)
    - [name of your new sub-category](#nameofsub-category)
<!---->
```

Dans le fichier lien.md

```md
<h1 align="center">Liste liens utiles</h1>

## Sommaire

1. [Ressource pour dev Front](#front-end)
  - [police d'écriture](#font)
  - [image / icon svg](#svg)
  - [design UX/UI](#ux-ui)

2. [Ressource pour dev Back](#back-end)
   - [outils pour les call API](#call-api) 

3. [Ressource pour devops](#devops)
    - [terminal](#terminal)
      - [macos](#terminal-macos)
      - [windows](#terminal-windows)
      - [linux](#terminal-linux)

4. [Intelligence artificielle](#IA)
    - [outils](#outils-ia)

<!--Ajoutes-->
NumeroDeLaCategorie. [Nom de la  Categorie](#AncreDeLaCategorie)
    - [Nom de la sous-categorie](#AncreDeLaSousCategorie)
<!---->
```

- Add ressource / Ajoute la ressource :

In file link.md

```html

 <!--Start of what you need to add-->

## name of your new Category <a id="nameNewCategory">

### name of your sub-category <a id="nameSubCategory"></a>

List of ... (write a content of your sub-category)

<table>
    <thead>
        <tr>
            <th>
               Description
            </th>
            <th>
                Link
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Descriptions of what your resource contain</td>
            <td><a href="link of your ressource">name of your ressource</td>
        </tr>
    </tbody>
</table>

---

<!--End-->
```

Dans le fichier lien.md

```html

 <!--Débur de ce que tu dois ajouter -->

## Nom de la nouvelle categorie <a id="AncreDeTaCategorie">

### Nom de la nouvelle sous categorie <a id="AncreDeTaSousCategorie">

Liste de ... (écrit le contenu de ta sous-categorie.)

<table>
    <thead>
        <tr>
            <th>
               Description
            </th>
            <th>
                Lien
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Description de ce que contient ta ressource</td>
            <td><a href="lien de ta ressource">nom de ta ressource</td>
        </tr>
    </tbody>
</table>

---

<!--End-->
```

To finish, simply commit. 

Pour finir, il suffit de commit.

```
git add .
git commit -m "..."
git push
```