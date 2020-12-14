# Vue3 Snippet (Visual Studio Code)

另外需要安装 "[Vue Basic Snippets](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-vue-basic-snippets)".

Code snippets for Vue (v3.x) + Vue Router (v4.x) + VueX (v4.x).

**最近要考试，没时间仔细编写文档和全面的搞源码，只能是在 2 的基础上做修改，等我 2021年 4 月之后再来调整文档和源码。**

## 规划

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue-snippets.png)

Vue 2 和 3 Template Directives 部分一样 （vscode-vue-basic-snippets）。

Vue 3 和 3 变化比较大，2 推荐 Optional 范式，3 推荐 Composition Functions 范式。Vue 中常用的 “Global API、Directives、Transition、Async Components、Instance Events、Lifecycle” 都发生了较大的变化。并且 Router/VueX 也推出了 4 版本。

另外随着 “reactive refs”、“Teleport” 新特性的引入，很多社区资源的升级都将是较大的变化。

因此将 Vue 3 和 3 的 Code Snippets 设计在一起，是不好的。

最好将 Vue 3 和 3 的 Code Snippets 各自分开，在项目中根据实际情况，在扩展中选择 `Disable (Workspace)`，如果觉得这样比较繁琐，可以在 “VS Code” 中安装 2 版本支持的扩展，在 “VS Code - Insiders” 中安装 3 版本支持的扩展。

---

![](https://raw.githubusercontent.com/caringrun/assets/master/vscode-vue3-snippets.gif)

## Supported languages (file extensions)

- JavaScript (`.js`)
- TypeScript (`.ts`)
- Vue (`.vue`)


## Resources 🤞

- [JavaScript Code Snippet - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-snippet)
- [JavaScript Comment Snippet - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=NicholasHsiang.vscode-javascript-comment)

---

## Snippets

查看源码，源码文件进行了分层，非常清晰，胜过文档描述，大致过一下大概有哪些 `prefix`。

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