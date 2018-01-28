# Vuex Tutorial
In this article, you can learnning:

* How to install
* What is Vuex
* Hello Vuex
* Core Concepts
    * State
        * mapState Helper
    * Getters
        * mapState Helper
    * Mutations
    * Actions
    * Modules

## How to install
* Stanalone
    * [dev version](https://unpkg.com/vuex)
* `npm install vuex`

## What is Vuex
refer to: https://vuex.vuejs.org/en/intro.html

## Hello Vuex
* import vue.js & vuex.js
* index.html
* create Vuex.Store(): `store = new Vuex.Store({})`
* commit the mutation: `store.commit('increment')`

## Core Concepts
### State
* create Vuex.Store()
* declare a state.count: `{ state: { count: 0 }}`
* use in components: `this.$store.state.count` 

### Getters
* create Vuex.Store()
* declare a getters.doneTodos: `{ getters: { doneTodos: ... }}`
* use in components: `this.$store.getters.doneTodos`

### Mutations
* create Vuex.Store()
* declare a mutations.increment: `{ mutations: { increment: function(){} }}`
* use in components: `this.$store.commit('increment')`

### Actions
* create Vuex.Store()
* declare a actions.increment: `{ actions: { increment: function(){} }}`
* use in components: `this.$store.dispatch('increment')`

### Modules
* create moduleA & moduleB
* create Vuex.Store() with tow Modules: `new Vuex.Store({modules: {a: moduleA,b: moduleB}})`
* use in components: `this.$store.state.a `
