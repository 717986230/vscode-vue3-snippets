<p>
  <h1 align="center">Vue 3 Snippet (Visual Studio Code)</h1>
</p>

<p align="center">
  <a href="https://github.com/xianghongai/vscode-vue3-snippets">
    <img src="https://img.shields.io/github/repo-size/xianghongai/vscode-vue3-snippets?style=plastic&color=4ac51c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue3-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/version-short/NicholasHsiang.vscode-vue3-snippets.svg?style=plastic&color=f07b3c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue3-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/installs-short/NicholasHsiang.vscode-vue3-snippets.svg?style=plastic&color=4ac51c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue3-snippets">
    <img src="https://vsmarketplacebadge.apphb.com/rating-short/NicholasHsiang.vscode-vue3-snippets.svg?style=plastic&color=4ac51c">
  </a>
  <a href="https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue3-snippets">
    <img src="https://img.shields.io/github/license/xianghongai/vscode-vue3-snippets?maxAge=2592000&style=plastic&color=4ac51c">
  </a>
</p>

[中文](./README_CN.md)

🌈🌈🌈 First need to install "[Vue Basic Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue-basic-snippets)", **they are one combined release.**

Code snippets for Vue (v3.x) + Vue Router (v4.x) + VueX (v4.x).

## Design

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue-snippets.png)

Vue 2 and 3 Template Directives are the same (vscode-vue-basic-snippets).

Vue 2 and 3 have relatively large changes, 2 recommends the Optional paradigm, and 3 recommends the Composition Functions paradigm. The commonly used "Global API, Directives, Transition, Async Components, Instance Events, Lifecycle" in Vue have undergone major changes. And Router/VueX also launched 4 versions.

In addition, with the introduction of new features of "reactive refs" and "Teleport", the upgrade of many community resources will be major changes.

Therefore, it is not good to design Vue 2 and 3 Code Snippets together.

It is best to separate the Code Snippets of Vue 2 and 3 respectively. According to the actual situation in the project, select `Disable (Workspace)` in the extension. If you feel this is more cumbersome, you can install the extension supported by version 2 in "`VS Code`" , Install the extensions supported by version 3 in "`VS Code-Insiders`".

---

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue3-snippets.gif)

## Supported languages (file extensions)

- JavaScript (`.js`)
- JSX (`.jsx`)
- TypeScript (`.ts`)
- Vue (`.vue`)


## Resources 🤞

- [JavaScript Code Snippet - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-snippet)
- [JavaScript Comment Snippet - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-comment)

---

## Snippets

Looking at the source code, the source code files are layered, very clear, better than the document description, and roughly what are the `prefix`.

+ [Vue 3](https://v3.vuejs.org/)
    - [x] Application Config
    - [x] Application API
    - [x] Global API
    - [x] Options API
    - [x] Instance Properties
    - [x] Instance Methods
    - [x] Directives
    - [x] Special Attributes
    - [x] Built-in Components
    - [x] Reactivity API
    - [x] Composition API
+ [Vue Router 4](https://next.router.vuejs.org/), TODO (2021-4)
    - [ ] \<router-link> Props
    - [ ] \<router-link>'s v-slot
    - [ ] \<router-view> Props
    - [ ] \<router-view>'s v-slot
    - [ ] createRouter
    - [ ] createWebHistory
    - [ ] createWebHashHistory
    - [ ] createMemoryHistory
    - [ ] NavigationFailureType
    - [ ] START_LOCATION
    - [ ] Composition API
    - [ ] TypeScript
    - [ ] Router Properties
    - [ ] Router Methods
    - [ ] RouterOptions
    - [ ] RouteRecordRaw
    - [ ] RouteRecordNormalized
    - [ ] RouteLocationRaw
    - [ ] RouteLocation
    - [ ] RouteLocationNormalized
    - [ ] NavigationFailure
    - [ ] NavigationGuard
    - [ ] Component Injections
+ [Vuex 4](https://next.vuex.vuejs.org/), TODO (2021-4)
    - [ ] Vuex.Store
    - [ ] Vuex.Store Constructor Options
    - [ ] Vuex.Store Instance Properties
    - [ ] Vuex.Store Instance Methods
    - [ ] Component Binding Helpers

---


## File Name

View "Style Guide" [Priority B Rules: Strongly Recommended (Improving Readability)](https://v3.vuejs.org/style-guide/#priority-b-rules-strongly-recommended-improving-readability).

- `${TM_FILENAME_BASE/([A-Z][a-z]*)+([A-Z][a-z]*)/${1:/downcase}-${2:/downcase}/g}`, foo-bar.vue  →  `name: foo-bar`;
- `${TM_FILENAME_BASE/(.*)/${1:/pascalcase}/g}`, foo-bar.vue  →  `name: FooBar`;
- `${TM_FILENAME_BASE}`, foo-bar.vue  →  `name: foo-bar`;
- `${TM_DIRECTORY}`, foo-bar/index.vue  →  `name: foo-bar`;


## License 📃

MIT License

**Donate**

![xianghongai@gmail.com](https://raw.githubusercontent.com/caringrun/assets/master/donate.png)
