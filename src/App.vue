<script>

import AppTitle from './components/AppTitle.vue'
import AppHero from './components/AppHero.vue'


export default{
  components: {
    AppTitle,
    AppHero,
  },
  data() {
    return {
      message: 'ciao Mirko'
    }

  },
  methods:{
    sayHello() {
      console.log('ciao')
    }
  }
}
</script>

<template>
  <!-- <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <div>
    <h2 @click="sayHello">{{message}}</h2>
  </div> -->
  <div>
    <AppHero></AppHero>
  </div>
  <AppTitle></AppTitle>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
