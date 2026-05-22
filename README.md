# powerbi-components

Ressources pour intégrer des dashboards **Power BI** dans un portfolio GitHub Pages — compatibles avec les deux approches du Module 2 : portfolio HTML monofichier et portfolio Quarto.

## Contenu

```
powerbi-components/
├── examples/
│   ├── html/
│   │   └── competitive-marketing-analysis.html   # page projet pour portfolio HTML
│   └── quarto/
│       └── competitive-marketing-analysis.qmd    # page projet pour portfolio Quarto
├── pbix/
│   └── Competitive Marketing Analysis.pbix       # rapport de démonstration (Microsoft)
└── index.html                                    # démo standalone GitHub Pages
```

## Approche 1 — Portfolio HTML monofichier

Copiez `examples/html/competitive-marketing-analysis.html` à la racine de votre repo portfolio, puis adaptez :

1. Remplacez `VOTRE_URL_EMBED_ICI` par l'URL fournie par Power BI
2. Recopiez votre `<nav>` et votre `<footer>` depuis `index.html`
3. Ajoutez une carte projet dans `index.html` :

```html
<div class="project-card">
  <h3>Competitive Marketing Analysis</h3>
  <p>Répartition des ventes $32K par canal — ROI comparatif et tendances mensuelles.</p>
  <div>
    <span class="tag">Power BI</span>
    <span class="tag">Data Visualisation</span>
  </div>
  <div class="project-links">
    <a href="competitive-marketing-analysis.html">Voir le dashboard →</a>
  </div>
</div>
```

4. Commitez et poussez — GitHub Pages met à jour en 2-3 minutes.

## Approche 2 — Portfolio Quarto

Copiez `examples/quarto/competitive-marketing-analysis.qmd` à la racine de votre repo portfolio, puis :

1. Remplacez `VOTRE_URL_EMBED_ICI` par l'URL fournie par Power BI
2. Ajoutez la page dans `_quarto.yml` :

```yaml
website:
  navbar:
    left:
      - href: competitive-marketing-analysis.qmd
        text: Dashboard BI
```

3. Commitez et poussez — GitHub Actions déclenche le build automatiquement.

## Obtenir l'URL d'embed Power BI

1. Ouvrir votre rapport dans **Power BI Service**
2. `Fichier > Incorporer le rapport > Publier sur le web (public)`
3. Lire l'avertissement et confirmer
4. Copier l'URL depuis le bloc `<iframe>` généré

> **Important :** ne publiez que des dashboards basés sur des données 100% publiques.
> La fonctionnalité "Publier sur le web" rend l'intégralité de vos données accessible à tous.
