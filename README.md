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

1.15 'vercel secrets add secretvar2 0'    On crée la variable secrète
	'vercel env add secret secretvar2 production'   On la déplace dans le bon environnement de travail
	

1.16 Les 3 environnements sont Production, Preview et Development
On utilise d'abord development puis on test sur preview pour finir par produire sur Production.
Ainsi on évite tout problème.

1.18 'https://vercelq18.vercel.app'

1.19 Un pull-request est l'envoi de modifications de projet. On va venir comparer le projet déjà
en place avec les fichiers qu'on envoien en créant une nouvelle branche. Ainsi on donne une proposition de l'aspect
que pourrait avoir le projet sans le modifier directement. 

Après la pull-request reçu par gitHub, vercel va déployer celle-ci dans l'environnement de Preview afin de tester le projet. Il trigger l'environnement Preview.

1.20 Lorsque l'on merge, la pull-request est déployée vers l'environnement de production.
Le test ayant été fructueux lors de l'étape précèdente.

1.21
La branche master main correspond à l'environnement de production
La branche "Branchage" secondaire correspond à l'environnement de développement.
 
 L'utilisation de pull-requests permet de s'assurer de la fiabilité des données avant de 
 venir écraser le projet master en utilisant le merge. On a aussi la possibilité de merge les branches quand on le souhaite et non pas en temps réel.
 
 Workflow d'une feature:
 - On vient modifier la branche qui est dans l'environnement de développement
 - On envoie les modifications en faisant un commit puis un push
 - On pull-request les modifications puis on les merge afin de les valider dans l'environnement de production.
 - On pull en modifiant la branche master.
 
 1.22
 Le serverless est le fait que le fournisseur de services cloud soit responsable de l'execution d'une partie du code en allouant dynamiquement les ressources.
 Le code est déclenché par des triggers.