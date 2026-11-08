# LandingPageDeepWater

La landing page de DeepWater, le terminal de marché. Une seule page, `index.html`, sans bibliothèque ni étape de compilation. Français et anglais (bouton FR / EN en haut).

## Voir la page chez soi

Ouvrir `index.html` dans un navigateur suffit. Pour la servir comme un vrai site :

```sh
npx http-server -p 4173
```

Puis ouvrir http://localhost:4173.

## Ce qu'il y a dedans

- `index.html` : la page. Les textes français sont dans le HTML, les textes anglais dans le dictionnaire du script, en bas du fichier.
- `assets/logo.svg` : l'icône de DeepWater, copiée de `resources/icon/deepwater.svg` dans le dépôt DeepWater.
- `assets/og.png` : l'image (1200 x 630) qui s'affiche quand on partage le lien.

La page couvre tout DeepWater : l'ouverture, la plongée (trois profondeurs), la visite des quatorze onglets, le globe, les sources et la fraîcheur des données, l'IA locale, l'application sur l'ordinateur, le code, les chiffres et les questions.

## Avant de la mettre en ligne

- Remplacer les deux adresses `example.invalid` (`og:url` et `og:image`) à l'endroit marqué `DEPLOY STEP` dans `index.html` par l'adresse réelle du site.
- Les boutons Télécharger mènent à la page Releases du dépôt DeepWater : il faut y avoir publié une version pour qu'elle ne soit pas vide.

## Choix de conception

- Un seul mot porte la page : la profondeur. Les couleurs viennent de la palette Abyss de l'app.
- Les aperçus de l'interface sont des dessins vectoriels, pas des captures d'écran, et la page le dit.
- La page respecte « réduire les animations » et fonctionne au clavier et au toucher.
