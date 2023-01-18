### In Progress...

# Weather-App

This template should help get you started developing with Vue 3 in Vite.

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Compile and Minify for Production

```sh
npm run build
```


### install Tailwindcss and configure 
```sh
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

## What I have learned in this project are:

  1. Using `Transition` component, a built-in components that can help work with transitions and animations in response to changing state <sub>[Read More...](https://vuejs.org/guide/built-ins/transition.html)</sub>
  2. Using Vue Devtools <sub>[Read More...](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd?hl=en)</sub>
  3. Using OpenWeatherMap API to fetch weather data <sub>[Read More...](https://openweathermap.org/api/one-call-3)</sub>
  4. Using `<Suspense>` which is a built-in component for orchestrating async dependencies in a component tree. <sub>[Read More...](https://vuejs.org/guide/built-ins/suspense.html)</sub>

## Dependencies
  - Tailwindcss & postcss & autoprefixer [link](https://tailwindcss.com/docs/installation/using-postcss)
  - axios [link](https://www.npmjs.com/package/axios)
  - UID [link](https://www.npmjs.com/package/uid)


  ## Note

> Use `Suspense` to render a loading state while waiting for multiple nested async dependencies down the component tree to be resolved

```vue
<template>
  <div>
    <Suspense>
      <AsyncCityView />
      <template #fallback>
        <p>Loading...</p>
      </template>
    </Suspense>
  </div>
</template>
<script setup>
import AsyncCityView from '../components/AsyncCityView.vue';


</script>
```