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

## Config settings
`npx create-nuxt-app <project-name>` <br />
? Project name: (nuxt-test) <br />
? Programming language: (Use arrow keys) <br />
  ❯ ◯ JavaScript <br />
    ◯ TypeScript <br />
? Package manager: (Use arrow keys) <br />
  ❯ ◯ Yarn <br />
    ◯ Npm <br />
UI framework: (Use arrow keys) <br />
  ❯ ◯ None <br />
    ◯ Ant Design Vue <br />
    ◯ BalmUI <br />
    ◯ Bootstrap Vue <br />
    ◯ Buefy <br />
    ◯ Chakra UI <br />
    ◯ Element <br />
    ◯ Framevuerk <br />
    ◯ Oruga <br />
    ◯ Tachyons <br />
    ◯ Tailwind CSS <br />
    ◯ Windi CSS <br />
    ◯ Vant <br />
    ◯ View UI <br />
    ◯ Vuetify.js<br />
? Nuxt.js modules: (Press <space> to select, <a> to toggle all, <i> to invert selection) <br />
  ❯ ◯ Axios - Promise based HTTP client <br />
    ◯ Progressive Web App (PWA) <br />
    ◯ Content - Git-based headless CMS <br />
? Linting tools: (Press <space> to select, <a> to toggle all, <i> to invert selection) <br />
  ❯ ◯ ESLint <br />
    ◯ Prettier <br />
    ◯ Lint staged files <br />
    ◯ StyleLint <br />
    ◯ Commitlint <br />
? Testing framework: (Use arrow keys) <br />
  ❯ ◯ None <br />
    ◯ Jest <br />
    ◯ AVA <br />
    ◯ WebdriverIO <br />
    ◯ Nightwatch <br />
? Rendering mode: (Use arrow keys) <br />
  ❯ ◯ Universal (SSR / SSG) <br />
    ◯ Single Page App <br />
? Deployment target: (Use arrow keys) <br />
  ❯ ◯ Server (Node.js hosting) <br />
    ◯ Static (Static/Jamstack hosting) <br />
? Development tools: (Press <space> to select, <a> to toggle all, <i> to invert selection) <br />
  ❯ ◯ jsconfig.json (Recommended for VS Code if you're not using typescript) <br />
    ◯ Semantic Pull Requests <br />
    ◯ Dependabot (For auto-updating dependencies, GitHub only) <br />
? Continuous integration: (Use arrow keys) <br />
  ❯ ◯ None <br />
    ◯ GitHub Actions (GitHub only) <br />
    ◯ Travis CI <br />
    ◯ CircleCI <br />
? Version control system: (Use arrow keys) <br />
  ❯ ◯ Git <br />
    ◯ None <br />

Sample Package.json
```
{
  "name": "nuxt-test",
  "version": "1.0.0",
  "private": true,
  "scripts": {
    "dev": "nuxt",
    "build": "nuxt build",
    "start": "nuxt start",
    "generate": "nuxt generate",
    "test": "jest"
  },
  "dependencies": {
    "core-js": "^3.15.1",
    "nuxt": "^2.15.7"
  },
  "devDependencies": {
    "@vue/test-utils": "^1.2.1",
    "babel-core": "7.0.0-bridge.0",
    "babel-jest": "^27.0.5",
    "jest": "^27.0.5",
    "vue-jest": "^3.0.4"
  }
}
```

Scripts
```
 To get started:

	cd nuxt-test
	yarn dev

  To build & start for production:

	cd nuxt-test
	yarn build
	yarn start

  To test:

	cd nuxt-test
	yarn test
```


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

## About Page
Add a new page to pages folder as `about.vue`, it will automatically craete a new route for your project on `http://localhost:3000/about`. You can also Meta details for this page as below or dynamicall by passing `this.xxx`.

```
<template>
  <div>
    <h1>About Dad Jokes</h1>
    <p>This is an app that displays corny Dad Jokes.</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'About The App',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Best place for corny dad joked'
        }
      ]
    }
  }
})
```


**************************************

## AppHeader
Create a common component to be shared between all pages. Add the `layouts/default.vue`, if its missing by defualt to include AppHeader to it.


**************************************

## Axios

https://www.smashingmagazine.com/2020/05/getting-started-axios-nuxt/
Add `'@nuxtjs/axios',` to modules in `nuxt.config.js.`. Create an async/await method and use axios as `$this.$axios.get("<url>", "<headers>")`. Example on `pages/jokes/index.vue`

```
async created() {
    const config = {
      headers: {
        'Accept': 'application/json'
      }
    }
    try {
      const res = await this.$axios.get('https://icanhazdadjoke.com/search?term=hipster', config);
      console.log(res.data);
    } catch(err) {
      console.log(err);
    }
  },
```