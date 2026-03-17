# Chambres d'Hôtes de  — Site MkDocs

Site web des Chambres d'Hôtes chbh, construit avec [MkDocs](https://www.mkdocs.org/) et le thème [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

---

## 📁 Structure du projet

```
chbh-mkdocs/
├── mkdocs.yml                    ← Configuration principale
├── docs/
│   ├── assets/
│   │   ├── images/               ← Logo et images locales (à ajouter)
│   │   └── stylesheets/
│   │       └── extra.css         ← CSS personnalisé
│   │   
│   ├── chambres/
│   │   ├── index.md              ← Vue d'ensemble des chambres
│   │   ├── chambre-1.md            ← Chambre 1
│   │   ├── chambre-2.md            ← Chambre 2
│   │  
│   └── tbh/
│       ├── petits-dejeuners.md   ← Petits déjeuners
│       ├── tables-dhotes.md      ← Tables d'hôte
│       ├── restaurants.md        ← Restaurants environnants
│       └── productions-locales.md← Productions locales
│   ├── apropos.md              ←
│   ├── contact.md              ←
│   ├── infos-pratiques.md              ←
│   ├── maison.md              ←
│   ├── jardin.md              ←
│   ├── alentours.md              ← Activités aux alentours
│   ├── index.md                  ← Page d'accueil
│   ├── localisation.md           ← Localisation & trajets
│   ├── tarifs.md                 ← Tarifs
│   ├── reservations.md           ← Réservations       
└── README.md                     ← Ce fichier
```

---

## 🚀 Installation

### Prérequis
- Python 3.8 ou plus récent
- pip

### Étapes

```bash
# 1. Installer MkDocs et le thème Material
pip install mkdocs-material

# 2. Se placer dans le dossier du projet
cd templerie-mkdocs

# 3. Lancer le serveur de développement local
mkdocs serve
```

Le site est alors accessible sur **http://127.0.0.1:8000**

---

## 🛠 Modifier le contenu

Chaque page du site correspond à un fichier `.md` (Markdown) dans le dossier `docs/`. Pour modifier une page :

1. Ouvrez le fichier `.md` correspondant avec n'importe quel éditeur de texte (Notepad, VS Code, Obsidian…)
2. Modifiez le contenu en Markdown
3. Sauvegardez — le site se recharge automatiquement si `mkdocs serve` est actif

### Syntaxe Markdown de base

```markdown
# Titre principal
## Sous-titre
### Section

Texte normal en paragraphe.

**gras** — *italique* — [lien](https://example.com)

- liste à puces
- item 2

| Colonne 1 | Colonne 2 |
|---|---|
| valeur | valeur |
```

### Fonctionnalités spéciales (Material)

```markdown
!!! info "Titre de la note"
    Contenu de la note informative.

!!! warning "Attention"
    Message d'avertissement.

!!! success "Succès"
    Message de succès.

!!! tip "Astuce"
    Conseil pratique.
```

---

## 🖼 Ajouter des images



Pour utiliser des images locales (recommandé) :

1. Placez vos images dans `docs/assets/images/`
2. Référencez-les dans vos pages avec un chemin relatif :
   ```markdown
   ![Description](assets/images/mon-image.jpg)
   ```
   ou depuis un sous-dossier :
   ```markdown
   ![Description](../assets/images/mon-image.jpg)
   ```

---

## 📄 Ajouter une page

1. Créez un nouveau fichier `.md` dans le bon dossier de `docs/`
2. Ajoutez-le dans la navigation du fichier `mkdocs.yml` :
   ```yaml
   nav:
     - Ma nouvelle page: dossier/ma-page.md
   ```

---

## 🌐 Déploiement

### Option 1 : GitHub Pages (gratuit)

```bash
# Déployer sur GitHub Pages
mkdocs gh-deploy
```

### Option 2 : Générer le site statique

```bash
# Générer le site dans le dossier /site
mkdocs build
```

Le dossier `site/` contient des fichiers HTML statiques que vous pouvez déposer sur n'importe quel hébergeur web (OVH, Infomaniak, etc.).

---

## ⚙️ Configuration principale (mkdocs.yml)

Les réglages importants dans `mkdocs.yml` :

| Paramètre | Description |
|---|---|
| `site_name` | Nom du site (onglet navigateur) |
| `site_url` | URL officielle du site |
| `theme.palette.primary` | Couleur principale (actuellement `teal`) |
| `theme.palette.accent` | Couleur d'accent (actuellement `red`) |
| `nav` | Structure de la navigation |

---

## 📞 Contact

****  
  
Tél : 
Email :
# chbh.fr
