<template>
  <AppHeader />

  <main class="container pt-3">
    <router-view></router-view>
  </main>
  
</template>

<script>
  import axios from 'axios';
  import SingleCard from './components/SingleCard.vue';
  import AppHeader from './components/AppHeader.vue';
  export default {
    components : {
      AppHeader
    }
  }
</script>

<style lang="scss">
  @import "/node_modules/bootstrap/scss/bootstrap";
</style>
