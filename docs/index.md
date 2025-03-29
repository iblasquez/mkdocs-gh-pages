# MkDocs et de MkDocs Material en quelques mots

- Site MkDocs : <https://www.mkdocs.org>
- Site Material for MkDocs : <https://squidfunk.github.io/mkdocs-material/>

## 🧱 MkDocs

MkDocs est un **générateur de documentation statique** écrit en Python. Il transforme des fichiers Markdown (`.md`) en un site web statique.

**Caractéristiques :**

- Configuration simple via `mkdocs.yml`
- S'appuye sur des fichiers Markdown
- Génère un site web navigable
- Vient avec un **thème de base** simple appelé **mkdocs**

**Installation :**

```bash
pip install mkdocs
```

**Commandes typiques :**

```bash
mkdocs new # crée un nouveau projet de documentation
mkdocs serve # démarre un serveur local avec rechargement automatique à chaque modification
mkdocs build # génère le site statique dans le dossier `site/`
```

**Structure pour un projet MkDocs :**

``` { .sh .no-copy }
.
├─ docs/        # dossier contenant les fichiers markdown
│  └─ index.md  # page d'accueil
└─ mkdocs.yml   # configuration du site
```

## 🎨 MkDocs Material

`mkdocs-material` (ou Material for MkDocs) est un **thème riche en fonctionnalités** pour MkDocs, inspiré par le Material Design de Google.

**Caractéristiques :**

- Design moderne et responsive
- Navigation améliorée (recherche instantanée, menu déroulant, table des matières à droite…)
- Prise en charge du **mode sombre**, du **versioning**, des **admonitions** (encadrés stylisés comme info, avertissement…)
- Intégration possible avec **Mermaid**, **PlantUML**, **Jupyter Notebooks**, etc.
- Personnalisation facile via le fichier `mkdocs.yml`

**Installation :**

```bash
pip install mkdocs-material
```

*Remarque :* **mkdocs-material** *installe automatiquement les versions compatibles de toutes les dépendances : MkDocs, Markdown, Pygments et les extensions Markdown pour Python en s'efforçant de prendre en charge les dernières versions : il n’est donc pas nécessaire d'installer ces paquets séparément.*
Ainsi, installer directement **mkdocs-material** ne nécessite pas d'installer mkdocs.

**Prise en compte du theme material par MkDocs :**

Pour être pris en compte par MkDocs, le thème **material** devra être ajouté dans le fichier de configuration **`mkdocs.yml`** :

```yaml
theme:
  name: material
```
