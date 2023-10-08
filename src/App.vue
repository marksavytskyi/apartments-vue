<script setup>
import {ref} from "vue";
import ApartmentsListVue from "./components/Apartments/ApartmentsList.vue";
import AptItems from "./components/Apartments/apartments";
</script>

<template>
  <header>
    <div class="wrapper"></div>
  </header>

  <main>
    <ApartmentsListVue :items="AptItems" />
  </main>
</template>

<style lang="scss" scoped>
#app {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  font-family: Montserrat, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.content {
  flex-grow: 1;
}
</style>
