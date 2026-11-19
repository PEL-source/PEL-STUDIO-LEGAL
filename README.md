# PEL Studio — pages légales

Dépôt **public** des informations légales des jeux édités par PEL Studio
(entreprise individuelle PERIO).

## Publication

Hébergement : **GitHub Pages** via le workflow Actions `.github/workflows/pages.yml`
(déclenché sur chaque push sur `main`).

Site : <https://pel-source.github.io/PEL-STUDIO-LEGAL/>

## Documents disponibles

| Jeu | Document | URL |
|---|---|---|
| Démineur Mobile | Politique de confidentialité | [demineur/confidentialite/](https://pel-source.github.io/PEL-STUDIO-LEGAL/demineur/confidentialite/) |
| Predator Eleven League | *(à venir)* | — |

## Contact

[contact.predatorelevenleague@gmail.com](mailto:contact.predatorelevenleague@gmail.com)

## Contenu

Ce dépôt ne contient **que** des pages HTML légales. Aucun code source, asset
ou fichier interne des jeux n’y est publié.

## Activation GitHub Pages (obligatoire, une fois)

Le workflow Actions **ne peut pas** activer Pages la première fois : le
`GITHUB_TOKEN` reçoit `Resource not accessible by integration` sur
`POST /repos/.../pages`. Une activation manuelle par le propriétaire du dépôt
est indispensable.

1. Ouvrir [Settings → Pages](https://github.com/PEL-source/PEL-STUDIO-LEGAL/settings/pages)
   en étant connecté avec le compte **PEL-source** (droits admin).
2. Sous **Build and deployment** → **Source**, choisir **GitHub Actions**.
3. Enregistrer. L’environnement `github-pages` peut déjà exister ; ce n’est pas
   suffisant tant que la source Pages n’est pas définie.
4. Relancer le workflow :
   - soit [Actions → Deploy GitHub Pages → Run workflow](https://github.com/PEL-source/PEL-STUDIO-LEGAL/actions/workflows/pages.yml)
     (branche `main`) ;
   - soit un push sur `main`.
5. Vérifier que le run est **vert**, puis ouvrir  
   `https://pel-source.github.io/PEL-STUDIO-LEGAL/demineur/confidentialite/`  
   (HTTPS, HTTP 200).

### Variante sans Actions

Si vous préférez un déploiement immédiat depuis la branche :

1. Settings → Pages → Source : **Deploy from a branch**
2. Branch : `main` / folder : `/ (root)` → **Save**
3. Attendre 1–2 minutes, puis vérifier la même URL.
