![Angular Logo](https://github.com/vercel/vercel/blob/master/packages/frameworks/logos/angular.svg)

# Angular Example

This directory is a brief example of an [Angular](https://angular.io/) app that can be deployed with Vercel and zero configuration.

## Deploy Your Own

Deploy your own Angular project with Vercel.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/vercel/vercel/tree/master/examples/angular)

_Live Example: https://angular.now-examples.now.sh_

### How We Created This Example

To get started with Angular, you can use the [Angular CLI](https://cli.angular.io/) to initialize the project:

```shell
$ ng new
```


1.4 'vercel -v'

1.5 'vercel init angular'

1.6 'cd angular && vercel'

1.7 'vercel ls tdvercel'     tdvercel est le nom du projet

1.8 'vercel logs tdvercel-8d9r6xmyl.vercel.app'   

1.9 'vercel inspect tdvercel-8d9r6xmyl.vercel.app'
On obtient les infos sur le déploiement du projet telles que la structure des fichiers, les chemins, l'état,...

1.10 Les variables d'environnement servent à configurer l'outil déployé avec Vercel à l'aide de paramètres en fonction de l'environnement.

1.11 'vercel env add plain var1 production'

1.12 'vercel env ls'

1.13 Les secrets sont faits pour transmettre des infos secretes via les variables d'environnement secrètes.
Ces variables sont invisibles car chiffrées.

1.15 'vercel secrets add secretvar2 0'
	'vercel env add secret secretvar2 production'

1.16 