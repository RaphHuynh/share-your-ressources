# About `share-your-ressources` 

[![en](https://img.shields.io/badge/lang-en-blue.svg)](./README.md)
[![fr](https://img.shields.io/badge/lang-fr-blue.svg)](./README-fr.md)

This repo is a community project that lets you share resources, tools, applications, courses, etc. that you find interesting.

To keep the repo clean and easy to navigate, here are some guidelines to follow when adding a new resource.

### Making a pull request <a id="making-a-pull-request"></a>

Making a pull request is mandatory to add any new resource:

- Fork the project, a new repository should be created on your github account.
- Clone this repo on your local machine :
  ```bash
  git clone https://github.com/YourUsername/share-your-ressources.git
  ```
- Create a new branch :
  ```bash
  git checkout -b my-new-branch
  ```
- Make your changes locally
- Commit and push your changes
  ```bash
  git add .
  git commit -m "my new commit"
  git push origin my-new-branch
  ```
- Github will propose you to make a pull request, click on the button and fill the form.

If you have any trouble, you can refer to [this tutorial](https://www.digitalocean.com/community/tutorials/how-to-create-a-pull-request-on-github) or ask for help in the [Discord server](https://discord.gg/Htg7jDAGHB).

### Adding a new resource

First, you need to choose the right category and sub-category for your resource. If you can't find a suitable category, you can create a new one.

> **Note:** If you create a new [category or sub-category](#category-format), you must update the [summary](summary-format).

Then, when you have found the right place for your resource, you can add it to the right file:
- `LINK-fr.md` for french resources
- `LINK.md` for english resources

Once you have modified the file, you can make a [pull request](#making-a-pull-request).
Ideally, you should add a description for each resource you add and make it available in both languages.

### Adding a new language

If you want to add a new language, you need to create two files:
- `LINK-language.md` for the resources in your language
- `README-language.md` for the `README` in your language

You also need to add a badge at the beginning of each markdown file:
```md
[![en](https://img.shields.io/badge/lang-en-blue.svg)](./README.md)
[![fr](https://img.shields.io/badge/lang-fr-blue.svg)](./README-fr.md)
[![language](https://img.shields.io/badge/lang-language-blue.svg)](./README-language.md)
```

### Category format <a id="category-format"></a>

Each category must follow this format:
```md
---
## Category <a id="anchorToCategory"></a>
Description of the category (optional)

### Sub-category 1 <a id="anchorToSubCategory1"></a>
Description of the sub-category (optional)

| Description                 | Link                         |
| --------------------------- | ---------------------------- |
| Description of the resource | [Name of the resource](link) |
```

### Summary format <a id="summary-format"></a>

The summary must contain every category and sub-category. It must be updated each time a new category or sub-category is added :
```md
1. [Category 1](#anchorToCategory1)
    - [Sub-category 1](#anchorToSubCategory1)
    - [Sub-category 2](#anchorToSubCategory2)
2. [Category 2](#anchorToCategory2)
    - [Sub-category 1](#anchorToSubCategory1)
    - [Sub-category 2](#anchorToSubCategory2)
```
