# <img alt="CryptoLogique Logo" src="/public/icons/logo.svg" height="40"/> Quasar Easy-Compta App🔒

Application web de type [SSR](https://vuejs.org/guide/scaling-up/ssr.html) multi-plateforme permettant de générer des factures et gérer les données financières à travers des transactions sécurisées vers des bases de données distantes/portables.

## Dépendances

- Quasar : [![npm version](https://badge.fury.io/js/quasar.svg)](https://badge.fury.io/js/quasar)

- Capacitor/core : [![npm version](https://badge.fury.io/js/@capacitor%2Fcore.svg)](https://badge.fury.io/js/@capacitor%2Fcore)

- Axios: [![npm version](https://badge.fury.io/js/axios.svg)](https://badge.fury.io/js/axios)

- Pinia : [![npm version](https://badge.fury.io/js/pinia.svg)](https://badge.fury.io/js/pinia)

- Pinia-plugin-persistedstate : [![npm version](https://badge.fury.io/js/pinia-plugin-persistedstate.svg)](https://badge.fury.io/js/pinia-plugin-persistedstate)
 
- Sequelize : [![npm version](https://badge.fury.io/js/sequelize.svg)](https://badge.fury.io/js/sequelize)

- Vue : [![npm version](https://badge.fury.io/js/vue.svg)](https://badge.fury.io/js/vue)

- Vue-I18n : [![npm version](https://badge.fury.io/js/vue-i18n.svg)](https://badge.fury.io/js/vue-i18n)

- Vue-Router : [![npm version](https://badge.fury.io/js/vue-router.svg)](https://badge.fury.io/js/vue-router)

### Installation

 #### Web

 Mettre à jour le fichier **envs/.env.production** avec les informations liées à votre base de données.

 **PREMIÈRE UTILISATION**

 Changer la variable *-INIT-* à **true** pour initialiser les données principales de l'application.

 **Ne pas oublier de remettre cette variable à 'false' avant de de redémarrer votre serveur web.**

 `> npm run build:web`

 `> cd dist/ssr`

 `> npm install`

 `> npm run start` --> Cette ligne va démarrer votre serveur web.

 #### Mobile

  - Ios : Fabrication de l'application pour mobiles et tablettes IOS.

  `> npm run build:ios`

  - Android : Fabrication de l'application pour mobiles et tablettes ANDROID.

  `> npm run build:and`

## Usage
 
 ### Web

 Démarrer le serveur web.

 Se rendre sur votre navigateur à l'adresse suivante **%PUB_APP_URL%**.

 *- __NOTE:__ PUB_APP_URL est une varable d'environnement se trouvant dans le fichier __envs/.env.production__ -*

 ### Mobile

 Après la fabrication de l'application, vous pouvez plublier votre application sur l'apple/play store.

 Suivez la documention sur [quasar doc](https://quasar.dev/quasar-cli-vite/developing-capacitor-apps/publishing-to-store), pour publier une application sur le store. 

 Vous pouvez également utiliser votre application sans la publier en récupérant le fichier exécutable de votre application:

 - *src-capacitor/android/app/build/outputs/apk/debug/app-debug.apk* **pour Android**.
 - *__%MACOSLibraryFolder%__/Developer/Xcode/DerivedData/App-__%hash%__/Build/Products/App* **pour IOS via Xcode**.