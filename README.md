# Mes projets

Page unique regroupant mes applications web déployées.

## Ajouter ou modifier un projet

Tout est dans [`index.html`](index.html). Les projets sont décrits par un
tableau JavaScript en bas du fichier :

```js
const projets = [
  {
    icone: "📚",
    nom: "Révisions — QCM",
    url: "https://revisions-qcm.vercel.app/",
    note: "QCM générés depuis un cours PDF",
  },
];
```

Ajoutez une entrée, poussez : Vercel redéploie tout seul.

## Technique

Un seul fichier HTML, sans dépendance, sans étape de construction : ni
framework, ni paquet npm, ni police externe. La page s'ouvre directement dans
un navigateur (`index.html`) et se déploie telle quelle.

Elle suit le thème clair ou sombre du système, s'adapte au mobile, et respecte
`prefers-reduced-motion`.

## Déploiement

Sur Vercel, importez le dépôt. Aucune configuration n'est nécessaire : sans
`package.json`, le projet est servi comme un site statique (preset « Other »,
sans commande de construction).
