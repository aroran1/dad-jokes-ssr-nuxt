# dad-jokes-ssr-nuxt

Nuxt.js is a framework to work with Vue. This enables key features for a UI application:
- Universal Apps / Server Side Rendering
- SEO optimization
- Control of head, title, meta etc
- Simple page routing

When a SPA applications load on a browser the serach engine crawlers usually see a blank page which doesn't help with SEO. Nuxt would make your application into a universal application which will preload your app on the server which will help SEO, page load speed with many other benefits like meta, title etc.

Nuxt use Vue meta library behind the scenes to load metao / title information for the pages. You cna also provide config for the default information.

With nuxt in place you don't have to configure the routing explicitly. Instead it proviodes you with a pages folder and and page (or layout) craeted in this folder will automatically be added to your routing. For example if you craee about.vue file inside pages you can hist http://xyx.com/about on the server path. Not complicated routing set-up is required with all teh dynamic functionality still being available.

## Other Features of NUXT

- Bundled with vue-router, Vuex, vue-meta and more
- Choice of universal or SPA
- Choice to include Express or other backend framework
- Choice to include Bootstrap or other UI framework
- Automatic code-splittling, Babel transpile, minification, HMR, Sass integration
- Easy build `nuxt generate` creates dist folder for deployment

Docs - https://nuxtjs.org/

API - https://icanhazdadjoke.com/api

Typescript - https://typescript.nuxtjs.org/cookbook/components/

**********************************
## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).


### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).


**************************************
