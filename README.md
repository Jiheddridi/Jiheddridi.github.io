# Jihed Dridi — Cloud & DevOps Portfolio

Portfolio bilingue (anglais / français) de Jihed Dridi, étudiant ingénieur spécialisé en cloud, DevOps, Kubernetes, GitOps et monitoring.

## Développement local

```bash
pnpm install
pnpm dev
```

Vérification et build de production :

```bash
pnpm check
pnpm build
```

## Déploiement GitHub Pages

Le workflow `.github/workflows/deploy-pages.yml` construit automatiquement le site et le publie sur GitHub Pages à chaque push sur `main`.

Dans GitHub, ouvrir **Settings → Pages**, choisir **GitHub Actions** comme source de déploiement, puis attendre la fin du workflow.

Le dépôt est prévu pour l’utilisateur GitHub [`Jiheddridi`](https://github.com/Jiheddridi) et le domaine `jihed-dridi.io`.

## DNS pour `jihed-dridi.io`

Chez le registrar du domaine :

- créer quatre enregistrements **A** pour `@` vers `185.199.108.153`, `185.199.109.153`, `185.199.110.153` et `185.199.111.153` ;
- créer un enregistrement **CNAME** pour `www` vers `Jiheddridi.github.io` ;
- supprimer les anciens enregistrements conflictuels pour `@` et `www` ;
- dans GitHub Pages, activer **Enforce HTTPS** après propagation DNS.

La propagation peut prendre plusieurs heures. Le fichier `client/public/CNAME` conserve le domaine après chaque build.

## Contenu et sources

Les informations affichées proviennent du CV et des dépôts publics déjà associés au projet. Le profil LinkedIn est relié comme source complémentaire, mais aucune donnée non vérifiable n’a été ajoutée lorsque LinkedIn demandait une session.

## Licence

MIT
