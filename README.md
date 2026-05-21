# powerbi-components

Composants Jekyll réutilisables pour intégrer des dashboards **Power BI** dans un portfolio statique.

## Contenu

```
powerbi-components/
├── _includes/
│   └── powerbi-dashboard.html   # composant principal
├── _sass/
│   └── _powerbi.scss            # styles optionnels
└── examples/
    └── projet-immobilier.md     # exemple d'utilisation dans une page projet
```

## Installation dans votre portfolio Jekyll

**1. Copier le composant**

```bash
cp _includes/powerbi-dashboard.html <votre-portfolio>/_includes/
cp _sass/_powerbi.scss <votre-portfolio>/_sass/
```

**2. Importer le SCSS** dans votre fichier principal (ex. `assets/css/main.scss`) :

```scss
@import "powerbi";
```

**3. Utiliser dans n'importe quelle page**

```markdown
{% include powerbi-dashboard.html
  title="Titre de votre dashboard"
  description="Description du projet."
  embed_url="https://app.powerbi.com/view?r=VOTRE_CODE_EMBED"
  data_source="Nom de la source"
  source_url="https://lien-vers-la-source.fr"
%}
```

## Obtenir l'URL d'embed Power BI

1. Ouvrir votre rapport dans **Power BI Service**
2. `Fichier > Incorporer le rapport > Publier sur le web (public)`
3. Lire l'avertissement et confirmer
4. Copier l'URL depuis le bloc `<iframe>` généré

> **Important :** ne publiez que des dashboards basés sur des données 100% publiques.
> La fonctionnalité "Publier sur le web" rend vos données accessibles à tous.

## Paramètres du composant

| Paramètre | Requis | Description |
|-----------|--------|-------------|
| `title` | ✅ | Titre affiché au-dessus du dashboard |
| `description` | — | Description courte du projet |
| `embed_url` | ✅ | URL d'embed fournie par Power BI |
| `data_source` | ✅ | Nom de la source de données |
| `source_url` | ✅ | URL vers la source ouverte |
| `height` | — | Hauteur de l'iframe (défaut : `600px`) |
