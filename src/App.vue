<script>
import Logo_ from './components/logo.vue'
import TitreMenu from './components/titre.vue'
import comppanier from './components/comppanier.vue'
import router from './router'

export default {
  name: 'App',
  components: {
    Logo_,
    TitreMenu,
    router,
    comppanier
  },
  data: (function () {
    return {
      menus: []
    }
  }),
  }

</script>
<template>
  <div>
  <Logo_></Logo_>
  <TitreMenu></TitreMenu>
  <h1></h1>
  <!-- <router-link to='/'><button>Retour à l'acceuil</button></router-link>
  <button a @click="$router.go(-1)">Etape précédente</button> -->
  <!-- <comppanier></comppanier> -->
  <router-view></router-view>
    </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}
</style>
